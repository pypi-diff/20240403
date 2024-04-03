# Comparing `tmp/SimpleJsonConfigParser-1.0.0.tar.gz` & `tmp/SimpleJsonConfigParser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleJsonConfigParser-1.0.0.tar", last modified: Wed Apr  3 05:35:30 2024, max compression
+gzip compressed data, was "SimpleJsonConfigParser-1.0.1.tar", last modified: Wed Apr  3 05:40:36 2024, max compression
```

## Comparing `SimpleJsonConfigParser-1.0.0.tar` & `SimpleJsonConfigParser-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser/
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser/ConfigReader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 05:35:30.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 05:35:30.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:35:30.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 05:35:30.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:40:36.971388 SimpleJsonConfigParser-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 05:40:33.000000 SimpleJsonConfigParser-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 05:40:36.971388 SimpleJsonConfigParser-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 05:40:33.000000 SimpleJsonConfigParser-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:40:36.967388 SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser/
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-03 05:40:33.000000 SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser/ConfigReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:40:33.000000 SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:40:36.967388 SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 05:40:36.000000 SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 05:40:36.000000 SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:40:36.000000 SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 05:40:36.000000 SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:40:36.971388 SimpleJsonConfigParser-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 05:40:33.000000 SimpleJsonConfigParser-1.0.1/setup.py
```

### Comparing `SimpleJsonConfigParser-1.0.0/LICENSE` & `SimpleJsonConfigParser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleJsonConfigParser-1.0.0/PKG-INFO` & `SimpleJsonConfigParser-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleJsonConfigParser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple JSON Config Parser for Python.
 Author: TPosty
 Author-email: 
 Keywords: python,configuration
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser/ConfigReader.py` & `SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser/ConfigReader.py`

 * *Files identical despite different names*

### Comparing `SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/PKG-INFO` & `SimpleJsonConfigParser-1.0.1/SimpleJsonConfigParser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleJsonConfigParser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple JSON Config Parser for Python.
 Author: TPosty
 Author-email: 
 Keywords: python,configuration
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SimpleJsonConfigParser-1.0.0/setup.py` & `SimpleJsonConfigParser-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 path = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(path, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Simple JSON Config Parser for Python.'
 LONG_DESCRIPTION = 'Simple JSON Config Parser for Python that allows creation, modification, and deletion of multiple JSON configuration files.'
 
 # Setting up
 setup(
     name="SimpleJsonConfigParser",
     version=VERSION,
```

