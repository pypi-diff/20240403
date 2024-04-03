# Comparing `tmp/html_elements-0.1.2.tar.gz` & `tmp/html_elements-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_elements-0.1.2.tar", max compression
+gzip compressed data, was "html_elements-0.1.3.tar", max compression
```

## Comparing `html_elements-0.1.2.tar` & `html_elements-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1076 2024-03-22 09:26:50.620238 html_elements-0.1.2/LICENSE
--rw-r--r--   0        0        0     1555 2024-03-22 09:23:20.750337 html_elements-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-02-14 14:26:35.458394 html_elements-0.1.2/html_elements/__init__.py
--rw-r--r--   0        0        0    10911 2024-03-21 15:02:34.794790 html_elements-0.1.2/html_elements/base.py
--rw-r--r--   0        0        0    34820 2024-03-22 09:06:32.947390 html_elements-0.1.2/html_elements/elements.py
--rw-r--r--   0        0        0     4159 2024-03-01 08:37:04.759557 html_elements-0.1.2/html_elements/extensions.py
--rw-r--r--   0        0        0      941 2024-03-22 09:28:22.861180 html_elements-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 html_elements-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-22 09:26:50.620238 html_elements-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1555 2024-03-22 09:23:20.750337 html_elements-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-02-14 14:26:35.458394 html_elements-0.1.3/html_elements/__init__.py
+-rw-r--r--   0        0        0    10911 2024-03-21 15:02:34.794790 html_elements-0.1.3/html_elements/base.py
+-rw-r--r--   0        0        0    34820 2024-03-22 09:06:32.947390 html_elements-0.1.3/html_elements/elements.py
+-rw-r--r--   0        0        0     4159 2024-03-01 08:37:04.759557 html_elements-0.1.3/html_elements/extensions.py
+-rw-r--r--   0        0        0        0 2024-04-03 17:56:10.211171 html_elements-0.1.3/html_elements/py.typed
+-rw-r--r--   0        0        0      941 2024-04-03 17:56:17.737567 html_elements-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 html_elements-0.1.3/PKG-INFO
```

### Comparing `html_elements-0.1.2/LICENSE` & `html_elements-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.2/README.md` & `html_elements-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.2/html_elements/base.py` & `html_elements-0.1.3/html_elements/base.py`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.2/html_elements/elements.py` & `html_elements-0.1.3/html_elements/elements.py`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.2/html_elements/extensions.py` & `html_elements-0.1.3/html_elements/extensions.py`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.2/pyproject.toml` & `html_elements-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "html-elements"
-version = "0.1.2"
+version = "0.1.3"
 description = "HTML element objects to use in pure Python server side rendering"
 authors = ["Anton De Meester <antondemeester@gmail.com>"]
 readme = "README.md"
 packages = [{include = "html_elements"}]
 license = "MIT"
 
 [project.urls]
```

### Comparing `html_elements-0.1.2/PKG-INFO` & `html_elements-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-elements
-Version: 0.1.2
+Version: 0.1.3
 Summary: HTML element objects to use in pure Python server side rendering
 License: MIT
 Author: Anton De Meester
 Author-email: antondemeester@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

