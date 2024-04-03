# Comparing `tmp/facebook-graphql-scraper-0.4.tar.gz` & `tmp/facebook-graphql-scraper-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-0.4.tar", last modified: Wed Apr  3 03:59:51 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-0.5.tar", last modified: Wed Apr  3 06:29:35 2024, max compression
```

## Comparing `facebook-graphql-scraper-0.4.tar` & `facebook-graphql-scraper-0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:59:51.104852 facebook-graphql-scraper-0.4/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.4/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 03:59:51.104467 facebook-graphql-scraper-0.4/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.4/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:59:51.101002 facebook-graphql-scraper-0.4/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 03:59:50.000000 facebook-graphql-scraper-0.4/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      515 2024-04-03 03:59:51.000000 facebook-graphql-scraper-0.4/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 03:59:50.000000 facebook-graphql-scraper-0.4/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 03:59:50.000000 facebook-graphql-scraper-0.4/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:59:51.101829 facebook-graphql-scraper-0.4/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.4/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:59:51.102228 facebook-graphql-scraper-0.4/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)      852 2024-04-03 02:58:29.000000 facebook-graphql-scraper-0.4/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4835 2024-04-03 03:45:40.000000 facebook-graphql-scraper-0.4/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:59:51.102731 facebook-graphql-scraper-0.4/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)     4984 2024-04-03 03:45:03.000000 facebook-graphql-scraper-0.4/fb_graphql_scraper/pages/page_optional.py
--rw-r--r--   0 renren     (501) staff       (20)      748 2024-04-03 03:57:17.000000 facebook-graphql-scraper-0.4/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:59:51.103879 facebook-graphql-scraper-0.4/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.4/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3481 2024-04-03 03:45:21.000000 facebook-graphql-scraper-0.4/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.4/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 03:59:51.104934 facebook-graphql-scraper-0.4/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)     1007 2024-04-03 03:58:12.000000 facebook-graphql-scraper-0.4/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:29:35.598538 facebook-graphql-scraper-0.5/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.5/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 06:29:35.598217 facebook-graphql-scraper-0.5/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.5/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:29:35.594056 facebook-graphql-scraper-0.5/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 06:29:35.000000 facebook-graphql-scraper-0.5/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      515 2024-04-03 06:29:35.000000 facebook-graphql-scraper-0.5/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 06:29:35.000000 facebook-graphql-scraper-0.5/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 06:29:35.000000 facebook-graphql-scraper-0.5/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:29:35.594790 facebook-graphql-scraper-0.5/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.5/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:29:35.595110 facebook-graphql-scraper-0.5/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)      852 2024-04-03 02:58:29.000000 facebook-graphql-scraper-0.5/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4835 2024-04-03 03:45:40.000000 facebook-graphql-scraper-0.5/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:29:35.596215 facebook-graphql-scraper-0.5/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)     4984 2024-04-03 03:45:03.000000 facebook-graphql-scraper-0.5/fb_graphql_scraper/pages/page_optional.py
+-rw-r--r--   0 renren     (501) staff       (20)      748 2024-04-03 03:57:17.000000 facebook-graphql-scraper-0.5/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:29:35.597620 facebook-graphql-scraper-0.5/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.5/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3481 2024-04-03 03:45:21.000000 facebook-graphql-scraper-0.5/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.5/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 06:29:35.598621 facebook-graphql-scraper-0.5/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      858 2024-04-03 06:29:13.000000 facebook-graphql-scraper-0.5/setup.py
```

### Comparing `facebook-graphql-scraper-0.4/LICENSE` & `facebook-graphql-scraper-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/PKG-INFO` & `facebook-graphql-scraper-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.4
+Version: 0.5
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.4/README.md` & `facebook-graphql-scraper-0.5/README.md`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-0.5/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.4
+Version: 0.5
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.4/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-0.5/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-0.5/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-0.5/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-0.5/fb_graphql_scraper/pages/page_optional.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/fb_graphql_scraper/test_program.py` & `facebook-graphql-scraper-0.5/fb_graphql_scraper/test_program.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-0.5/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-0.5/fb_graphql_scraper/utils/parser.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-0.5/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.4/setup.py` & `facebook-graphql-scraper-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='0.4',
+    version='0.5',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
-        "fb_graphql_scraper.resources", 
-        "fb_graphql_scraper.utils",
-        "fb_graphql_scraper.resources.data",
-        "fb_graphql_scraper.resources.chromedriver-mac-arm64"],
+        "fb_graphql_scraper.utils"],
     license='MIT',
     description='Implement Facebook scraper for post data retrieval',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='FaustRen',
     author_email='faustren1z@gmail.com',
     url='https://github.com/FaustRen/facebook_graphql_scraper',
```

