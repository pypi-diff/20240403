# Comparing `tmp/types-aiofiles-23.2.0.20240331.tar.gz` & `tmp/types-aiofiles-23.2.0.20240403.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiofiles-23.2.0.20240331.tar", last modified: Sun Mar 31 02:18:25 2024, max compression
+gzip compressed data, was "types-aiofiles-23.2.0.20240403.tar", last modified: Wed Apr  3 02:15:09 2024, max compression
```

## Comparing `types-aiofiles-23.2.0.20240331.tar` & `types-aiofiles-23.2.0.20240403.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:25.547433 types-aiofiles-23.2.0.20240331/
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-31 02:18:25.547433 types-aiofiles-23.2.0.20240331/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:25.547433 types-aiofiles-23.2.0.20240331/aiofiles-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/os.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/ospath.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:25.547433 types-aiofiles-23.2.0.20240331/aiofiles-stubs/tempfile/
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/tempfile/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/tempfile/temptypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:25.547433 types-aiofiles-23.2.0.20240331/aiofiles-stubs/threadpool/
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/threadpool/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/threadpool/binary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/threadpool/text.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-31 02:17:27.000000 types-aiofiles-23.2.0.20240331/aiofiles-stubs/threadpool/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 02:18:25.547433 types-aiofiles-23.2.0.20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:25.547433 types-aiofiles-23.2.0.20240331/types_aiofiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/types_aiofiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/types_aiofiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/types_aiofiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-31 02:18:25.000000 types-aiofiles-23.2.0.20240331/types_aiofiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:15:09.018793 types-aiofiles-23.2.0.20240403/
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-03 02:15:07.000000 types-aiofiles-23.2.0.20240403/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 02:15:07.000000 types-aiofiles-23.2.0.20240403/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-03 02:15:09.018793 types-aiofiles-23.2.0.20240403/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:15:09.014793 types-aiofiles-23.2.0.20240403/aiofiles-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-03 02:15:07.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/os.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/ospath.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:15:07.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:15:09.014793 types-aiofiles-23.2.0.20240403/aiofiles-stubs/tempfile/
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/tempfile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/tempfile/temptypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:15:09.018793 types-aiofiles-23.2.0.20240403/aiofiles-stubs/threadpool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/threadpool/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/threadpool/binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/threadpool/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-03 02:14:57.000000 types-aiofiles-23.2.0.20240403/aiofiles-stubs/threadpool/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:15:09.018793 types-aiofiles-23.2.0.20240403/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-03 02:15:07.000000 types-aiofiles-23.2.0.20240403/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:15:09.018793 types-aiofiles-23.2.0.20240403/types_aiofiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-03 02:15:08.000000 types-aiofiles-23.2.0.20240403/types_aiofiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-03 02:15:08.000000 types-aiofiles-23.2.0.20240403/types_aiofiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:15:08.000000 types-aiofiles-23.2.0.20240403/types_aiofiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 02:15:08.000000 types-aiofiles-23.2.0.20240403/types_aiofiles.egg-info/top_level.txt
```

### Comparing `types-aiofiles-23.2.0.20240331/CHANGELOG.md` & `types-aiofiles-23.2.0.20240403/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 23.2.0.20240403 (2024-04-03)
+
+[aiofiles] Annotate AiofilesContextManagerTempDir (#11705)
+
 ## 23.2.0.20240331 (2024-03-31)
 
 Remove bare Incomplete annotations in third-party stubs (#11671)
 
 ## 23.2.0.20240311 (2024-03-11)
 
 Use PEP 570 syntax in third party stubs (#11554)
```

### Comparing `types-aiofiles-23.2.0.20240331/PKG-INFO` & `types-aiofiles-23.2.0.20240403/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiofiles
-Version: 23.2.0.20240331
+Version: 23.2.0.20240403
 Summary: Typing stubs for aiofiles
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-aiofiles` aims to provide accurate annotations
 for `aiofiles==23.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `6d19a17f57762815426942c21d0fadc91aa1e817` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
```

### Comparing `types-aiofiles-23.2.0.20240331/aiofiles-stubs/base.pyi` & `types-aiofiles-23.2.0.20240403/aiofiles-stubs/base.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.2.0.20240331/aiofiles-stubs/os.pyi` & `types-aiofiles-23.2.0.20240403/aiofiles-stubs/os.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.2.0.20240331/aiofiles-stubs/ospath.pyi` & `types-aiofiles-23.2.0.20240403/aiofiles-stubs/ospath.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.2.0.20240331/aiofiles-stubs/tempfile/__init__.pyi` & `types-aiofiles-23.2.0.20240403/aiofiles-stubs/tempfile/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -252,8 +252,8 @@
     prefix: bytes | None = None,
     dir: BytesPath | None = None,
     loop: AbstractEventLoop | None = None,
     executor: Incomplete | None = None,
 ) -> AiofilesContextManagerTempDir[None, None, AsyncTemporaryDirectory]: ...
 
 class AiofilesContextManagerTempDir(AiofilesContextManager[_T_co, _T_contra, _V_co]):
-    async def __aenter__(self): ...
+    async def __aenter__(self) -> str: ...  # type: ignore[override]
```

### Comparing `types-aiofiles-23.2.0.20240331/aiofiles-stubs/tempfile/temptypes.pyi` & `types-aiofiles-23.2.0.20240403/aiofiles-stubs/tempfile/temptypes.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.2.0.20240331/aiofiles-stubs/threadpool/__init__.pyi` & `types-aiofiles-23.2.0.20240403/aiofiles-stubs/threadpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.2.0.20240331/aiofiles-stubs/threadpool/binary.pyi` & `types-aiofiles-23.2.0.20240403/aiofiles-stubs/threadpool/binary.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.2.0.20240331/aiofiles-stubs/threadpool/text.pyi` & `types-aiofiles-23.2.0.20240403/aiofiles-stubs/threadpool/text.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.2.0.20240331/setup.py` & `types-aiofiles-23.2.0.20240403/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-aiofiles` aims to provide accurate annotations
 for `aiofiles==23.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `6d19a17f57762815426942c21d0fadc91aa1e817` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="23.2.0.20240331",
+      version="23.2.0.20240403",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md",
```

### Comparing `types-aiofiles-23.2.0.20240331/types_aiofiles.egg-info/PKG-INFO` & `types-aiofiles-23.2.0.20240403/types_aiofiles.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiofiles
-Version: 23.2.0.20240331
+Version: 23.2.0.20240403
 Summary: Typing stubs for aiofiles
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-aiofiles` aims to provide accurate annotations
 for `aiofiles==23.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `6d19a17f57762815426942c21d0fadc91aa1e817` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
```

### Comparing `types-aiofiles-23.2.0.20240331/types_aiofiles.egg-info/SOURCES.txt` & `types-aiofiles-23.2.0.20240403/types_aiofiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

