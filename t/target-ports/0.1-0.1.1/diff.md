# Comparing `tmp/target-ports-0.1.tar.gz` & `tmp/target-ports-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-0.1.tar", last modified: Wed Apr  3 20:28:09 2024, max compression
+gzip compressed data, was "target-ports-0.1.1.tar", last modified: Wed Apr  3 20:38:36 2024, max compression
```

## Comparing `target-ports-0.1.tar` & `target-ports-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:28:09.054819 target-ports-0.1/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-0.1/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     2630 2024-04-03 20:28:09.054333 target-ports-0.1/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)       23 2024-04-03 15:11:51.000000 target-ports-0.1/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1233 2024-04-03 17:06:55.000000 target-ports-0.1/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 20:28:09.054895 target-ports-0.1/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:28:09.038014 target-ports-0.1/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:28:09.041109 target-ports-0.1/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-0.1/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     5633 2024-04-03 20:27:18.000000 target-ports-0.1/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:28:09.053778 target-ports-0.1/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     2630 2024-04-03 20:28:09.000000 target-ports-0.1/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 20:28:09.000000 target-ports-0.1/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 20:28:09.000000 target-ports-0.1/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 20:28:09.000000 target-ports-0.1/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 20:28:09.000000 target-ports-0.1/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 20:28:09.000000 target-ports-0.1/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:38:36.378773 target-ports-0.1.1/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-0.1.1/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     2632 2024-04-03 20:38:36.378156 target-ports-0.1.1/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)       23 2024-04-03 15:11:51.000000 target-ports-0.1.1/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 20:34:58.000000 target-ports-0.1.1/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 20:38:36.378849 target-ports-0.1.1/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:38:36.361007 target-ports-0.1.1/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:38:36.364279 target-ports-0.1.1/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-0.1.1/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     5647 2024-04-03 20:36:31.000000 target-ports-0.1.1/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:38:36.377503 target-ports-0.1.1/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     2632 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/top_level.txt
```

### Comparing `target-ports-0.1/LICENSE` & `target-ports-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-0.1/PKG-INFO` & `target-ports-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 0.1
+Version: 0.1.1
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

### Comparing `target-ports-0.1/pyproject.toml` & `target-ports-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "0.1"
+version = "0.1.1"
 description = "Scan ports of a target"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
```

### Comparing `target-ports-0.1/src/target_ports/target_ports.py` & `target-ports-0.1.1/src/target_ports/target_ports.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def scanport(self, target:str, port: int):
         try:
             sock = socket(AF_INET, SOCK_STREAM)
             s = sock.connect_ex((target, port))
             if s==0:
                 print(termcolor.colored((f'[+] Port {port} is opened.'), 'green'))
             else:
-                print(f'port {port} is closed.')
+                print(f'[-] port {port} is closed.', end='\r')
             sock.close()
         except KeyboardInterrupt:
             exit(1)
         except gaierror:
             print(termcolor.colored('SCANERROR', 'red'), f' : cannot resolve {target}.')
             exit(1)
         except error:
```

### Comparing `target-ports-0.1/src/target_ports.egg-info/PKG-INFO` & `target-ports-0.1.1/src/target_ports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 0.1
+Version: 0.1.1
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

