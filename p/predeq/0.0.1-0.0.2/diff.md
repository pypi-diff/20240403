# Comparing `tmp/predeq-0.0.1.tar.gz` & `tmp/predeq-0.0.2.tar.gz`

## Comparing `predeq-0.0.1.tar` & `predeq-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 predeq-0.0.1/src/predeq/__init__.py
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 predeq-0.0.1/src/predeq/_predeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 predeq-0.0.1/src/predeq/recipes.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 predeq-0.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 predeq-0.0.1/LICENSE
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 predeq-0.0.1/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 predeq-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 predeq-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 predeq-0.0.2/src/predeq/__init__.py
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 predeq-0.0.2/src/predeq/_predeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 predeq-0.0.2/src/predeq/recipes.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 predeq-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 predeq-0.0.2/LICENSE
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 predeq-0.0.2/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 predeq-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 predeq-0.0.2/PKG-INFO
```

### Comparing `predeq-0.0.1/src/predeq/_predeq.py` & `predeq-0.0.2/src/predeq/_predeq.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,106 +1,132 @@
 import ast
-from functools import partial
-from inspect import getsource, isfunction
+from functools import cached_property, partial
+from inspect import getsource, iscode, isfunction
 from itertools import chain
 
 
 class predeq:
     def __init__(self, predicate) -> None:
         self.pred = predicate
-        self.source = _get_pred_body(predicate)
+
+    @cached_property
+    def _cached_repr(self):
+        predicate = (
+            # show source for lambdas, but __name__ for functions (function body might be too long)
+            (_get_callable_source(self.pred) if islambda(self.pred) else getattr(self.pred, '__name__', None))
+            # if not available, fallback to repr
+            or repr(self.pred)
+        )
+        return f'<predeq to meet {predicate}>'
 
     def __repr__(self) -> str:
-        return '<' + self.source + '>'
+        return self._cached_repr
 
     def __eq__(self, other):
         return self.pred(other)
 
 
 _DUMMY_POSITION = {'lineno': 1, 'col_offset': 0}
+_ENABLE_ONE_NODE_SHORT_PATH = True  # see _get_pred_body() below
 
 
-def _get_pred_body(predicate) -> 'str | None':
-    if not isfunction(predicate) and hasattr(predicate, '__call__'):
-        predicate = predicate.__call__
+def _get_callable_source(clbl) -> 'str | None':
+    if not isfunction(clbl) and hasattr(clbl, '__call__'):
+        clbl = clbl.__call__
 
     try:
-        full_source = getsource(predicate).strip()
+        full_source = getsource(clbl).strip()
     except OSError:
         return None
 
     # Problem: the source code returned by inspect.get_source() often has unwanted additional context, such as:
     #   - the statement where lambda is defined (e.g. "x = lambda: None" or "print(getsource(lambda: None))")
     #   - in pytest environment, because of assertion rewrite, source offsets are not entirely correct,
     #     and might include the whole assert statement or even the whole test function.
     # Solution: parse the AST of whatever `getsource()` returns, and find the function or lambda node
-    # which compiles to the same bytecode as original predicate. If there is only one function or lambda,
-    # we can assume it is the one we need (to avoid unnecessary compilation).
-
-    looking_for_lambda = islambda(predicate)
-    nodes = filter_instance(ast.Lambda if looking_for_lambda else ast.FunctionDef, ast.walk(ast.parse(full_source)))
+    # which compiles to the same bytecode as original callable.
 
-    if (first := next(nodes, None)) is None:
-        # no func/lambda node found in AST, should not happen
+    try:
+        tree = ast.parse(full_source)
+    except SyntaxError:
+        # the context available in `full_source` is not a valid code on its own
         return None
 
-    if (second := next(nodes, None)) is None:
-        # there is only `first` node, return its source segment
-        return ast.get_source_segment(full_source, first)
-
-    # there is more than one, prepend first and second to the iterator and compare by bytecode
-    freevars = predicate.__code__.co_freevars
-    compile_node = _compile_node if not freevars else partial(_compile_node_with_freevars, freevars)
-    for node in chain((first, second), nodes):
+    looking_for_lambda = islambda(clbl)
+    nodes = filter_instance(ast.Lambda if looking_for_lambda else ast.FunctionDef, ast.walk(tree))
+
+    # _ENABLE_ONE_NODE_SHORT_PATH enables "short path": if there is only one function node in AST of the source
+    # returned by `getsource()`, it is assumed that this is the function we are looking source code for.
+    # It is enabled by default, but omitted in tests to verify this assumption and bytecode comparison code.
+    if _ENABLE_ONE_NODE_SHORT_PATH:
+        if (first := next(nodes, None)) is None:
+            # no func/lambda node found in AST, should not happen
+            return None
+
+        if (second := next(nodes, None)) is None:
+            # there is only `first` node, return its source segment
+            return ast.get_source_segment(full_source, first)
+
+        # there is more than one, prepend first and second to the iterator and compare by bytecode
+        nodes = chain((first, second), nodes)
+
+    compile_node = _get_node_compiler(clbl.__code__)
+    for node in nodes:
+        # lambda node has to be wrapped into Expr to be compiled, see `echo lambda:0 | python -m ast`
         code = compile_node(ast.Expr(node, **_DUMMY_POSITION) if looking_for_lambda else node)
