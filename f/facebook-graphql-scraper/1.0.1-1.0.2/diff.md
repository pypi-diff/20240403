# Comparing `tmp/facebook-graphql-scraper-1.0.1.tar.gz` & `tmp/facebook-graphql-scraper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-1.0.1.tar", last modified: Wed Apr  3 08:10:05 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-1.0.2.tar", last modified: Wed Apr  3 09:10:13 2024, max compression
```

## Comparing `facebook-graphql-scraper-1.0.1.tar` & `facebook-graphql-scraper-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.847328 facebook-graphql-scraper-1.0.1/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.1/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     5182 2024-04-03 08:10:05.846974 facebook-graphql-scraper-1.0.1/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4688 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.1/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.843723 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     5182 2024-04-03 08:10:05.000000 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 08:10:05.000000 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 08:10:05.000000 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 08:10:05.000000 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.844356 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.844711 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4816 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.845064 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     4953 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/pages/page_optional.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.845273 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/resources/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/resources/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     1052 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.845441 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.846446 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 08:10:05.847413 facebook-graphql-scraper-1.0.1/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      909 2024-04-03 08:09:32.000000 facebook-graphql-scraper-1.0.1/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:10:13.478284 facebook-graphql-scraper-1.0.2/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.2/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     5279 2024-04-03 09:10:13.477791 facebook-graphql-scraper-1.0.2/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4785 2024-04-03 09:09:31.000000 facebook-graphql-scraper-1.0.2/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:10:13.474945 facebook-graphql-scraper-1.0.2/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     5279 2024-04-03 09:10:13.000000 facebook-graphql-scraper-1.0.2/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 09:10:13.000000 facebook-graphql-scraper-1.0.2/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 09:10:13.000000 facebook-graphql-scraper-1.0.2/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 09:10:13.000000 facebook-graphql-scraper-1.0.2/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:10:13.475598 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:10:13.475953 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4816 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:10:13.476311 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     4953 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:10:13.476520 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/resources/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/resources/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     1052 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:10:13.476669 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:10:13.477352 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-1.0.2/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 09:10:13.478386 facebook-graphql-scraper-1.0.2/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      909 2024-04-03 09:09:48.000000 facebook-graphql-scraper-1.0.2/setup.py
```

### Comparing `facebook-graphql-scraper-1.0.1/LICENSE` & `facebook-graphql-scraper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/PKG-INFO` & `facebook-graphql-scraper-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,23 @@
 
 Or, to install the latest master branch:
 
 ```sh
 pip install git+https://github.com/faustren/facebook-graphql-scraper.git
 ```
 
+## Requirements
+
+```sh
+ipython==8.19.0
+pytz==2023.3.post1
+selenium_wire==5.1.0
+tqdm==4.66.1
+```
+
 ### Usage
 
 You can choose between two methods to collect user posts data. 
 
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
```

### Comparing `facebook-graphql-scraper-1.0.1/README.md` & `facebook-graphql-scraper-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 
 Or, to install the latest master branch:
 
 ```sh
 pip install git+https://github.com/faustren/facebook-graphql-scraper.git
 ```
 
+## Requirements
+
+```sh
+ipython==8.19.0
+pytz==2023.3.post1
+selenium_wire==5.1.0
+tqdm==4.66.1
+```
+
 ### Usage
 
 You can choose between two methods to collect user posts data. 
 
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
```

### Comparing `facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-1.0.2/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,23 @@
 
 Or, to install the latest master branch:
 
 ```sh
 pip install git+https://github.com/faustren/facebook-graphql-scraper.git
 ```
 
+## Requirements
+
+```sh
+ipython==8.19.0
+pytz==2023.3.post1
+selenium_wire==5.1.0
+tqdm==4.66.1
+```
+
 ### Usage
 
 You can choose between two methods to collect user posts data. 
 
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
```

### Comparing `facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-1.0.2/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-1.0.2/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-1.0.2/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-1.0.2/fb_graphql_scraper/pages/page_optional.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/test_program.py` & `facebook-graphql-scraper-1.0.2/fb_graphql_scraper/test_program.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-1.0.2/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-1.0.2/fb_graphql_scraper/utils/parser.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-1.0.2/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.1/setup.py` & `facebook-graphql-scraper-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='1.0.1',
+    version='1.0.2',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
         "fb_graphql_scraper.resources"
```

