# Comparing `tmp/target-ports-1.0.1.tar.gz` & `tmp/target-ports-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-1.0.1.tar", last modified: Wed Apr  3 21:27:53 2024, max compression
+gzip compressed data, was "target-ports-1.0.2.tar", last modified: Wed Apr  3 21:39:51 2024, max compression
```

## Comparing `target-ports-1.0.1.tar` & `target-ports-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:27:53.597784 target-ports-1.0.1/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.1/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 21:27:53.597261 target-ports-1.0.1/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 21:12:11.000000 target-ports-1.0.1/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 21:17:01.000000 target-ports-1.0.1/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 21:27:53.597863 target-ports-1.0.1/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:27:53.586824 target-ports-1.0.1/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:27:53.589955 target-ports-1.0.1/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.1/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     5655 2024-04-03 21:16:31.000000 target-ports-1.0.1/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:27:53.596678 target-ports-1.0.1/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 21:27:53.000000 target-ports-1.0.1/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:39:51.634468 target-ports-1.0.2/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.2/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 21:39:51.632887 target-ports-1.0.2/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 21:12:11.000000 target-ports-1.0.2/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 21:31:06.000000 target-ports-1.0.2/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 21:39:51.634671 target-ports-1.0.2/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:39:51.615620 target-ports-1.0.2/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:39:51.619115 target-ports-1.0.2/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.2/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     5727 2024-04-03 21:38:56.000000 target-ports-1.0.2/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:39:51.631574 target-ports-1.0.2/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 21:39:51.000000 target-ports-1.0.2/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 21:39:51.000000 target-ports-1.0.2/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 21:39:51.000000 target-ports-1.0.2/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 21:39:51.000000 target-ports-1.0.2/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 21:39:51.000000 target-ports-1.0.2/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 21:39:51.000000 target-ports-1.0.2/src/target_ports.egg-info/top_level.txt
```

### Comparing `target-ports-1.0.1/LICENSE` & `target-ports-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.1/PKG-INFO` & `target-ports-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

### Comparing `target-ports-1.0.1/README.md` & `target-ports-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.1/pyproject.toml` & `target-ports-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "1.0.1"
+version = "1.0.2"
 description = "Scan ports of a target"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
```

### Comparing `target-ports-1.0.1/src/target_ports/target_ports.py` & `target-ports-1.0.2/src/target_ports/target_ports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 __version__ = '0.1'
 
 from socket import socket, AF_INET, SOCK_STREAM, gaierror, error
-from platform import system as operatingSystem
 from optioner import options
 from sys import argv
 from re import match
 import termcolor
 
 class _scan_ports_:
     def __init__(self, targets:str | list[str], nports: int = 65535):
@@ -19,20 +18,22 @@
             nports (int, optional): Number of ports to scan. Defaults to 65535.
         """
         # call scan according to targets
         
         if type(targets)==str:
             self.scan(targets, nports)
         elif type(targets)==list[str]:
-            print(termcolor.colored((f'-- Multiple Targets Detected.'), 'blue'))
+            print(termcolor.colored((f'|-- Multiple Targets Detected.'), 'blue'))
             for target in targets:
                 self.scan(target, nports)
+        
+        print(termcolor.colored('target-ports', 'blue'), termcolor.colored(f'v{__version__}', 'red'), 'Jumpstart')
     
     def scan(self, target:str, ports: int):
-        print(termcolor.colored((f'\n-- Starting scan for {target}.'), 'light_red'))
+        print('|-- Starting scan for', termcolor.colored(f'{target}.', 'red'))
         for port in range(1, ports+1):
             self.scanport(target, port)
     
     def scanport(self, target:str, port: int):
         try:
             sock = socket(AF_INET, SOCK_STREAM)
             s = sock.connect_ex((target, port))
```

### Comparing `target-ports-1.0.1/src/target_ports.egg-info/PKG-INFO` & `target-ports-1.0.2/src/target_ports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

