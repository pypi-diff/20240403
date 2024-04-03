# Comparing `tmp/octostar_streamlit-0.1.1.tar.gz` & `tmp/octostar_streamlit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octostar_streamlit-0.1.1.tar", max compression
+gzip compressed data, was "octostar_streamlit-0.1.2.tar", max compression
```

## Comparing `octostar_streamlit-0.1.1.tar` & `octostar_streamlit-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1074 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/README.md
--rw-r--r--   0        0        0     1884 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/method_call.py
--rw-r--r--   0        0        0     7821 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/params.py
--rw-r--r--   0        0        0     6134 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/entities.py
--rw-r--r--   0        0        0      281 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/method_call.py
--rw-r--r--   0        0        0        0 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/__init__.py
--rw-r--r--   0        0        0      673 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/method_call.py
--rw-r--r--   0        0        0     1766 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/params.py
--rw-r--r--   0        0        0      222 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/params_base_model.py
--rw-r--r--   0        0        0      867 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/streamlit_executor.py
--rw-r--r--   0        0        0    10049 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/desktop.py
--rw-r--r--   0        0        0      253 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/.gitignore
--rw-r--r--   0        0        0      357 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/index.html
--rw-r--r--   0        0        0    42450 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/package-lock.json
--rw-r--r--   0        0        0      413 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/package.json
--rw-r--r--   0        0        0     1497 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/public/vite.svg
--rw-r--r--   0        0        0      835 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/core.ts
--rw-r--r--   0        0        0    15318 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/desktop.ts
--rw-r--r--   0        0        0     2373 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/main.ts
--rw-r--r--   0        0        0     4177 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/ontology.ts
--rw-r--r--   0        0        0       38 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      527 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/tsconfig.json
--rw-r--r--   0        0        0      396 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/main.py
--rw-r--r--   0        0        0     3984 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/ontology.py
--rw-r--r--   0        0        0      661 2024-04-03 00:01:49.228615 octostar_streamlit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-03 00:13:28.710115 octostar_streamlit-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-03 00:13:28.710115 octostar_streamlit-0.1.2/README.md
+-rw-r--r--   0        0        0     1884 2024-04-03 00:13:28.710115 octostar_streamlit-0.1.2/octostar_streamlit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:13:28.710115 octostar_streamlit-0.1.2/octostar_streamlit/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:13:28.710115 octostar_streamlit-0.1.2/octostar_streamlit/core/desktop/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-03 00:13:28.710115 octostar_streamlit-0.1.2/octostar_streamlit/core/desktop/method_call.py
+-rw-r--r--   0        0        0     7821 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/core/desktop/params.py
+-rw-r--r--   0        0        0     6134 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/core/entities.py
+-rw-r--r--   0        0        0      281 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/core/method_call.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/core/ontology/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/core/ontology/method_call.py
+-rw-r--r--   0        0        0     1766 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/core/ontology/params.py
+-rw-r--r--   0        0        0      222 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/core/params_base_model.py
+-rw-r--r--   0        0        0      867 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/core/streamlit_executor.py
+-rw-r--r--   0        0        0    10049 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/desktop.py
+-rw-r--r--   0        0        0      253 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/.gitignore
+-rw-r--r--   0        0        0      357 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/index.html
+-rw-r--r--   0        0        0    42450 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/package-lock.json
+-rw-r--r--   0        0        0      413 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/package.json
+-rw-r--r--   0        0        0     1497 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/public/vite.svg
+-rw-r--r--   0        0        0      835 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/core.ts
+-rw-r--r--   0        0        0    15318 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/desktop.ts
+-rw-r--r--   0        0        0     2373 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/main.ts
+-rw-r--r--   0        0        0     4177 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/ontology.ts
+-rw-r--r--   0        0        0       38 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      527 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/frontend/tsconfig.json
+-rw-r--r--   0        0        0      396 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/main.py
+-rw-r--r--   0        0        0     3984 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/octostar_streamlit/ontology.py
+-rw-r--r--   0        0        0      661 2024-04-03 00:13:28.714115 octostar_streamlit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.2/PKG-INFO
```

### Comparing `octostar_streamlit-0.1.1/LICENSE` & `octostar_streamlit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/__init__.py` & `octostar_streamlit-0.1.2/octostar_streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/method_call.py` & `octostar_streamlit-0.1.2/octostar_streamlit/core/desktop/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/params.py` & `octostar_streamlit-0.1.2/octostar_streamlit/core/desktop/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/core/entities.py` & `octostar_streamlit-0.1.2/octostar_streamlit/core/entities.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/method_call.py` & `octostar_streamlit-0.1.2/octostar_streamlit/core/ontology/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/params.py` & `octostar_streamlit-0.1.2/octostar_streamlit/core/ontology/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/core/streamlit_executor.py` & `octostar_streamlit-0.1.2/octostar_streamlit/core/streamlit_executor.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/desktop.py` & `octostar_streamlit-0.1.2/octostar_streamlit/desktop.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/frontend/package-lock.json` & `octostar_streamlit-0.1.2/octostar_streamlit/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/frontend/public/vite.svg` & `octostar_streamlit-0.1.2/octostar_streamlit/frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/core.ts` & `octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/core.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/desktop.ts` & `octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/desktop.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/main.ts` & `octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/main.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/ontology.ts` & `octostar_streamlit-0.1.2/octostar_streamlit/frontend/src/ontology.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/frontend/tsconfig.json` & `octostar_streamlit-0.1.2/octostar_streamlit/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/octostar_streamlit/ontology.py` & `octostar_streamlit-0.1.2/octostar_streamlit/ontology.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.1/pyproject.toml` & `octostar_streamlit-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octostar-streamlit"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Oleksandr Korzhov <another.fullstack.dev@gmail.com>"]
 readme = "README.md"
 
 [tool.mypy]
 python_version = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 check_untyped_defs = true
```

### Comparing `octostar_streamlit-0.1.1/PKG-INFO` & `octostar_streamlit-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octostar-streamlit
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Oleksandr Korzhov
 Author-email: another.fullstack.dev@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

