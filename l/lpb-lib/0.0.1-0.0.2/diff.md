# Comparing `tmp/lpb_lib-0.0.1.tar.gz` & `tmp/lpb_lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpb_lib-0.0.1.tar", last modified: Wed Apr  3 10:33:44 2024, max compression
+gzip compressed data, was "lpb_lib-0.0.2.tar", last modified: Wed Apr  3 10:41:05 2024, max compression
```

## Comparing `lpb_lib-0.0.1.tar` & `lpb_lib-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:33:44.143175 lpb_lib-0.0.1/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      564 2024-04-03 10:33:44.139174 lpb_lib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-03 09:45:26.000000 lpb_lib-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2024-04-03 09:50:41.000000 lpb_lib-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      614 2024-04-03 10:33:44.148236 lpb_lib-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 10:33:44.062992 lpb_lib-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 10:33:44.081985 lpb_lib-0.0.1/src/lib/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:52:21.000000 lpb_lib-0.0.1/src/lib/__init__.py
--rw-rw-rw-   0        0        0       22 2024-04-03 09:57:22.000000 lpb_lib-0.0.1/src/lib/big_query.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:33:44.134116 lpb_lib-0.0.1/src/lpb_lib.egg-info/
--rw-rw-rw-   0        0        0      564 2024-04-03 10:33:43.000000 lpb_lib-0.0.1/src/lpb_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-04-03 10:33:44.000000 lpb_lib-0.0.1/src/lpb_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:33:43.000000 lpb_lib-0.0.1/src/lpb_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-03 10:33:43.000000 lpb_lib-0.0.1/src/lpb_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 10:41:05.338519 lpb_lib-0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      564 2024-04-03 10:41:05.337520 lpb_lib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-04-03 09:45:26.000000 lpb_lib-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-03 09:50:41.000000 lpb_lib-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      614 2024-04-03 10:41:05.343518 lpb_lib-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 10:41:05.260620 lpb_lib-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 10:41:05.291058 lpb_lib-0.0.2/src/lpb_lib/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:52:21.000000 lpb_lib-0.0.2/src/lpb_lib/__init__.py
+-rw-rw-rw-   0        0        0       22 2024-04-03 09:57:22.000000 lpb_lib-0.0.2/src/lpb_lib/big_query.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:41:05.334519 lpb_lib-0.0.2/src/lpb_lib.egg-info/
+-rw-rw-rw-   0        0        0      564 2024-04-03 10:41:05.000000 lpb_lib-0.0.2/src/lpb_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-04-03 10:41:05.000000 lpb_lib-0.0.2/src/lpb_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 10:41:05.000000 lpb_lib-0.0.2/src/lpb_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 10:41:05.000000 lpb_lib-0.0.2/src/lpb_lib.egg-info/top_level.txt
```

### Comparing `lpb_lib-0.0.1/PKG-INFO` & `lpb_lib-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpb_lib
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package contains tools that will help me to develop my projects
 Home-page: https://github.com/Fajitas08090/lpb_lib
 Author: fajitas30
 Author-email: maxime.renac@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpb_lib-0.0.1/setup.cfg` & `lpb_lib-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7062 5f6c 6962 0d0a 7665 7273   = lpb_lib..vers
-00000020: 696f 6e20 3d20 302e 302e 310d 0a61 7574  ion = 0.0.1..aut
+00000020: 696f 6e20 3d20 302e 302e 320d 0a61 7574  ion = 0.0.2..aut
 00000030: 686f 7220 3d20 6661 6a69 7461 7333 300d  hor = fajitas30.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6d61 7869 6d65 2e72 656e 6163 4067 6d61  maxime.renac@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5468 6973 2070 6163 6b61  ion = This packa
 00000080: 6765 2063 6f6e 7461 696e 7320 746f 6f6c  ge contains tool
 00000090: 7320 7468 6174 2077 696c 6c20 6865 6c70  s that will help
```

### Comparing `lpb_lib-0.0.1/src/lpb_lib.egg-info/PKG-INFO` & `lpb_lib-0.0.2/src/lpb_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpb_lib
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package contains tools that will help me to develop my projects
 Home-page: https://github.com/Fajitas08090/lpb_lib
 Author: fajitas30
 Author-email: maxime.renac@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

