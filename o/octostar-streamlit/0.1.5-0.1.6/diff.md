# Comparing `tmp/octostar_streamlit-0.1.5.tar.gz` & `tmp/octostar_streamlit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octostar_streamlit-0.1.5.tar", max compression
+gzip compressed data, was "octostar_streamlit-0.1.6.tar", max compression
```

## Comparing `octostar_streamlit-0.1.5.tar` & `octostar_streamlit-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0     1073 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/LICENSE
--rw-r--r--   0        0        0      324 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/README.md
--rw-r--r--   0        0        0     1965 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/desktop/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/desktop/method_call.py
--rw-r--r--   0        0        0     7821 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/desktop/params.py
--rw-r--r--   0        0        0     6134 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/entities.py
--rw-r--r--   0        0        0      281 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/method_call.py
--rw-r--r--   0        0        0        0 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/ontology/__init__.py
--rw-r--r--   0        0        0      673 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/ontology/method_call.py
--rw-r--r--   0        0        0     1766 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/ontology/params.py
--rw-r--r--   0        0        0      222 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/params_base_model.py
--rw-r--r--   0        0        0      867 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/core/streamlit_executor.py
--rw-r--r--   0        0        0    10049 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/desktop.py
--rw-r--r--   0        0        0      253 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/.gitignore
--rw-r--r--   0        0        0      356 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/index.html
--rw-r--r--   0        0        0    42450 2024-04-03 16:42:55.715278 octostar_streamlit-0.1.5/octostar_streamlit/frontend/package-lock.json
--rw-r--r--   0        0        0      413 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/package.json
--rw-r--r--   0        0        0     1497 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/public/vite.svg
--rw-r--r--   0        0        0      835 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/core.ts
--rw-r--r--   0        0        0    14114 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/desktop.ts
--rw-r--r--   0        0        0     2373 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/main.ts
--rw-r--r--   0        0        0     4166 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/ontology.ts
--rw-r--r--   0        0        0       38 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      527 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/tsconfig.json
--rw-r--r--   0        0        0       86 2024-04-03 16:42:37.163216 octostar_streamlit-0.1.5/octostar_streamlit/frontend/vite.config.ts
--rw-r--r--   0        0        0     3984 2024-04-03 16:42:37.167216 octostar_streamlit-0.1.5/octostar_streamlit/ontology.py
--rw-r--r--   0        0        0      677 2024-04-03 16:42:37.167216 octostar_streamlit-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/LICENSE
+-rw-r--r--   0        0        0      324 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/README.md
+-rw-r--r--   0        0        0     1965 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/core/desktop/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/core/desktop/method_call.py
+-rw-r--r--   0        0        0     7821 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/core/desktop/params.py
+-rw-r--r--   0        0        0     6134 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/core/entities.py
+-rw-r--r--   0        0        0      281 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/core/method_call.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/core/ontology/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-03 16:59:38.566802 octostar_streamlit-0.1.6/octostar_streamlit/core/ontology/method_call.py
+-rw-r--r--   0        0        0     1766 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/core/ontology/params.py
+-rw-r--r--   0        0        0      222 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/core/params_base_model.py
+-rw-r--r--   0        0        0      867 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/core/streamlit_executor.py
+-rw-r--r--   0        0        0    10049 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/desktop.py
+-rw-r--r--   0        0        0      253 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/.gitignore
+-rw-r--r--   0        0        0   235160 2024-04-03 17:00:06.798939 octostar_streamlit-0.1.6/octostar_streamlit/frontend/dist/assets/index-BCMUK_M-.js
+-rw-r--r--   0        0        0      383 2024-04-03 17:00:06.798939 octostar_streamlit-0.1.6/octostar_streamlit/frontend/dist/index.html
+-rw-r--r--   0        0        0     1497 2024-04-03 17:00:06.606938 octostar_streamlit-0.1.6/octostar_streamlit/frontend/dist/vite.svg
+-rw-r--r--   0        0        0      356 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/index.html
+-rw-r--r--   0        0        0    42450 2024-04-03 17:00:02.930920 octostar_streamlit-0.1.6/octostar_streamlit/frontend/package-lock.json
+-rw-r--r--   0        0        0      413 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/package.json
+-rw-r--r--   0        0        0     1497 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/public/vite.svg
+-rw-r--r--   0        0        0      835 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/core.ts
+-rw-r--r--   0        0        0    14114 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/desktop.ts
+-rw-r--r--   0        0        0     2373 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/main.ts
+-rw-r--r--   0        0        0     4166 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/ontology.ts
+-rw-r--r--   0        0        0       38 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      527 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/tsconfig.json
+-rw-r--r--   0        0        0       86 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/frontend/vite.config.ts
+-rw-r--r--   0        0        0     3984 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/octostar_streamlit/ontology.py
+-rw-r--r--   0        0        0      736 2024-04-03 16:59:38.570802 octostar_streamlit-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.6/PKG-INFO
```

### Comparing `octostar_streamlit-0.1.5/LICENSE` & `octostar_streamlit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/__init__.py` & `octostar_streamlit-0.1.6/octostar_streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/core/desktop/method_call.py` & `octostar_streamlit-0.1.6/octostar_streamlit/core/desktop/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/core/desktop/params.py` & `octostar_streamlit-0.1.6/octostar_streamlit/core/desktop/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/core/entities.py` & `octostar_streamlit-0.1.6/octostar_streamlit/core/entities.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/core/ontology/method_call.py` & `octostar_streamlit-0.1.6/octostar_streamlit/core/ontology/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/core/ontology/params.py` & `octostar_streamlit-0.1.6/octostar_streamlit/core/ontology/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/core/streamlit_executor.py` & `octostar_streamlit-0.1.6/octostar_streamlit/core/streamlit_executor.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/desktop.py` & `octostar_streamlit-0.1.6/octostar_streamlit/desktop.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/frontend/package-lock.json` & `octostar_streamlit-0.1.6/octostar_streamlit/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/frontend/public/vite.svg` & `octostar_streamlit-0.1.6/octostar_streamlit/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/core.ts` & `octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/core.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/desktop.ts` & `octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/desktop.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/main.ts` & `octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/main.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/frontend/src/ontology.ts` & `octostar_streamlit-0.1.6/octostar_streamlit/frontend/src/ontology.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/frontend/tsconfig.json` & `octostar_streamlit-0.1.6/octostar_streamlit/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/octostar_streamlit/ontology.py` & `octostar_streamlit-0.1.6/octostar_streamlit/ontology.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.5/pyproject.toml` & `octostar_streamlit-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "octostar-streamlit"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 license = "MIT"
 authors = ["Oleksandr Korzhov <another.fullstack.dev@gmail.com>"]
 readme = "README.md"
+include = [
+    "octostar_streamlit/frontend/dist/**/*",
+]
 
 [tool.mypy]
 python_version = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 check_untyped_defs = true
 ignore_missing_imports = true
 warn_redundant_casts = true
 warn_unused_ignores = true
```

### Comparing `octostar_streamlit-0.1.5/PKG-INFO` & `octostar_streamlit-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octostar-streamlit
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: MIT
 Author: Oleksandr Korzhov
 Author-email: another.fullstack.dev@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

