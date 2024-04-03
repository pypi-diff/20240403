# Comparing `tmp/target-ports-0.1.1.tar.gz` & `tmp/target-ports-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-0.1.1.tar", last modified: Wed Apr  3 20:38:36 2024, max compression
+gzip compressed data, was "target-ports-1.0.tar", last modified: Wed Apr  3 21:13:03 2024, max compression
```

## Comparing `target-ports-0.1.1.tar` & `target-ports-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:38:36.378773 target-ports-0.1.1/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-0.1.1/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     2632 2024-04-03 20:38:36.378156 target-ports-0.1.1/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)       23 2024-04-03 15:11:51.000000 target-ports-0.1.1/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 20:34:58.000000 target-ports-0.1.1/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 20:38:36.378849 target-ports-0.1.1/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:38:36.361007 target-ports-0.1.1/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:38:36.364279 target-ports-0.1.1/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-0.1.1/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     5647 2024-04-03 20:36:31.000000 target-ports-0.1.1/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 20:38:36.377503 target-ports-0.1.1/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     2632 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 20:38:36.000000 target-ports-0.1.1/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:13:03.388322 target-ports-1.0/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4419 2024-04-03 21:13:03.387951 target-ports-1.0/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 21:12:11.000000 target-ports-1.0/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1233 2024-04-03 20:42:57.000000 target-ports-1.0/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 21:13:03.388404 target-ports-1.0/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:13:03.381716 target-ports-1.0/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:13:03.384143 target-ports-1.0/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     5653 2024-04-03 20:42:48.000000 target-ports-1.0/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:13:03.387604 target-ports-1.0/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4419 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 21:13:03.000000 target-ports-1.0/src/target_ports.egg-info/top_level.txt
```

### Comparing `target-ports-0.1.1/LICENSE` & `target-ports-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-0.1.1/pyproject.toml` & `target-ports-1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "0.1.1"
+version = "1.0"
 description = "Scan ports of a target"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
```

### Comparing `target-ports-0.1.1/src/target_ports/target_ports.py` & `target-ports-1.0/src/target_ports/target_ports.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from platform import system as operatingSystem
 from optioner import options
 from sys import argv
 from re import match
 import termcolor
 
 class _scan_ports_:
-    def __init__(self, targets:str | list[str], nports: int = 100):
+    def __init__(self, targets:str | list[str], nports: int = 65535):
         """_scan_ports_:
         Scan ports on a target.
 
         Args:
             targets (str | list[str]): target ip
-            nports (int, optional): Number of ports to scan. Defaults to 100.
+            nports (int, optional): Number of ports to scan. Defaults to 65535.
         """
         # call scan according to targets
         
         if type(targets)==str:
             self.scan(targets, nports)
         elif type(targets)==list[str]:
             print(termcolor.colored((f'-- Multiple Targets Detected.'), 'blue'))
@@ -60,15 +60,15 @@
     print(termcolor.colored('target-ports', 'blue'), termcolor.colored(f'v{__version__}', 'red'))
     print('\nhelp text\n')
     print('  |  -h or --help      : show this help text and exit.')
     print('  |  -v or --version   : show version and exit.')
     print('  |  -c or --current   : scan localhost.')
     print('  |  -t or --target    : specify single target.')
     print('  |  -ts or --targets  : specify multiple targets.')
-    print('  |  -p or --ports     : number of ports to scan (each, if more than one target is provided.)[optional: default -> 100]')
+    print('  |  -p or --ports     : number of ports to scan (each, if more than one target is provided.)[optional: default -> 65535]')
     print(termcolor.colored('\nNote', 'red') + ':')
     print('     (i) -t(or --target) and -ts(or --targets) are mutually exclusive.')
     print('    (ii) -p(or --ports) is optional.')
     print('   (iii) This tool is just for educational pursose. The author(s) are not responsible for any misuse (AS STATED IN THE LICENSE).')
     exit(0)
 
 def main():
```

