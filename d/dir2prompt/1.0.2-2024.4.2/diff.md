# Comparing `tmp/dir2prompt-1.0.2.tar.gz` & `tmp/dir2prompt-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir2prompt-1.0.2.tar", last modified: Wed Apr  3 04:04:04 2024, max compression
+gzip compressed data, was "dir2prompt-2024.4.2.tar", last modified: Wed Apr  3 03:59:06 2024, max compression
```

## Comparing `dir2prompt-1.0.2.tar` & `dir2prompt-2024.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 04:04:04.666605 dir2prompt-1.0.2/
--rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.2/LICENSE
--rw-r--r--   0 mkieffer   (501) staff       (20)     6030 2024-04-03 04:04:04.666422 dir2prompt-1.0.2/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)     3752 2024-04-03 03:32:38.000000 dir2prompt-1.0.2/README.md
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 04:04:04.666194 dir2prompt-1.0.2/dir2prompt.egg-info/
--rw-r--r--   0 mkieffer   (501) staff       (20)     6030 2024-04-03 04:04:04.000000 dir2prompt-1.0.2/dir2prompt.egg-info/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)      257 2024-04-03 04:04:04.000000 dir2prompt-1.0.2/dir2prompt.egg-info/SOURCES.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-03 04:04:04.000000 dir2prompt-1.0.2/dir2prompt.egg-info/dependency_links.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)       37 2024-04-03 04:04:04.000000 dir2prompt-1.0.2/dir2prompt.egg-info/entry_points.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        4 2024-04-03 04:04:04.000000 dir2prompt-1.0.2/dir2prompt.egg-info/top_level.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)     1217 2024-04-03 04:02:12.000000 dir2prompt-1.0.2/pyproject.toml
--rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-03 04:04:04.666642 dir2prompt-1.0.2/setup.cfg
--rw-r--r--   0 mkieffer   (501) staff       (20)     1346 2024-04-03 03:21:38.000000 dir2prompt-1.0.2/setup.py
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 04:04:04.665993 dir2prompt-1.0.2/src/
--rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-02 07:15:41.000000 dir2prompt-1.0.2/src/__init__.py
--rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-1.0.2/src/config.json
--rw-r--r--   0 mkieffer   (501) staff       (20)     7390 2024-04-03 03:29:17.000000 dir2prompt-1.0.2/src/d2p.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 03:59:06.946035 dir2prompt-2024.4.2/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-2024.4.2/LICENSE
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6033 2024-04-03 03:59:06.945811 dir2prompt-2024.4.2/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)     3752 2024-04-03 03:32:38.000000 dir2prompt-2024.4.2/README.md
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 03:59:06.945541 dir2prompt-2024.4.2/dir2prompt.egg-info/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6033 2024-04-03 03:59:06.000000 dir2prompt-2024.4.2/dir2prompt.egg-info/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)      257 2024-04-03 03:59:06.000000 dir2prompt-2024.4.2/dir2prompt.egg-info/SOURCES.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-03 03:59:06.000000 dir2prompt-2024.4.2/dir2prompt.egg-info/dependency_links.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)       37 2024-04-03 03:59:06.000000 dir2prompt-2024.4.2/dir2prompt.egg-info/entry_points.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)        4 2024-04-03 03:59:06.000000 dir2prompt-2024.4.2/dir2prompt.egg-info/top_level.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1220 2024-04-03 03:58:48.000000 dir2prompt-2024.4.2/pyproject.toml
+-rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-03 03:59:06.946074 dir2prompt-2024.4.2/setup.cfg
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1346 2024-04-03 03:21:38.000000 dir2prompt-2024.4.2/setup.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 03:59:06.945310 dir2prompt-2024.4.2/src/
+-rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-02 07:15:41.000000 dir2prompt-2024.4.2/src/__init__.py
+-rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-2024.4.2/src/config.json
+-rw-r--r--   0 mkieffer   (501) staff       (20)     7390 2024-04-03 03:29:17.000000 dir2prompt-2024.4.2/src/d2p.py
```

### Comparing `dir2prompt-1.0.2/LICENSE` & `dir2prompt-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.2/PKG-INFO` & `dir2prompt-2024.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.2
+Version: 2024.4.2
 Summary: A tool to generate prompts from directory contents
 Home-page: https://github.com/mkieffer1107/dir2prompt
 Author: Max Kieffer
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
```

### Comparing `dir2prompt-1.0.2/README.md` & `dir2prompt-2024.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.2/dir2prompt.egg-info/PKG-INFO` & `dir2prompt-2024.4.2/dir2prompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.2
+Version: 2024.4.2
 Summary: A tool to generate prompts from directory contents
 Home-page: https://github.com/mkieffer1107/dir2prompt
 Author: Max Kieffer
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
```

### Comparing `dir2prompt-1.0.2/pyproject.toml` & `dir2prompt-2024.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dir2prompt"
-version = "1.0.2"
+version = "2024.4.2"
 license = {file = "LICENSE"}
 authors = [
   { name="Max Kieffer", email="wkieffer@ufl.edu" },
 ]
 description = "A tool to generate prompts from directory contents"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `dir2prompt-1.0.2/setup.py` & `dir2prompt-2024.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.2/src/config.json` & `dir2prompt-2024.4.2/src/config.json`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.2/src/d2p.py` & `dir2prompt-2024.4.2/src/d2p.py`

 * *Files identical despite different names*

