# Comparing `tmp/GoogleNb-0.0.1.tar.gz` & `tmp/GoogleNb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleNb-0.0.1.tar", last modified: Tue Apr  2 22:21:50 2024, max compression
+gzip compressed data, was "GoogleNb-0.0.2.tar", last modified: Tue Apr  2 22:17:59 2024, max compression
```

## Comparing `GoogleNb-0.0.1.tar` & `GoogleNb-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 22:21:50.826701 GoogleNb-0.0.1/
--rw-rw-rw-   0        0        0     1083 2024-02-04 19:16:00.000000 GoogleNb-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      788 2024-04-02 22:21:50.824702 GoogleNb-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-04-02 22:11:48.000000 GoogleNb-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 22:21:50.826701 GoogleNb-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1083 2024-04-02 22:21:43.000000 GoogleNb-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:21:50.795701 GoogleNb-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 22:21:50.803700 GoogleNb-0.0.1/src/GoogleNb/
--rw-rw-rw-   0        0        0     1713 2024-03-27 13:07:44.000000 GoogleNb-0.0.1/src/GoogleNb/GoogleDrive.py
--rw-rw-rw-   0        0        0     6008 2024-04-02 22:13:14.000000 GoogleNb-0.0.1/src/GoogleNb/GoogleSheet.py
--rw-rw-rw-   0        0        0        0 2024-03-19 20:27:02.000000 GoogleNb-0.0.1/src/GoogleNb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:21:50.823700 GoogleNb-0.0.1/src/GoogleNb.egg-info/
--rw-rw-rw-   0        0        0      788 2024-04-02 22:21:50.000000 GoogleNb-0.0.1/src/GoogleNb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-04-02 22:21:50.000000 GoogleNb-0.0.1/src/GoogleNb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 22:21:50.000000 GoogleNb-0.0.1/src/GoogleNb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-02 22:21:50.000000 GoogleNb-0.0.1/src/GoogleNb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 22:21:50.000000 GoogleNb-0.0.1/src/GoogleNb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 22:17:59.574269 GoogleNb-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2024-02-04 19:16:00.000000 GoogleNb-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      788 2024-04-02 22:17:59.572267 GoogleNb-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-04-02 22:11:48.000000 GoogleNb-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 22:17:59.574269 GoogleNb-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2024-03-29 21:45:41.000000 GoogleNb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:17:59.484268 GoogleNb-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:17:59.539268 GoogleNb-0.0.2/src/GoogleNb/
+-rw-rw-rw-   0        0        0     1713 2024-03-27 13:07:44.000000 GoogleNb-0.0.2/src/GoogleNb/GoogleDrive.py
+-rw-rw-rw-   0        0        0     6008 2024-04-02 22:13:14.000000 GoogleNb-0.0.2/src/GoogleNb/GoogleSheet.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 20:27:02.000000 GoogleNb-0.0.2/src/GoogleNb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:17:59.571267 GoogleNb-0.0.2/src/GoogleNb.egg-info/
+-rw-rw-rw-   0        0        0      788 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/top_level.txt
```

### Comparing `GoogleNb-0.0.1/LICENSE` & `GoogleNb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleNb-0.0.1/PKG-INFO` & `GoogleNb-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleNb
-Version: 0.0.1
+Version: 0.0.2
 Summary: API google
 Home-page: https://github.com/niba291/PyDrive
 Author: niba291
 Author-email: nibaldochavezp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleNb-0.0.1/setup.py` & `GoogleNb-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools                     import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name                            = "GoogleNb",
-    version                         = "0.0.1",
+    version                         = "0.0.2",
     author                          = "niba291",
     author_email                    = "nibaldochavezp@gmail.com",
     description                     = "API google",
     url                             = "https://github.com/niba291/PyDrive",
     license                         = "MIT",
     long_description                = long_description,
     long_description_content_type   = "text/markdown",
```

### Comparing `GoogleNb-0.0.1/src/GoogleNb/GoogleDrive.py` & `GoogleNb-0.0.2/src/GoogleNb/GoogleDrive.py`

 * *Files identical despite different names*

### Comparing `GoogleNb-0.0.1/src/GoogleNb/GoogleSheet.py` & `GoogleNb-0.0.2/src/GoogleNb/GoogleSheet.py`

 * *Files identical despite different names*

### Comparing `GoogleNb-0.0.1/src/GoogleNb.egg-info/PKG-INFO` & `GoogleNb-0.0.2/src/GoogleNb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleNb
-Version: 0.0.1
+Version: 0.0.2
 Summary: API google
 Home-page: https://github.com/niba291/PyDrive
 Author: niba291
 Author-email: nibaldochavezp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

