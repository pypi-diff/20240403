# Comparing `tmp/last_layer-0.1.8.tar.gz` & `tmp/last_layer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "last_layer-0.1.8.tar", max compression
+gzip compressed data, was "last_layer-0.1.9.tar", max compression
```

## Comparing `last_layer-0.1.8.tar` & `last_layer-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2024-03-22 11:10:14.397163 last_layer-0.1.8/LICENSE
--rw-r--r--   0        0        0     5703 2024-03-22 11:59:38.574691 last_layer-0.1.8/Readme.md
--rw-r--r--   0        0        0      103 2024-03-27 21:03:32.083818 last_layer-0.1.8/last_layer/__init__.py
--rw-r--r--   0        0        0      297 2024-03-22 11:50:23.509561 last_layer-0.1.8/last_layer/__main__.py
--rw-r--r--   0        0        0     2181 2024-03-27 21:04:03.012283 last_layer-0.1.8/last_layer/core.py
--rw-r--r--   0        0        0  3452242 2024-03-27 17:28:16.030725 last_layer-0.1.8/last_layer/lib/library.so
--rw-r--r--   0        0        0  3434392 2024-03-27 17:28:13.628833 last_layer-0.1.8/last_layer/lib/library_linux.so
--rw-r--r--   0        0        0      997 2024-03-27 21:04:09.825540 last_layer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6571 1970-01-01 00:00:00.000000 last_layer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-03-22 11:10:14.397163 last_layer-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5703 2024-03-22 11:59:38.574691 last_layer-0.1.9/Readme.md
+-rw-r--r--   0        0        0      103 2024-03-27 21:03:32.083818 last_layer-0.1.9/last_layer/__init__.py
+-rw-r--r--   0        0        0      297 2024-03-22 11:50:23.509561 last_layer-0.1.9/last_layer/__main__.py
+-rw-r--r--   0        0        0     2420 2024-03-27 21:39:42.993488 last_layer-0.1.9/last_layer/core.py
+-rw-r--r--   0        0        0  3452242 2024-03-27 17:28:16.030725 last_layer-0.1.9/last_layer/lib/library.so
+-rw-r--r--   0        0        0  3434392 2024-03-27 17:28:13.628833 last_layer-0.1.9/last_layer/lib/library_linux.so
+-rw-r--r--   0        0        0     1005 2024-03-27 21:39:52.832152 last_layer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 last_layer-0.1.9/PKG-INFO
```

### Comparing `last_layer-0.1.8/LICENSE` & `last_layer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `last_layer-0.1.8/Readme.md` & `last_layer-0.1.9/Readme.md`

 * *Files identical despite different names*

### Comparing `last_layer-0.1.8/last_layer/core.py` & `last_layer-0.1.9/last_layer/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,27 @@
 elif platform.system().lower() == "windows":
     raise Warning("Windows is not supported.")
 else:
     lib_file = "library.so"  # Fallback or default to non-Linux
 
 # Try to load the library from the package resources
 so_path = pkg_resources.resource_filename("last_layer", f"lib/{lib_file}")
+
 try:
     library = ctypes.cdll.LoadLibrary(so_path)
 except OSError:
     # Fallback to trying to load directly in case of failure
-    library = ctypes.cdll.LoadLibrary(f"lib/{lib_file}")
+    for path in [f"lib/{lib_file}", f"/var/task/last_layer/{lib_file}"]:
+        try:
+            library = ctypes.cdll.LoadLibrary(f"lib/{lib_file}")
+            break
+        except OSError:
+            continue
+    else:
+        raise ImportError(f"Failed to load shared library {lib_file}")
 
 Threats = [
     "MixedLangMarker",
     "InvisibleUnicodeDetector",
     "MarkdownLinkDetector",
     "HiddenTextDetector",
     "Base64Detector",
```

### Comparing `last_layer-0.1.8/last_layer/lib/library.so` & `last_layer-0.1.9/last_layer/lib/library.so`

 * *Files identical despite different names*

### Comparing `last_layer-0.1.8/last_layer/lib/library_linux.so` & `last_layer-0.1.9/last_layer/lib/library_linux.so`

 * *Files identical despite different names*

### Comparing `last_layer-0.1.8/pyproject.toml` & `last_layer-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "last_layer"
-version = "0.1.8"
+version = "0.1.9"
 description = "Ultra-fast, Low Latency LLM security solution"
-authors = ["Tangln <gh@tangln.com>"]
-maintainers = ["Tangln <gh@tangln.com>"]
+authors = ["Last Layer <gh@tangln.com>"]
+maintainers = ["Last Layer <gh@tangln.com>"]
 repository = "https://github.com/tangln/last_layer"
 license = "MIT"
 readme = "Readme.md"
 keywords = [
     "llm",
     "language model",
     "security",
```

### Comparing `last_layer-0.1.8/PKG-INFO` & `last_layer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: last_layer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ultra-fast, Low Latency LLM security solution
 Home-page: https://github.com/tangln/last_layer
 License: MIT
 Keywords: llm,language model,security,adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,PII detection,self-hardening
-Author: Tangln
+Author: Last Layer
 Author-email: gh@tangln.com
-Maintainer: Tangln
+Maintainer: Last Layer
 Maintainer-email: gh@tangln.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