-        if code.co_code == predicate.__code__.co_code:
+        if code.co_code == clbl.__code__.co_code:
             return ast.get_source_segment(full_source, node)
 
     return None
 
 
+def _get_node_compiler(code):
+    # When `node` is compiled in module scope, names other than its arguments are loaded from global scope
+    # using LOAD_GLOBAL instruction. However, sometimes the function has variables captured from outer scope,
+    # which should be loaded by LOAD_DEREF. This causes a difference in the bytecode of the recompiled node.
+
+    # If a function's code has non-empty `co_freevars` (names of variables captured from outer scope),
+    # the node is compiled in the scope of an artificial function which has those freevars defined.
+    # The compiler then produces LOAD_DEREF instructions, and the bytecode is equal to original function's one.
+    # Otherwise, module scope compiler is used because it does not do unnecessary work.
+
+    freevars = code.co_freevars
+    return _compile_node if not freevars else partial(_compile_node_with_freevars, freevars)
+
+
+def _find_code(iterable, *default):
+    return next(filter(iscode, iterable), *default)
+
+
 def _compile_node(node):
     # get node's code object from module's co_consts
-    # python <= 3.10: co_consts = (<code object from node>, 'func_name', None)
-    # python >= 3.11: co_consts = (<code object from node>, None)
-    return compile(ast.Module([node], []), '<dummy>', 'exec').co_consts[0]
+    return _find_code(compile(ast.Module([node], []), '<dummy>', 'exec').co_consts)
 
 
 _NO_ARGS = ast.arguments(posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[])
 
 
 def _compile_node_with_freevars(freevars, node):
     """Compile `node` in the function scope with `freevars` defined."""
 
-    # When `node` is compiled in module scope, names other than its arguments are loaded from global scope
-    # using LOAD_GLOBAL instruction. However, sometimes the predicate has variables captured from outer scope,
-    # which will be loaded by LOAD_DEREF. This causes a difference in the bytecode of the recompiled node.
-
-    # If a predicate's code has non-empty `co_freevars` (names of variables captured from outer scope),
-    # the node is compiled in the scope of a dummy function which has those freevars defined.
-    # The compiler then produces LOAD_DEREF instructions, and the bytecode is equal to original predicate's one.
-
-    outer_node = _compile_node(ast.FunctionDef(
+    # get inner node's code object from outer node's co_consts
+    return _find_code(_compile_node(ast.FunctionDef(
         **_DUMMY_POSITION,
         name='@outer_scope@',  # use a syntactically invalid name to avoid any potential name clashes
         args=_NO_ARGS,
         decorator_list=[],
         body=[
             ast.Assign(
                 [ast.Name(freevar, ctx=ast.Store(), **_DUMMY_POSITION) for freevar in freevars],
                 ast.Constant(None, **_DUMMY_POSITION),
                 **_DUMMY_POSITION
             ),
             node,
         ],
-    ))
-    # get inner node's code object from outer node's co_consts
-    # python <= 3.10: co_consts = (None, <code object from node>, 'func_name')
-    # python >= 3.11: co_consts = (None, <code object from node>)
-    return outer_node.co_consts[1]
+    )).co_consts)
 
 
 def islambda(obj):
     # apparently there is no more reliable method than checking __name__
     return isfunction(obj) and obj.__name__ == '<lambda>'
```

### Comparing `predeq-0.0.1/LICENSE` & `predeq-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `predeq-0.0.1/PKG-INFO` & `predeq-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.3
 Name: predeq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Predicate-based equivalence testing
 Project-URL: Homepage, https://github.com/petuzk/predeq
 Author-email: Taras Radchenko <petuzk.dev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
+Provides-Extra: dev
+Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # predeq
 
 PredEq is a utility library for testing objects using an equivalence predicate.
 At its core, the `predeq(predicate)` is an object which tests equal to `X` if `predicate(X)` returns True.
```

