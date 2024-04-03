# Comparing `tmp/deadnews_template_python-2.0.7b0.tar.gz` & `tmp/deadnews_template_python-2.0.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadnews_template_python-2.0.7b0.tar", max compression
+gzip compressed data, was "deadnews_template_python-2.0.7b1.tar", max compression
```

## Comparing `deadnews_template_python-2.0.7b0.tar` & `deadnews_template_python-2.0.7b1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-04-03 16:12:07.073014 deadnews_template_python-2.0.7b0/LICENSE
--rw-r--r--   0        0        0     1577 2024-04-03 16:12:07.073014 deadnews_template_python-2.0.7b0/README.md
--rw-r--r--   0        0        0     2938 2024-04-03 16:12:22.221023 deadnews_template_python-2.0.7b0/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-03 16:12:07.077014 deadnews_template_python-2.0.7b0/src/deadnews_template_python/__init__.py
--rw-r--r--   0        0        0      514 2024-04-03 16:12:07.077014 deadnews_template_python-2.0.7b0/src/deadnews_template_python/__main__.py
--rw-r--r--   0        0        0     1392 2024-04-03 16:12:07.077014 deadnews_template_python-2.0.7b0/src/deadnews_template_python/app.py
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 deadnews_template_python-2.0.7b0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-03 16:31:54.002567 deadnews_template_python-2.0.7b1/LICENSE
+-rw-r--r--   0        0        0     1577 2024-04-03 16:31:54.002567 deadnews_template_python-2.0.7b1/README.md
+-rw-r--r--   0        0        0     2938 2024-04-03 16:32:02.962586 deadnews_template_python-2.0.7b1/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-03 16:31:54.002567 deadnews_template_python-2.0.7b1/src/deadnews_template_python/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-03 16:31:54.002567 deadnews_template_python-2.0.7b1/src/deadnews_template_python/__main__.py
+-rw-r--r--   0        0        0     1392 2024-04-03 16:31:54.002567 deadnews_template_python-2.0.7b1/src/deadnews_template_python/app.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 deadnews_template_python-2.0.7b1/PKG-INFO
```

### Comparing `deadnews_template_python-2.0.7b0/LICENSE` & `deadnews_template_python-2.0.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.7b0/README.md` & `deadnews_template_python-2.0.7b1/README.md`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.7b0/pyproject.toml` & `deadnews_template_python-2.0.7b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "deadnews-template-python"
-version = "2.0.7-beta.0"
+version = "2.0.7-beta.1"
 description = "Python Project Template"
 authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/deadnews/deadnews-template-python"
 repository = "https://github.com/deadnews/deadnews-template-python"
 documentation = "https://deadnews.github.io/deadnews-template-python"
```

### Comparing `deadnews_template_python-2.0.7b0/src/deadnews_template_python/__main__.py` & `deadnews_template_python-2.0.7b1/src/deadnews_template_python/__main__.py`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.7b0/src/deadnews_template_python/app.py` & `deadnews_template_python-2.0.7b1/src/deadnews_template_python/app.py`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.7b0/PKG-INFO` & `deadnews_template_python-2.0.7b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadnews-template-python
-Version: 2.0.7b0
+Version: 2.0.7b1
 Summary: Python Project Template
 Home-page: https://github.com/deadnews/deadnews-template-python
 License: MIT
 Keywords: python,template,layout
 Author: DeadNews
 Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.10,<4.0
```

