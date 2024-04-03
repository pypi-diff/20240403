# Comparing `tmp/otter_service_stdalone-0.1.7.tar.gz` & `tmp/otter_service_stdalone-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service_stdalone-0.1.7.tar", last modified: Mon Sep 11 23:49:39 2023, max compression
+gzip compressed data, was "otter_service_stdalone-0.1.8.tar", last modified: Tue Sep 12 01:51:36 2023, max compression
```

## Comparing `otter_service_stdalone-0.1.7.tar` & `otter_service_stdalone-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-09-11 23:49:39.840190 otter_service_stdalone-0.1.7/
--rw-r--r--   0 sean       (501) staff       (20)     1344 2023-09-11 23:49:39.840059 otter_service_stdalone-0.1.7/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      883 2023-03-14 21:34:27.000000 otter_service_stdalone-0.1.7/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2022-12-27 21:45:58.000000 otter_service_stdalone-0.1.7/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      837 2023-09-11 23:49:39.840962 otter_service_stdalone-0.1.7/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-09-11 23:49:39.833882 otter_service_stdalone-0.1.7/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-09-11 23:49:39.837006 otter_service_stdalone-0.1.7/src/otter_service_stdalone/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-09-11 23:49:21.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     6738 2023-09-11 23:46:28.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone/app.py
--rw-r--r--   0 sean       (501) staff       (20)     1734 2023-03-14 21:34:27.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone/fs_logging.py
--rw-r--r--   0 sean       (501) staff       (20)     6024 2023-03-14 21:34:27.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone/index.html
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-09-11 23:49:39.839610 otter_service_stdalone-0.1.7/src/otter_service_stdalone.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     1344 2023-09-11 23:49:39.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      439 2023-09-11 23:49:39.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-09-11 23:49:39.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       75 2023-09-11 23:49:39.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       23 2023-09-11 23:49:39.000000 otter_service_stdalone-0.1.7/src/otter_service_stdalone.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-09-12 01:51:36.110725 otter_service_stdalone-0.1.8/
+-rw-r--r--   0 sean       (501) staff       (20)     1344 2023-09-12 01:51:36.110598 otter_service_stdalone-0.1.8/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      883 2023-03-14 21:34:27.000000 otter_service_stdalone-0.1.8/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2022-12-27 21:45:58.000000 otter_service_stdalone-0.1.8/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      837 2023-09-12 01:51:36.111582 otter_service_stdalone-0.1.8/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-09-12 01:51:36.104804 otter_service_stdalone-0.1.8/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-09-12 01:51:36.107974 otter_service_stdalone-0.1.8/src/otter_service_stdalone/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-09-12 01:51:25.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     6799 2023-09-12 01:51:05.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone/app.py
+-rw-r--r--   0 sean       (501) staff       (20)     1734 2023-03-14 21:34:27.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone/fs_logging.py
+-rw-r--r--   0 sean       (501) staff       (20)     6024 2023-03-14 21:34:27.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone/index.html
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-09-12 01:51:36.110022 otter_service_stdalone-0.1.8/src/otter_service_stdalone.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     1344 2023-09-12 01:51:36.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      439 2023-09-12 01:51:36.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-09-12 01:51:36.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       75 2023-09-12 01:51:36.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       23 2023-09-12 01:51:36.000000 otter_service_stdalone-0.1.8/src/otter_service_stdalone.egg-info/top_level.txt
```

### Comparing `otter_service_stdalone-0.1.7/PKG-INFO` & `otter_service_stdalone-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter_service_stdalone
-Version: 0.1.7
+Version: 0.1.8
 Summary: Grading Service for Instructors using Otter Grader
 Home-page: https://github.com/sean-morris/otter-service-stdalone
 Author: Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service_stdalone-0.1.7/README.md` & `otter_service_stdalone-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `otter_service_stdalone-0.1.7/setup.cfg` & `otter_service_stdalone-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service_stdalone-0.1.7/src/otter_service_stdalone/app.py` & `otter_service_stdalone-0.1.8/src/otter_service_stdalone/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 __UPLOADS__ = "/tmp/uploads"
 
 
 def copySubDirNotebooksToParentDir(parent_dir):
     for root, dirs, files in os.walk(parent_dir):
         for directory in dirs:
             print(f"Subdirectory: {os.path.join(root, directory)}")
-
-            source_directory = os.path.join(root, directory)
-            shutil.copytree(source_directory, parent_dir)
+            dir_path = os.path.join(root, directory)
+            for f in os.listdir(dir_path):
+                if os.path.isfile(f):
+                    shutil.move(f, parent_dir)
 
 
 class GradeNotebooks():
     async def grade(self, p, notebooks_zip):
         try:
             zip_folder = notebooks_zip.split(".")[0]
             with ZipFile(notebooks_zip, 'r') as zObject:
```

### Comparing `otter_service_stdalone-0.1.7/src/otter_service_stdalone/fs_logging.py` & `otter_service_stdalone-0.1.8/src/otter_service_stdalone/fs_logging.py`

 * *Files identical despite different names*

### Comparing `otter_service_stdalone-0.1.7/src/otter_service_stdalone/index.html` & `otter_service_stdalone-0.1.8/src/otter_service_stdalone/index.html`

 * *Files identical despite different names*

### Comparing `otter_service_stdalone-0.1.7/src/otter_service_stdalone.egg-info/PKG-INFO` & `otter_service_stdalone-0.1.8/src/otter_service_stdalone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-service-stdalone
-Version: 0.1.7
+Version: 0.1.8
 Summary: Grading Service for Instructors using Otter Grader
 Home-page: https://github.com/sean-morris/otter-service-stdalone
 Author: Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

