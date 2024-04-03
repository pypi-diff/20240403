# Comparing `tmp/lpb_lib-0.0.7.tar.gz` & `tmp/lpb_lib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpb_lib-0.0.7.tar", last modified: Wed Apr  3 14:09:00 2024, max compression
+gzip compressed data, was "lpb_lib-0.0.8.tar", last modified: Wed Apr  3 14:21:49 2024, max compression
```

## Comparing `lpb_lib-0.0.7.tar` & `lpb_lib-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:09:00.302574 lpb_lib-0.0.7/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      755 2024-04-03 14:09:00.302574 lpb_lib-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-04-03 14:07:09.000000 lpb_lib-0.0.7/README.md
--rw-rw-rw-   0        0        0     1207 2024-04-03 13:20:54.000000 lpb_lib-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      626 2024-04-03 14:09:00.307577 lpb_lib-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 14:09:00.258168 lpb_lib-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:09:00.284379 lpb_lib-0.0.7/src/lpb_lib/
--rw-rw-rw-   0        0        0        0 2024-04-03 14:08:10.000000 lpb_lib-0.0.7/src/lpb_lib/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-04-03 13:21:41.000000 lpb_lib-0.0.7/src/lpb_lib/big_query.py
--rw-rw-rw-   0        0        0      367 2024-04-03 13:13:33.000000 lpb_lib-0.0.7/src/lpb_lib/compute_log.py
--rw-rw-rw-   0        0        0      558 2024-04-03 14:07:38.000000 lpb_lib-0.0.7/src/lpb_lib/get_env.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:09:00.300575 lpb_lib-0.0.7/src/lpb_lib.egg-info/
--rw-rw-rw-   0        0        0      755 2024-04-03 14:08:59.000000 lpb_lib-0.0.7/src/lpb_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-03 14:08:59.000000 lpb_lib-0.0.7/src/lpb_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:08:59.000000 lpb_lib-0.0.7/src/lpb_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 14:08:59.000000 lpb_lib-0.0.7/src/lpb_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 14:21:49.470280 lpb_lib-0.0.8/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      755 2024-04-03 14:21:49.469282 lpb_lib-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-04-03 14:07:09.000000 lpb_lib-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1207 2024-04-03 13:20:54.000000 lpb_lib-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      626 2024-04-03 14:21:49.472278 lpb_lib-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 14:21:49.436004 lpb_lib-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 14:21:49.455558 lpb_lib-0.0.8/src/lpb_lib/
+-rw-rw-rw-   0        0        0        0 2024-04-03 14:08:10.000000 lpb_lib-0.0.8/src/lpb_lib/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-04-03 13:21:41.000000 lpb_lib-0.0.8/src/lpb_lib/big_query.py
+-rw-rw-rw-   0        0        0      367 2024-04-03 13:13:33.000000 lpb_lib-0.0.8/src/lpb_lib/compute_log.py
+-rw-rw-rw-   0        0        0      574 2024-04-03 14:21:06.000000 lpb_lib-0.0.8/src/lpb_lib/get_env.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:21:49.468282 lpb_lib-0.0.8/src/lpb_lib.egg-info/
+-rw-rw-rw-   0        0        0      755 2024-04-03 14:21:48.000000 lpb_lib-0.0.8/src/lpb_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-04-03 14:21:48.000000 lpb_lib-0.0.8/src/lpb_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 14:21:48.000000 lpb_lib-0.0.8/src/lpb_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 14:21:48.000000 lpb_lib-0.0.8/src/lpb_lib.egg-info/top_level.txt
```

### Comparing `lpb_lib-0.0.7/PKG-INFO` & `lpb_lib-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpb_lib
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package contains tools that will help me to develop my projects
 Home-page: https://github.com/Fajitas08090/lpb_lib
 Author: Maxime Renac
 Author-email: maxime.renac@lepetitballon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpb_lib-0.0.7/pyproject.toml` & `lpb_lib-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lpb_lib-0.0.7/setup.cfg` & `lpb_lib-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7062 5f6c 6962 0d0a 7665 7273   = lpb_lib..vers
-00000020: 696f 6e20 3d20 302e 302e 370d 0a61 7574  ion = 0.0.7..aut
+00000020: 696f 6e20 3d20 302e 302e 380d 0a61 7574  ion = 0.0.8..aut
 00000030: 686f 7220 3d20 4d61 7869 6d65 2052 656e  hor = Maxime Ren
 00000040: 6163 0d0a 6175 7468 6f72 5f65 6d61 696c  ac..author_email
 00000050: 203d 206d 6178 696d 652e 7265 6e61 6340   = maxime.renac@
 00000060: 6c65 7065 7469 7462 616c 6c6f 6e2e 636f  lepetitballon.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2054 6869 7320 7061 636b 6167 6520 636f   This package co
 00000090: 6e74 6169 6e73 2074 6f6f 6c73 2074 6861  ntains tools tha
```

### Comparing `lpb_lib-0.0.7/src/lpb_lib/big_query.py` & `lpb_lib-0.0.8/src/lpb_lib/big_query.py`

 * *Files identical despite different names*

### Comparing `lpb_lib-0.0.7/src/lpb_lib/get_env.py` & `lpb_lib-0.0.8/src/lpb_lib/get_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import lpb_lib
 
 def find_code_in_env_file(path, code_to_find):    
     """
     Find a code in the .env file and return its value.
     Args:
     :path: The path to the .env file.
     :code_to_find: The code to find in the .env file.
```

### Comparing `lpb_lib-0.0.7/src/lpb_lib.egg-info/PKG-INFO` & `lpb_lib-0.0.8/src/lpb_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpb_lib
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package contains tools that will help me to develop my projects
 Home-page: https://github.com/Fajitas08090/lpb_lib
 Author: Maxime Renac
 Author-email: maxime.renac@lepetitballon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

