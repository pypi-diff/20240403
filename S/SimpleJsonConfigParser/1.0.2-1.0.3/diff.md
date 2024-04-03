# Comparing `tmp/SimpleJsonConfigParser-1.0.2.tar.gz` & `tmp/SimpleJsonConfigParser-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleJsonConfigParser-1.0.2.tar", last modified: Wed Apr  3 06:21:25 2024, max compression
+gzip compressed data, was "SimpleJsonConfigParser-1.0.3.tar", last modified: Wed Apr  3 13:46:41 2024, max compression
```

## Comparing `SimpleJsonConfigParser-1.0.2.tar` & `SimpleJsonConfigParser-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.821669 SimpleJsonConfigParser-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 06:21:15.000000 SimpleJsonConfigParser-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 06:21:25.821669 SimpleJsonConfigParser-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-03 06:21:15.000000 SimpleJsonConfigParser-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.821669 SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser/
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-03 06:21:15.000000 SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser/ConfigReader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:15.000000 SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.821669 SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 06:21:25.000000 SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 06:21:25.000000 SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:21:25.000000 SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 06:21:25.000000 SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:21:25.821669 SimpleJsonConfigParser-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 06:21:15.000000 SimpleJsonConfigParser-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:46:41.887933 SimpleJsonConfigParser-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 13:46:34.000000 SimpleJsonConfigParser-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 13:46:41.887933 SimpleJsonConfigParser-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-03 13:46:34.000000 SimpleJsonConfigParser-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:46:41.887933 SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser/
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-03 13:46:34.000000 SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser/ConfigReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:46:34.000000 SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:46:41.887933 SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 13:46:41.000000 SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 13:46:41.000000 SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:46:41.000000 SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 13:46:41.000000 SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:46:41.887933 SimpleJsonConfigParser-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 13:46:34.000000 SimpleJsonConfigParser-1.0.3/setup.py
```

### Comparing `SimpleJsonConfigParser-1.0.2/LICENSE` & `SimpleJsonConfigParser-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleJsonConfigParser-1.0.2/PKG-INFO` & `SimpleJsonConfigParser-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleJsonConfigParser
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple JSON Config Parser for Python.
 Author: TPosty
 Author-email: 
 Keywords: python,configuration
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SimpleJsonConfigParser-1.0.2/README.md` & `SimpleJsonConfigParser-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser/ConfigReader.py` & `SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser/ConfigReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import json
 
-class config_reader():
+class config_parser():
 
     def __init__(self, base_directory):
         self.base_directory = base_directory
 
     def create_config(self, config_name: str, *args):
         # Config file name (what to save the file as)
         # Path - Where to save the config file
```

### Comparing `SimpleJsonConfigParser-1.0.2/SimpleJsonConfigParser.egg-info/PKG-INFO` & `SimpleJsonConfigParser-1.0.3/SimpleJsonConfigParser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleJsonConfigParser
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple JSON Config Parser for Python.
 Author: TPosty
 Author-email: 
 Keywords: python,configuration
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SimpleJsonConfigParser-1.0.2/setup.py` & `SimpleJsonConfigParser-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 path = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(path, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'Simple JSON Config Parser for Python.'
 LONG_DESCRIPTION = 'Simple JSON Config Parser for Python that allows creation, modification, and deletion of multiple JSON configuration files.'
 
 # Setting up
 setup(
     name="SimpleJsonConfigParser",
     version=VERSION,
```

