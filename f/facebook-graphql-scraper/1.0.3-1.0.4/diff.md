# Comparing `tmp/facebook-graphql-scraper-1.0.3.tar.gz` & `tmp/facebook-graphql-scraper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-1.0.3.tar", last modified: Wed Apr  3 09:25:42 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-1.0.4.tar", last modified: Wed Apr  3 10:05:37 2024, max compression
```

## Comparing `facebook-graphql-scraper-1.0.3.tar` & `facebook-graphql-scraper-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:25:42.107468 facebook-graphql-scraper-1.0.3/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.3/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     5153 2024-04-03 09:25:42.107129 facebook-graphql-scraper-1.0.3/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4659 2024-04-03 09:22:44.000000 facebook-graphql-scraper-1.0.3/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:25:42.103441 facebook-graphql-scraper-1.0.3/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     5153 2024-04-03 09:25:41.000000 facebook-graphql-scraper-1.0.3/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 09:25:42.000000 facebook-graphql-scraper-1.0.3/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 09:25:41.000000 facebook-graphql-scraper-1.0.3/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 09:25:41.000000 facebook-graphql-scraper-1.0.3/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:25:42.104699 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:25:42.105215 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4816 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:25:42.105577 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     4953 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/pages/page_optional.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:25:42.105805 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/resources/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/resources/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     1052 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:25:42.105960 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 09:25:42.106660 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-1.0.3/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 09:25:42.107541 facebook-graphql-scraper-1.0.3/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      909 2024-04-03 09:25:33.000000 facebook-graphql-scraper-1.0.3/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.263063 facebook-graphql-scraper-1.0.4/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.4/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     5153 2024-04-03 10:05:37.262708 facebook-graphql-scraper-1.0.4/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4659 2024-04-03 09:22:44.000000 facebook-graphql-scraper-1.0.4/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.259676 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     5153 2024-04-03 10:05:37.000000 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 10:05:37.000000 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 10:05:37.000000 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 10:05:37.000000 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.260382 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.260738 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4816 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.261128 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     4903 2024-04-03 10:04:53.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.261357 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/resources/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/resources/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     1052 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.261521 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.262235 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 10:05:37.263141 facebook-graphql-scraper-1.0.4/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      909 2024-04-03 10:05:18.000000 facebook-graphql-scraper-1.0.4/setup.py
```

### Comparing `facebook-graphql-scraper-1.0.3/LICENSE` & `facebook-graphql-scraper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/PKG-INFO` & `facebook-graphql-scraper-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.3
+Version: 1.0.4
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-1.0.3/README.md` & `facebook-graphql-scraper-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.3
+Version: 1.0.4
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-1.0.3/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/pages/page_optional.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
             print(f"Clear unsuccessfully, message: {e}")
 
     def get_in_url(self):
         self.driver.get(url=self.url)
 
     def login_account(self, user: str, password: str, user_element, pwd_element):
         user_element = self.driver.find_element(By.XPATH, user_element)
-        user_element = self.driver.find_element()
         user_element.send_keys(user)
         password_element = self.driver.find_element(By.XPATH, pwd_element)
         password_element.send_keys(password)
         password_element.send_keys(Keys.ENTER)
 
     def scroll_window(self):
         self.driver.execute_script(
```

### Comparing `facebook-graphql-scraper-1.0.3/fb_graphql_scraper/test_program.py` & `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/test_program.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/parser.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.3/setup.py` & `facebook-graphql-scraper-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='1.0.3',
+    version='1.0.4',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
         "fb_graphql_scraper.resources"
```

