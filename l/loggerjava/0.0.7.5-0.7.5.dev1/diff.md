# Comparing `tmp/loggerjava-0.0.7.5.tar.gz` & `tmp/loggerjava-0.7.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerjava-0.0.7.5.tar", last modified: Wed Apr  3 14:51:41 2024, max compression
+gzip compressed data, was "loggerjava-0.7.5.dev1.tar", last modified: Wed Apr  3 15:11:40 2024, max compression
```

## Comparing `loggerjava-0.0.7.5.tar` & `loggerjava-0.7.5.dev1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:41.576277 loggerjava-0.0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-03 14:51:41.576277 loggerjava-0.0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:41.572276 loggerjava-0.0.7.5/loggerjava/
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/loggerjava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/loggerjava/loggerjava.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/loggerjava/test_loggerjava.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:41.576277 loggerjava-0.0.7.5/loggerjava.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-03 14:51:41.000000 loggerjava-0.0.7.5/loggerjava.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 14:51:41.000000 loggerjava-0.0.7.5/loggerjava.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:51:41.000000 loggerjava-0.0.7.5/loggerjava.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 14:51:41.000000 loggerjava-0.0.7.5/loggerjava.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:51:41.576277 loggerjava-0.0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/loggerjava/
+-rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/loggerjava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/loggerjava/loggerjava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/loggerjava/test_loggerjava.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/loggerjava.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-03 15:11:40.000000 loggerjava-0.7.5.dev1/loggerjava.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 15:11:40.000000 loggerjava-0.7.5.dev1/loggerjava.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:11:40.000000 loggerjava-0.7.5.dev1/loggerjava.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 15:11:40.000000 loggerjava-0.7.5.dev1/loggerjava.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/setup.py
```

### Comparing `loggerjava-0.0.7.5/LICENSE` & `loggerjava-0.7.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerjava-0.0.7.5/PKG-INFO` & `loggerjava-0.7.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.0.7.5
+Version: 0.7.5.dev1
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -73,14 +73,16 @@
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.7.5.dev1` follow SemVer, no actual updates
+
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
```

### Comparing `loggerjava-0.0.7.5/README.md` & `loggerjava-0.7.5.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.7.5.dev1` follow SemVer, no actual updates
+
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
```

### Comparing `loggerjava-0.0.7.5/loggerjava/__init__.py` & `loggerjava-0.7.5.dev1/loggerjava/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 import loggerjava
 
 if __name__ == '__main__':
     pass
 
-ver = "v0.0.7.5"
+ver = "v0.7.5.dev1"
 name = "log"
 absolutepath = False
 showdetailedtime = False
 showinconsole = True
 filetype = ".log"
 file_encoding = "utf-8"
 route = r"log.log"
```

### Comparing `loggerjava-0.0.7.5/loggerjava/loggerjava.py` & `loggerjava-0.7.5.dev1/loggerjava/loggerjava.py`

 * *Files identical despite different names*

### Comparing `loggerjava-0.0.7.5/loggerjava/test_loggerjava.py` & `loggerjava-0.7.5.dev1/loggerjava/test_loggerjava.py`

 * *Files identical despite different names*

### Comparing `loggerjava-0.0.7.5/loggerjava.egg-info/PKG-INFO` & `loggerjava-0.7.5.dev1/loggerjava.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.0.7.5
+Version: 0.7.5.dev1
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -73,14 +73,16 @@
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.7.5.dev1` follow SemVer, no actual updates
+
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
```

### Comparing `loggerjava-0.0.7.5/setup.py` & `loggerjava-0.7.5.dev1/setup.py`

 * *Files identical despite different names*

