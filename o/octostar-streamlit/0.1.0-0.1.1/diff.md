# Comparing `tmp/octostar_streamlit-0.1.0.tar.gz` & `tmp/octostar_streamlit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octostar_streamlit-0.1.0.tar", max compression
+gzip compressed data, was "octostar_streamlit-0.1.1.tar", max compression
```

## Comparing `octostar_streamlit-0.1.0.tar` & `octostar_streamlit-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1074 2024-04-02 18:14:40.684041 octostar_streamlit-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-03-25 19:08:06.934741 octostar_streamlit-0.1.0/README.md
--rw-r--r--   0        0        0     1884 2024-03-30 16:14:41.571754 octostar_streamlit-0.1.0/octostar_streamlit/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 04:35:51.197030 octostar_streamlit-0.1.0/octostar_streamlit/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 23:54:12.923655 octostar_streamlit-0.1.0/octostar_streamlit/core/desktop/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-02 17:34:25.798855 octostar_streamlit-0.1.0/octostar_streamlit/core/desktop/method_call.py
--rw-r--r--   0        0        0     7821 2024-04-02 02:39:47.115763 octostar_streamlit-0.1.0/octostar_streamlit/core/desktop/params.py
--rw-r--r--   0        0        0     6134 2024-04-02 18:05:04.513723 octostar_streamlit-0.1.0/octostar_streamlit/core/entities.py
--rw-r--r--   0        0        0      281 2024-03-29 12:03:54.758291 octostar_streamlit-0.1.0/octostar_streamlit/core/method_call.py
--rw-r--r--   0        0        0        0 2024-04-02 02:26:19.429098 octostar_streamlit-0.1.0/octostar_streamlit/core/ontology/__init__.py
--rw-r--r--   0        0        0      673 2024-04-02 02:22:12.070850 octostar_streamlit-0.1.0/octostar_streamlit/core/ontology/method_call.py
--rw-r--r--   0        0        0     1766 2024-04-02 14:53:22.124258 octostar_streamlit-0.1.0/octostar_streamlit/core/ontology/params.py
--rw-r--r--   0        0        0      222 2024-03-29 12:14:25.228859 octostar_streamlit-0.1.0/octostar_streamlit/core/params_base_model.py
--rw-r--r--   0        0        0      867 2024-03-29 13:11:44.695472 octostar_streamlit-0.1.0/octostar_streamlit/core/streamlit_executor.py
--rw-r--r--   0        0        0    10049 2024-04-02 17:49:27.980323 octostar_streamlit-0.1.0/octostar_streamlit/desktop.py
--rw-r--r--   0        0        0      253 2024-03-26 04:20:07.701188 octostar_streamlit-0.1.0/octostar_streamlit/frontend/.gitignore
--rw-r--r--   0        0        0      357 2024-03-26 04:25:43.681269 octostar_streamlit-0.1.0/octostar_streamlit/frontend/index.html
--rw-r--r--   0        0        0    42450 2024-03-28 02:05:13.964715 octostar_streamlit-0.1.0/octostar_streamlit/frontend/package-lock.json
--rw-r--r--   0        0        0      413 2024-03-28 02:05:13.918146 octostar_streamlit-0.1.0/octostar_streamlit/frontend/package.json
--rw-r--r--   0        0        0     1497 2024-03-26 04:20:07.701709 octostar_streamlit-0.1.0/octostar_streamlit/frontend/public/vite.svg
--rw-r--r--   0        0        0      835 2024-04-02 14:38:29.668702 octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/core.ts
--rw-r--r--   0        0        0    15318 2024-04-02 14:38:37.150593 octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/desktop.ts
--rw-r--r--   0        0        0     2373 2024-04-02 17:53:24.951272 octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/main.ts
--rw-r--r--   0        0        0     4177 2024-04-02 14:40:22.688780 octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/ontology.ts
--rw-r--r--   0        0        0       38 2024-03-26 04:20:07.702309 octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      527 2024-03-26 04:20:07.702493 octostar_streamlit-0.1.0/octostar_streamlit/frontend/tsconfig.json
--rw-r--r--   0        0        0      396 2024-03-26 04:53:16.781015 octostar_streamlit-0.1.0/octostar_streamlit/main.py
--rw-r--r--   0        0        0     3984 2024-04-02 18:07:10.934728 octostar_streamlit-0.1.0/octostar_streamlit/ontology.py
--rw-r--r--   0        0        0      661 2024-03-28 01:25:20.191290 octostar_streamlit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/README.md
+-rw-r--r--   0        0        0     1884 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/method_call.py
+-rw-r--r--   0        0        0     7821 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/params.py
+-rw-r--r--   0        0        0     6134 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/entities.py
+-rw-r--r--   0        0        0      281 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/method_call.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/method_call.py
+-rw-r--r--   0        0        0     1766 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/params.py
+-rw-r--r--   0        0        0      222 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/params_base_model.py
+-rw-r--r--   0        0        0      867 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/core/streamlit_executor.py
+-rw-r--r--   0        0        0    10049 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/desktop.py
+-rw-r--r--   0        0        0      253 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/.gitignore
+-rw-r--r--   0        0        0      357 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/index.html
+-rw-r--r--   0        0        0    42450 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/package-lock.json
+-rw-r--r--   0        0        0      413 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/package.json
+-rw-r--r--   0        0        0     1497 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/public/vite.svg
+-rw-r--r--   0        0        0      835 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/core.ts
+-rw-r--r--   0        0        0    15318 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/desktop.ts
+-rw-r--r--   0        0        0     2373 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/main.ts
+-rw-r--r--   0        0        0     4177 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/ontology.ts
+-rw-r--r--   0        0        0       38 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      527 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/frontend/tsconfig.json
+-rw-r--r--   0        0        0      396 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/main.py
+-rw-r--r--   0        0        0     3984 2024-04-03 00:01:49.224615 octostar_streamlit-0.1.1/octostar_streamlit/ontology.py
+-rw-r--r--   0        0        0      661 2024-04-03 00:01:49.228615 octostar_streamlit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.1/PKG-INFO
```

### Comparing `octostar_streamlit-0.1.0/LICENSE` & `octostar_streamlit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/__init__.py` & `octostar_streamlit-0.1.1/octostar_streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/core/desktop/method_call.py` & `octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/core/desktop/params.py` & `octostar_streamlit-0.1.1/octostar_streamlit/core/desktop/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/core/entities.py` & `octostar_streamlit-0.1.1/octostar_streamlit/core/entities.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/core/ontology/method_call.py` & `octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/core/ontology/params.py` & `octostar_streamlit-0.1.1/octostar_streamlit/core/ontology/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/core/streamlit_executor.py` & `octostar_streamlit-0.1.1/octostar_streamlit/core/streamlit_executor.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/desktop.py` & `octostar_streamlit-0.1.1/octostar_streamlit/desktop.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/frontend/package-lock.json` & `octostar_streamlit-0.1.1/octostar_streamlit/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/frontend/public/vite.svg` & `octostar_streamlit-0.1.1/octostar_streamlit/frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/core.ts` & `octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/core.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/desktop.ts` & `octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/desktop.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/main.ts` & `octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/main.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/frontend/src/ontology.ts` & `octostar_streamlit-0.1.1/octostar_streamlit/frontend/src/ontology.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/frontend/tsconfig.json` & `octostar_streamlit-0.1.1/octostar_streamlit/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/octostar_streamlit/ontology.py` & `octostar_streamlit-0.1.1/octostar_streamlit/ontology.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.0/pyproject.toml` & `octostar_streamlit-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octostar-streamlit"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Oleksandr Korzhov <another.fullstack.dev@gmail.com>"]
 readme = "README.md"
 
 [tool.mypy]
 python_version = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 check_untyped_defs = true
```

### Comparing `octostar_streamlit-0.1.0/PKG-INFO` & `octostar_streamlit-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octostar-streamlit
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Oleksandr Korzhov
 Author-email: another.fullstack.dev@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

