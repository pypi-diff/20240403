# Comparing `tmp/pldag-0.4.2.tar.gz` & `tmp/pldag-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.4.2.tar", max compression
+gzip compressed data, was "pldag-0.4.3.tar", max compression
```

## Comparing `pldag-0.4.2.tar` & `pldag-0.4.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.4.2/LICENSE
--rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.4.2/README.md
--rw-r--r--   0        0        0    13205 2024-04-03 11:58:05.815287 pldag-0.4.2/pldag/__init__.py
--rw-r--r--   0        0        0      278 2024-04-03 12:07:27.547115 pldag-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.4.3/README.md
+-rw-r--r--   0        0        0    13313 2024-04-03 14:39:22.258188 pldag-0.4.3/pldag/__init__.py
+-rw-r--r--   0        0        0      278 2024-04-03 14:39:29.337734 pldag-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.4.3/PKG-INFO
```

### Comparing `pldag-0.4.2/LICENSE` & `pldag-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.4.2/README.md` & `pldag-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.4.2/pldag/__init__.py` & `pldag-0.4.3/pldag/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,20 +114,20 @@
 
     def set_primitives(self, aliases: List[str], bound: complex = complex(0,1)) -> List[str]:
         """Add multiple primitive prime factor matrices"""
         for alias in aliases:
             self.set_primitive(alias, bound)
         return aliases
 
-    def _set_composite(self, valued_children: list, negate: bool = False, aliases: List[str] = []) -> str:
+    def _set_composite(self, valued_children: list, negate: bool = False, aliases: List[str] = [], force_id: Optional[str] = None) -> str:
         for child_alias, value, hide in valued_children:
             if child_alias not in self._imap:
                 self.set_primitive(child_alias, value, hide)
 
-        _id = sha256(str(valued_children).encode()).hexdigest()
+        _id = sha256(str(valued_children).encode()).hexdigest() if force_id is None else force_id
         if _id in self._imap:
             arr = np.zeros(self._amat.shape[1], dtype=np.int64)
             arr[[self._imap[child] for child,_,_ in valued_children]] = 1
             self._amat[self._imap[_id]] = arr
             self._dvec[self._imap[_id]] = complex(0, 1)
             self._nvec[self._imap[_id]] = negate * 1
         else:
@@ -143,15 +143,15 @@
             for alias in aliases:
                 self._amap[alias] = _id
         else:
             self._amap[_id] = _id
 
         return _id
     
-    def set_composite(self, children: list, bias: int, negate: bool = False, aliases: List[str] = []) -> str:
+    def set_composite(self, children: list, bias: int, negate: bool = False, aliases: List[str] = [], force_id: Optional[str] = None) -> str:
         """
             Add a composite prime factor matrix.
             If alias already registred, only the prime factor matrix is updated.
         """
         valued_children = sorted(
             chain(
                 map(
@@ -168,15 +168,15 @@
                         complex(bias, bias), 
                         True,
                     )
                 ]
             ), 
             key=lambda x: x[0]
         )
-        return self._set_composite(valued_children, negate, aliases)
+        return self._set_composite(valued_children, negate, aliases, force_id)
 
     @staticmethod
     def _prop_algo(A: np.ndarray, F: np.ndarray, B: np.ndarray, forced: np.ndarray, max_iterations: int = 100):
 
         """
             Propagation algorithm.
```

### Comparing `pldag-0.4.2/PKG-INFO` & `pldag-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

