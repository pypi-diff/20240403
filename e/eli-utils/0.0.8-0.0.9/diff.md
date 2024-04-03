# Comparing `tmp/eli_utils-0.0.8.tar.gz` & `tmp/eli_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eli_utils-0.0.8.tar", last modified: Mon Jan 22 12:11:07 2024, max compression
+gzip compressed data, was "eli_utils-0.0.9.tar", last modified: Wed Feb 14 16:09:19 2024, max compression
```

## Comparing `eli_utils-0.0.8.tar` & `eli_utils-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eli       (1000) eli       (1000)        0 2024-01-22 12:11:07.423244 eli_utils-0.0.8/
--rw-r--r--   0 eli       (1000) eli       (1000)     1069 2023-11-25 09:05:04.000000 eli_utils-0.0.8/LICENSE
--rw-r--r--   0 eli       (1000) eli       (1000)     1617 2024-01-22 12:11:07.423244 eli_utils-0.0.8/PKG-INFO
--rw-r--r--   0 eli       (1000) eli       (1000)      826 2023-11-25 09:05:04.000000 eli_utils-0.0.8/README.md
-drwxr-xr-x   0 eli       (1000) eli       (1000)        0 2024-01-22 12:11:07.423244 eli_utils-0.0.8/eli_utils/
--rw-r--r--   0 eli       (1000) eli       (1000)      269 2024-01-18 11:06:37.000000 eli_utils-0.0.8/eli_utils/__init__.py
--rw-r--r--   0 eli       (1000) eli       (1000)     1437 2023-11-25 09:12:16.000000 eli_utils-0.0.8/eli_utils/_modidx.py
--rw-r--r--   0 eli       (1000) eli       (1000)      784 2024-01-22 12:10:31.000000 eli_utils-0.0.8/eli_utils/image.py
--rw-r--r--   0 eli       (1000) eli       (1000)     1061 2024-01-18 11:24:35.000000 eli_utils-0.0.8/eli_utils/io.py
--rw-r--r--   0 eli       (1000) eli       (1000)     1241 2023-11-25 09:12:16.000000 eli_utils-0.0.8/eli_utils/plotting.py
--rw-r--r--   0 eli       (1000) eli       (1000)     1694 2023-11-25 09:12:16.000000 eli_utils-0.0.8/eli_utils/video.py
-drwxr-xr-x   0 eli       (1000) eli       (1000)        0 2024-01-22 12:11:07.423244 eli_utils-0.0.8/eli_utils.egg-info/
--rw-r--r--   0 eli       (1000) eli       (1000)     1617 2024-01-22 12:11:07.000000 eli_utils-0.0.8/eli_utils.egg-info/PKG-INFO
--rw-r--r--   0 eli       (1000) eli       (1000)      377 2024-01-22 12:11:07.000000 eli_utils-0.0.8/eli_utils.egg-info/SOURCES.txt
--rw-r--r--   0 eli       (1000) eli       (1000)        1 2024-01-22 12:11:07.000000 eli_utils-0.0.8/eli_utils.egg-info/dependency_links.txt
--rw-r--r--   0 eli       (1000) eli       (1000)       61 2024-01-22 12:11:07.000000 eli_utils-0.0.8/eli_utils.egg-info/entry_points.txt
--rw-r--r--   0 eli       (1000) eli       (1000)        1 2023-11-25 09:05:28.000000 eli_utils-0.0.8/eli_utils.egg-info/not-zip-safe
--rw-r--r--   0 eli       (1000) eli       (1000)       45 2024-01-22 12:11:07.000000 eli_utils-0.0.8/eli_utils.egg-info/requires.txt
--rw-r--r--   0 eli       (1000) eli       (1000)       10 2024-01-22 12:11:07.000000 eli_utils-0.0.8/eli_utils.egg-info/top_level.txt
--rw-r--r--   0 eli       (1000) eli       (1000)       38 2024-01-22 12:11:07.423244 eli_utils-0.0.8/setup.cfg
--rw-r--r--   0 eli       (1000) eli       (1000)     2596 2023-11-25 09:05:04.000000 eli_utils-0.0.8/setup.py
+drwxr-xr-x   0 eli       (1000) eli       (1000)        0 2024-02-14 16:09:19.668836 eli_utils-0.0.9/
+-rw-r--r--   0 eli       (1000) eli       (1000)     1069 2023-11-25 09:05:04.000000 eli_utils-0.0.9/LICENSE
+-rw-r--r--   0 eli       (1000) eli       (1000)     1617 2024-02-14 16:09:19.668836 eli_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 eli       (1000) eli       (1000)      826 2023-11-25 09:05:04.000000 eli_utils-0.0.9/README.md
+drwxr-xr-x   0 eli       (1000) eli       (1000)        0 2024-02-14 16:09:19.668836 eli_utils-0.0.9/eli_utils/
+-rw-r--r--   0 eli       (1000) eli       (1000)      269 2024-01-18 11:06:37.000000 eli_utils-0.0.9/eli_utils/__init__.py
+-rw-r--r--   0 eli       (1000) eli       (1000)     1437 2023-11-25 09:12:16.000000 eli_utils-0.0.9/eli_utils/_modidx.py
+-rw-r--r--   0 eli       (1000) eli       (1000)      784 2024-01-22 12:10:31.000000 eli_utils-0.0.9/eli_utils/image.py
+-rw-r--r--   0 eli       (1000) eli       (1000)     1133 2024-02-14 16:07:02.000000 eli_utils-0.0.9/eli_utils/io.py
+-rw-r--r--   0 eli       (1000) eli       (1000)     1241 2023-11-25 09:12:16.000000 eli_utils-0.0.9/eli_utils/plotting.py
+-rw-r--r--   0 eli       (1000) eli       (1000)     1694 2023-11-25 09:12:16.000000 eli_utils-0.0.9/eli_utils/video.py
+drwxr-xr-x   0 eli       (1000) eli       (1000)        0 2024-02-14 16:09:19.668836 eli_utils-0.0.9/eli_utils.egg-info/
+-rw-r--r--   0 eli       (1000) eli       (1000)     1617 2024-02-14 16:09:19.000000 eli_utils-0.0.9/eli_utils.egg-info/PKG-INFO
+-rw-r--r--   0 eli       (1000) eli       (1000)      377 2024-02-14 16:09:19.000000 eli_utils-0.0.9/eli_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 eli       (1000) eli       (1000)        1 2024-02-14 16:09:19.000000 eli_utils-0.0.9/eli_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 eli       (1000) eli       (1000)       61 2024-02-14 16:09:19.000000 eli_utils-0.0.9/eli_utils.egg-info/entry_points.txt
+-rw-r--r--   0 eli       (1000) eli       (1000)        1 2023-11-25 09:05:28.000000 eli_utils-0.0.9/eli_utils.egg-info/not-zip-safe
+-rw-r--r--   0 eli       (1000) eli       (1000)       45 2024-02-14 16:09:19.000000 eli_utils-0.0.9/eli_utils.egg-info/requires.txt
+-rw-r--r--   0 eli       (1000) eli       (1000)       10 2024-02-14 16:09:19.000000 eli_utils-0.0.9/eli_utils.egg-info/top_level.txt
+-rw-r--r--   0 eli       (1000) eli       (1000)       38 2024-02-14 16:09:19.668836 eli_utils-0.0.9/setup.cfg
+-rw-r--r--   0 eli       (1000) eli       (1000)     2596 2023-11-25 09:05:04.000000 eli_utils-0.0.9/setup.py
```

### Comparing `eli_utils-0.0.8/LICENSE` & `eli_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eli_utils-0.0.8/PKG-INFO` & `eli_utils-0.0.9/eli_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eli_utils
-Version: 0.0.8
+Name: eli-utils
+Version: 0.0.9
 Summary: Useful utilities I re-use in multiple projects
 Home-page: https://github.com/elifriedman/eli_utils
 Author: Eli Friedman
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `eli_utils-0.0.8/README.md` & `eli_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `eli_utils-0.0.8/eli_utils/_modidx.py` & `eli_utils-0.0.9/eli_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `eli_utils-0.0.8/eli_utils/image.py` & `eli_utils-0.0.9/eli_utils/image.py`

 * *Files identical despite different names*

### Comparing `eli_utils-0.0.8/eli_utils/plotting.py` & `eli_utils-0.0.9/eli_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `eli_utils-0.0.8/eli_utils/video.py` & `eli_utils-0.0.9/eli_utils/video.py`

 * *Files identical despite different names*

### Comparing `eli_utils-0.0.8/eli_utils.egg-info/PKG-INFO` & `eli_utils-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eli-utils
-Version: 0.0.8
+Name: eli_utils
+Version: 0.0.9
 Summary: Useful utilities I re-use in multiple projects
 Home-page: https://github.com/elifriedman/eli_utils
 Author: Eli Friedman
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `eli_utils-0.0.8/setup.py` & `eli_utils-0.0.9/setup.py`

 * *Files identical despite different names*

