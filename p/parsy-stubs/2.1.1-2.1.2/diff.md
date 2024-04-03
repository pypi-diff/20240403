# Comparing `tmp/parsy_stubs-2.1.1.tar.gz` & `tmp/parsy_stubs-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsy_stubs-2.1.1.tar", max compression
+gzip compressed data, was "parsy_stubs-2.1.2.tar", max compression
```

## Comparing `parsy_stubs-2.1.1.tar` & `parsy_stubs-2.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2024-04-01 23:41:19.567750 parsy_stubs-2.1.1/LICENSE
--rw-r--r--   0        0        0      460 2024-04-01 23:41:19.567750 parsy_stubs-2.1.1/README.md
--rw-r--r--   0        0        0     6006 2024-04-01 23:41:19.567750 parsy_stubs-2.1.1/parsy-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2024-04-01 23:41:19.567750 parsy_stubs-2.1.1/parsy-stubs/py.typed
--rw-r--r--   0        0        0      520 2024-04-01 23:41:19.567750 parsy_stubs-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 parsy_stubs-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-03 07:48:14.054117 parsy_stubs-2.1.2/LICENSE
+-rw-r--r--   0        0        0      479 2024-04-03 07:48:14.054117 parsy_stubs-2.1.2/README.md
+-rw-r--r--   0        0        0     6006 2024-04-03 07:48:14.054117 parsy_stubs-2.1.2/parsy-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-04-03 07:48:14.054117 parsy_stubs-2.1.2/parsy-stubs/py.typed
+-rw-r--r--   0        0        0      520 2024-04-03 07:48:14.054117 parsy_stubs-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 parsy_stubs-2.1.2/PKG-INFO
```

### Comparing `parsy_stubs-2.1.1/LICENSE` & `parsy_stubs-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parsy_stubs-2.1.1/parsy-stubs/__init__.pyi` & `parsy_stubs-2.1.2/parsy-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `parsy_stubs-2.1.1/pyproject.toml` & `parsy_stubs-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsy-stubs"
-version = "2.1.1"
+version = "2.1.2"
 description = ""
 authors = ["Basile Dura <basile@bdura.me>"]
 readme = "README.md"
 packages = [
     { include = "parsy-stubs/__init__.pyi" },
     { include = "parsy-stubs/py.typed" },
 ]
```

### Comparing `parsy_stubs-2.1.1/PKG-INFO` & `parsy_stubs-2.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsy-stubs
-Version: 2.1.1
+Version: 2.1.2
 Summary: 
 Author: Basile Dura
 Author-email: basile@bdura.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,20 +12,21 @@
 Description-Content-Type: text/markdown
 
 # Stub files for Parsy
 
 [Parsy](https://github.com/python-parsy/parsy) is an extremely elegant
 monadic parser combinator library for LL(infinity) grammars.
 
-This library aims to enhance your developer experience (as well as catching a swathe of bugs before you run any test)
+This library aims to enhance your developer experience (as well as catching a
+swathe of bugs before you run any test using static type checking with tools like Mypy)
 by providing type-hinting.
 
 ## Installation
 
 ```shell
-pip install git+https://github.com/bdura/parsy-stubs
+pip install parsy-stubs
 ```
 
 ## Disclaimer
 
 I am not affiliated in any way with the original library.
```

