# Comparing `tmp/kontext-1.2.0.tar.gz` & `tmp/kontext-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kontext-1.2.0.tar", max compression
+gzip compressed data, was "kontext-1.2.1.tar", max compression
```

## Comparing `kontext-1.2.0.tar` & `kontext-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1092 2024-02-23 13:21:32.262991 kontext-1.2.0/LICENSE
--rw-r--r--   0        0        0     1537 2024-02-23 13:21:32.262991 kontext-1.2.0/README.md
--rw-r--r--   0        0        0      446 2024-02-23 13:21:32.262991 kontext-1.2.0/kontext/__init__.py
--rw-r--r--   0        0        0      738 2024-02-23 13:21:32.262991 kontext-1.2.0/kontext/log_record.py
--rw-r--r--   0        0        0     4249 2024-02-23 13:21:32.262991 kontext-1.2.0/kontext/main.py
--rw-r--r--   0        0        0        1 2024-02-23 13:21:32.262991 kontext-1.2.0/kontext/py.typed
--rw-r--r--   0        0        0     2340 2024-02-23 13:21:32.262991 kontext-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2411 1970-01-01 00:00:00.000000 kontext-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-03 08:53:01.232352 kontext-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1537 2024-04-03 08:53:01.232352 kontext-1.2.1/README.md
+-rw-r--r--   0        0        0      446 2024-04-03 08:53:01.236353 kontext-1.2.1/kontext/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-03 08:53:01.236353 kontext-1.2.1/kontext/log_record.py
+-rw-r--r--   0        0        0     4249 2024-04-03 08:53:01.236353 kontext-1.2.1/kontext/main.py
+-rw-r--r--   0        0        0        1 2024-04-03 08:53:01.236353 kontext-1.2.1/kontext/py.typed
+-rw-r--r--   0        0        0     2340 2024-04-03 08:53:01.236353 kontext-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2411 1970-01-01 00:00:00.000000 kontext-1.2.1/PKG-INFO
```

### Comparing `kontext-1.2.0/LICENSE` & `kontext-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kontext-1.2.0/README.md` & `kontext-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kontext-1.2.0/kontext/log_record.py` & `kontext-1.2.1/kontext/log_record.py`

 * *Files identical despite different names*

### Comparing `kontext-1.2.0/kontext/main.py` & `kontext-1.2.1/kontext/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,35 @@
 
     @property
     def _default_cls(self) -> Type[ContextDataProtocol]:
         raise NotImplementedError
 
 
 class AbstractContext(ContextMeta):
+    def __enter__(self) -> None:
+        data = _get_or_default(self._kontext, self._default_cls)
+        new_data = data.copy()
+        new_data.update(data)
+        self._token = self._kontext.set(new_data)
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[Exception]],
+        exc_value: Optional[Exception],
+        traceback: Any,
+    ) -> None:
+        self._kontext.reset(self._token)
+
+
+class Context(
+    AbstractContext,
+    metaclass=ContextFactory,
+    kontext=_context,
+    default_cls=ContextData,
+):
     @overload
     def __call__(self, func: Callable[P, Awaitable[R]]) -> Callable[P, Awaitable[R]]:
         ...  # pragma: no cover
 
     @overload
     def __call__(self, func: Callable[P, R]) -> Callable[P, R]:
         ...  # pragma: no cover
@@ -77,49 +98,26 @@
     def __call__(
         self, func: Callable[P, R]
     ) -> Union[Callable[P, Awaitable[R]], Callable[P, R]]:
         if iscoroutinefunction(func):
 
             @wraps(func)
             async def async_inner(*args: P.args, **kwargs: P.kwargs) -> R:
-                with self:
+                with Context():
                     return await func(*args, **kwargs)  # type: ignore
 
             return async_inner
 
         @wraps(func)
         def sync_inner(*args: P.args, **kwargs: P.kwargs) -> R:
-            with self:
+            with Context():
                 return func(*args, **kwargs)
 
         return sync_inner
 
-    def __enter__(self) -> None:
-        data = _get_or_default(self._kontext, self._default_cls)
-        new_data = data.copy()
-        new_data.update(data)
-        self._token = self._kontext.set(new_data)
-
-    def __exit__(
-        self,
-        exc_type: Optional[Type[Exception]],
-        exc_value: Optional[Exception],
-        traceback: Any,
-    ) -> None:
-        self._kontext.reset(self._token)
-
-
-class Context(
-    AbstractContext,
-    metaclass=ContextFactory,
-    kontext=_context,
-    default_cls=ContextData,
-):
-    pass
-
 
 class ContextProxyProtocol(Protocol):  # pragma: no cover
     def __setitem__(self, key: Any, item: Any) -> None:
         ...
 
     def __getitem__(self, key: Any) -> Any:
         ...
```

### Comparing `kontext-1.2.0/pyproject.toml` & `kontext-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.0"
+version = "1.2.1"
 tag_format = "$version"
 version_files = [
     "kontext/__init__.py",
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "kontext"
-version = "1.2.0"
+version = "1.2.1"
 description = "Easy contextual information logging"
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/kontext"
 homepage = "https://pypi.org/project/kontext"
 keywords = ["contextvar", "logging", "context-logging"]
```

### Comparing `kontext-1.2.0/PKG-INFO` & `kontext-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kontext
-Version: 1.2.0
+Version: 1.2.1
 Summary: Easy contextual information logging
 Home-page: https://pypi.org/project/kontext
 License: MIT
 Keywords: contextvar,logging,context-logging
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
```

