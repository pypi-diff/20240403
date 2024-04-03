# Comparing `tmp/target-ports-1.0.tar.gz` & `tmp/target-ports-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-1.0.tar", last modified: Wed Apr  3 21:13:03 2024, max compression
+gzip compressed data, was "target-ports-1.0.1.tar", last modified: Wed Apr  3 21:27:53 2024, max compression
```

## Comparing `target-ports-1.0.tar` & `target-ports-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:13:03.388322 target-ports-1.0/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     4419 2024-04-03 21:13:03.387951 target-ports-1.0/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 21:12:11.000000 target-ports-1.0/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1233 2024-04-03 20:42:57.000000 target-ports-1.0/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 21:13:03.388404 target-ports-1.0/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:13:03.381716 target-ports-1.0/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:13:03.384143 target-ports-1.0/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     5653 2024-04-03 20:42:48.000000 target-ports-1.0/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:13:03.387604 target-ports-1.0/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     4419 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:27:53.597784 target-ports-1.0.1/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.1/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 21:27:53.597261 target-ports-1.0.1/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 21:12:11.000000 target-ports-1.0.1/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 21:17:01.000000 target-ports-1.0.1/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 21:27:53.597863 target-ports-1.0.1/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:27:53.586824 target-ports-1.0.1/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:27:53.589955 target-ports-1.0.1/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.1/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     5655 2024-04-03 21:16:31.000000 target-ports-1.0.1/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:27:53.596678 target-ports-1.0.1/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/top_level.txt
```

### Comparing `target-ports-1.0/LICENSE` & `target-ports-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-1.0/PKG-INFO` & `target-ports-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0
+Version: 1.0.1
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
-Requires-Dist: optioner>=1.4.4
+Requires-Dist: optioner>=1.4.5
 
 ![PyPI - Version](https://img.shields.io/pypi/v/target-ports)
 ![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/target-ports)
 ![Static Badge](https://img.shields.io/badge/Dependencies-optioner%3E%3D1.4.4%2C%20termcolor-purple?style=plastic&logo=python&logoColor=pink&link=https%3A%2F%2Fgithub.com%2Fd33pster%2Foptioner)
 
 
 # Overview
```

### Comparing `target-ports-1.0/README.md` & `target-ports-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `target-ports-1.0/pyproject.toml` & `target-ports-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "1.0"
+version = "1.0.1"
 description = "Scan ports of a target"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'termcolor',
-    'optioner>=1.4.4'
+    'optioner>=1.4.5'
 ]
 keywords = ['d33pster', 'port scanner', 'port', 'scanner', 'recon', 'portscanner', 'target-ports', 'targetports']
 readme = {file = "README.md", content-type = "text/markdown"}
 license = { file = "LICENSE" }
 authors = [
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"}
 ]
```

### Comparing `target-ports-1.0/src/target_ports/target_ports.py` & `target-ports-1.0.1/src/target_ports/target_ports.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     shortargs = ['h', 'v', 't', 'ts', 'p','c']
     longargs = ['help', 'version', 'target', 'targets', 'ports','current']
     
     optionctrl = options(shortargs, longargs, argv[1:], compulsory_short_args=['t'], compulsory_long_args=['target'], ignore=['-h', '--help', '-v', '--version', '-ts', '--targets', '-c', '--current'], ifthisthennotthat=[['h','help'],['v','version'], ['t','target'],['ts','targets']])
     
     args, check, error, falseargs = optionctrl._argparse()
     
-    ports = 100
+    ports = 65535
     target: str | list[str]
     current:bool = False
     
     if not check:
         print(termcolor.colored(('SCANERROR'), 'red'), f': {error}')
         exit(1)
     else:
```

### Comparing `target-ports-1.0/src/target_ports.egg-info/PKG-INFO` & `target-ports-1.0.1/src/target_ports.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0
+Version: 1.0.1
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
-Requires-Dist: optioner>=1.4.4
+Requires-Dist: optioner>=1.4.5
 
 ![PyPI - Version](https://img.shields.io/pypi/v/target-ports)
 ![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/target-ports)
 ![Static Badge](https://img.shields.io/badge/Dependencies-optioner%3E%3D1.4.4%2C%20termcolor-purple?style=plastic&logo=python&logoColor=pink&link=https%3A%2F%2Fgithub.com%2Fd33pster%2Foptioner)
 
 
 # Overview
```

