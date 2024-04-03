# Comparing `tmp/facebook-graphql-scraper-0.9.tar.gz` & `tmp/facebook-graphql-scraper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-0.9.tar", last modified: Wed Apr  3 07:57:54 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-1.0.1.tar", last modified: Wed Apr  3 08:10:05 2024, max compression
```

## Comparing `facebook-graphql-scraper-0.9.tar` & `facebook-graphql-scraper-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.914114 facebook-graphql-scraper-0.9/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.9/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     5180 2024-04-03 07:57:54.913808 facebook-graphql-scraper-0.9/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4688 2024-04-03 07:57:17.000000 facebook-graphql-scraper-0.9/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.910704 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     5180 2024-04-03 07:57:54.000000 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 07:57:54.000000 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 07:57:54.000000 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 07:57:54.000000 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.911561 facebook-graphql-scraper-0.9/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.911957 facebook-graphql-scraper-0.9/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4726 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.912278 facebook-graphql-scraper-0.9/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     4953 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/pages/page_optional.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.912516 facebook-graphql-scraper-0.9/fb_graphql_scraper/resources/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/resources/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     1052 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.912667 facebook-graphql-scraper-0.9/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.913313 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 07:57:54.914191 facebook-graphql-scraper-0.9/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      907 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.847328 facebook-graphql-scraper-1.0.1/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.1/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     5182 2024-04-03 08:10:05.846974 facebook-graphql-scraper-1.0.1/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4688 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.1/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.843723 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     5182 2024-04-03 08:10:05.000000 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 08:10:05.000000 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 08:10:05.000000 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 08:10:05.000000 facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.844356 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.844711 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4816 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.845064 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     4953 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.845273 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/resources/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/resources/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     1052 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.845441 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 08:10:05.846446 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 08:10:05.847413 facebook-graphql-scraper-1.0.1/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      909 2024-04-03 08:09:32.000000 facebook-graphql-scraper-1.0.1/setup.py
```

### Comparing `facebook-graphql-scraper-0.9/LICENSE` & `facebook-graphql-scraper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/PKG-INFO` & `facebook-graphql-scraper-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.9
+Version: 1.0.1
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.9/README.md` & `facebook-graphql-scraper-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.9
+Version: 1.0.1
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-1.0.1/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,16 @@
             "post_likes": [],
             "comment_share_type": [],
             "comment_share_value": []
         }
 
 
 class FacebookGraphqlScraper(FacebookSettings):
-    def __init__(self,url="https://www.facebook.com/",fb_account:str=None, pwd:str=None):
-        super().__init__(url=url, fb_account=fb_account, pwd=pwd)
+    def __init__(self,url="https://www.facebook.com/",fb_account:str=None, pwd:str=None,driver_path:str=None):
+        super().__init__(url=url, fb_account=fb_account, pwd=pwd,driver_path=driver_path)
 
     def checking_page(self):
         try:
             self.page_optional.click_reject_login_button()
             self.page_optional.scroll_window()
         except Exception as e:
             print(f"Get in to page unsucessfully, quit driver.\n error message: {e}")
@@ -61,17 +61,17 @@
     def move_to_next_kol(self, url:str):
         self.page_optional.driver.get(url=url)
 
     def pause(self):
         time.sleep(1)
 
     @classmethod
-    def get_user_posts(cls, fb_username_or_userid:str, loop_times:int=50, fb_account:str=None, pwd:str=None):
+    def get_user_posts(cls, fb_username_or_userid:str, loop_times:int=50, fb_account:str=None, pwd:str=None,driver_path:str=None):
         url = "https://www.facebook.com/"+fb_username_or_userid
-        spider = cls(url=url,fb_account=fb_account,pwd=pwd)
+        spider = cls(url=url,fb_account=fb_account,pwd=pwd,driver_path=driver_path)
         # Scroll page
         for round in tqdm(range(loop_times)): # 滾動次數
             spider.page_optional.scroll_window()
             spider.pause()
 
         # Collect data
         driver_requests = spider.page_optional.driver.requests
```

### Comparing `facebook-graphql-scraper-0.9/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/pages/page_optional.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/fb_graphql_scraper/test_program.py` & `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/test_program.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/parser.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-1.0.1/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.9/setup.py` & `facebook-graphql-scraper-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='0.9',
+    version='1.0.1',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
         "fb_graphql_scraper.resources"
```

