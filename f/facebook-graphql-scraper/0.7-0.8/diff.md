# Comparing `tmp/facebook-graphql-scraper-0.7.tar.gz` & `tmp/facebook-graphql-scraper-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-0.7.tar", last modified: Wed Apr  3 07:16:48 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-0.8.tar", last modified: Wed Apr  3 07:38:41 2024, max compression
```

## Comparing `facebook-graphql-scraper-0.7.tar` & `facebook-graphql-scraper-0.8.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.769139 facebook-graphql-scraper-0.7/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.7/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 07:16:48.768777 facebook-graphql-scraper-0.7/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.7/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.763838 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 07:16:48.000000 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      750 2024-04-03 07:16:48.000000 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 07:16:48.000000 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 07:16:48.000000 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.764740 facebook-graphql-scraper-0.7/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:14:38.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.765457 facebook-graphql-scraper-0.7/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)       23 2024-04-03 07:10:44.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      858 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4734 2024-04-03 07:15:48.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.766035 facebook-graphql-scraper-0.7/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     5001 2024-04-03 07:12:17.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/pages/page_optional.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.766638 facebook-graphql-scraper-0.7/fb_graphql_scraper/resources/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/resources/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/resources/test_resources.py
--rw-r--r--   0 renren     (501) staff       (20)      807 2024-04-03 07:13:00.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.766826 facebook-graphql-scraper-0.7/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.768025 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:00:23.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 07:16:48.769213 facebook-graphql-scraper-0.7/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      907 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.7/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.851220 facebook-graphql-scraper-0.8/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.8/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 07:38:41.850898 facebook-graphql-scraper-0.8/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.8/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.847979 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 07:38:41.000000 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 07:38:41.000000 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 07:38:41.000000 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 07:38:41.000000 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.848631 facebook-graphql-scraper-0.8/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:14:38.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.848989 facebook-graphql-scraper-0.8/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:32:48.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4814 2024-04-03 07:38:12.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.849324 facebook-graphql-scraper-0.8/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     5001 2024-04-03 07:12:17.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.849568 facebook-graphql-scraper-0.8/fb_graphql_scraper/resources/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/resources/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     1076 2024-04-03 07:36:00.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.849727 facebook-graphql-scraper-0.8/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.850417 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:00:23.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 07:38:41.851304 facebook-graphql-scraper-0.8/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      907 2024-04-03 07:33:18.000000 facebook-graphql-scraper-0.8/setup.py
```

### Comparing `facebook-graphql-scraper-0.7/LICENSE` & `facebook-graphql-scraper-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.7/PKG-INFO` & `facebook-graphql-scraper-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.7
+Version: 0.8
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.7/README.md` & `facebook-graphql-scraper-0.8/README.md`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.7
+Version: 0.8
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,13 +9,12 @@
 fb_graphql_scraper/facebook_graphql_scraper.py
 fb_graphql_scraper/test_program.py
 fb_graphql_scraper/base/__init__.py
 fb_graphql_scraper/base/base_page.py
 fb_graphql_scraper/pages/__init__.py
 fb_graphql_scraper/pages/page_optional.py
 fb_graphql_scraper/resources/__init__.py
-fb_graphql_scraper/resources/test_resources.py
 fb_graphql_scraper/tests/__init__.py
 fb_graphql_scraper/utils/__init__.py
 fb_graphql_scraper/utils/locator.py
 fb_graphql_scraper/utils/parser.py
 fb_graphql_scraper/utils/utils.py
```

### Comparing `facebook-graphql-scraper-0.7/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-0.8/fb_graphql_scraper/base/base_page.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding:utf-8 -*-
 from seleniumwire import webdriver
-from pathlib import Path
+from selenium.webdriver.chrome.service import Service
 
 
 class BasePage(object):
-    # driver_path = str(Path(__file__).resolve().parent.parent/ 'resources' / 'chromedriver-mac-arm64' / 'chromedriver')
-    def __init__(self):
+    def __init__(self, driver_path):
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_argument("--disable-blink-features")
         chrome_options.add_argument("--disable-notifications")
         chrome_options.add_argument("--disable-blink-features=AutomationControlled")
         chrome_options.add_argument("--headless=new")
-        self.driver = webdriver.Chrome(options=chrome_options)
+        svc = Service(driver_path)
+        self.driver = webdriver.Chrome(service=svc,options=chrome_options)
         self.driver.maximize_window()
 
 # from selenium.webdriver.chrome.service import Service
 # svc = Service(BasePage.driver_path)
-# self.driver = webdriver.Chrome(service=svc, options=chrome_options)
-##
+# self.driver = webdriver.Chrome(service=svc, options=chrome_options)
```

### Comparing `facebook-graphql-scraper-0.7/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-0.8/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from fb_graphql_scraper.utils.locator import *
 from fb_graphql_scraper.utils.utils import *
 from fb_graphql_scraper.utils.parser import RequestsParser
 from tqdm import tqdm, trange
 
 
 class FacebookSettings:
-    def __init__(self,url,username_or_userid:str=None,pwd:str=None):
+    def __init__(self,url,username_or_userid:str=None,pwd:str=None,driver_path:str=None):
         super().__init__()
         self.username_or_userid = username_or_userid
         self.pwd = pwd
         self.url=url
-        self.set_spider()
+        self.set_spider(driver_path=driver_path)
         self.set_container()
     
-    def set_spider(self):
+    def set_spider(self, driver_path):
         """>> Description: Auto login account or click "X" button to continue, 
         but some account can't not be display info if you don't login account
         >> Args: url (_str_): target user which you want to collect data."""
-        self.base_page = BasePage()
+        self.base_page = BasePage(driver_path=driver_path)
         self.page_optional = PageOptional(
             url_in=self.url, 
             driver=self.base_page.driver,
             username_or_userid=self.username_or_userid,
             pwd=self.pwd
         )
         time.sleep(5)
```

### Comparing `facebook-graphql-scraper-0.7/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-0.8/fb_graphql_scraper/pages/page_optional.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.7/fb_graphql_scraper/test_program.py` & `facebook-graphql-scraper-0.8/fb_graphql_scraper/test_program.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
 from dotenv import load_dotenv
 import os
 
 
 # ## Load account info
 # load_dotenv()
-# username_or_userid = os.getenv("FB_USERNAME_OR_USERID")
+# username_or_userid = os.getenv("FB_USERNAME_OR_USERID") # Facebook帳號密碼
 # pwd = os.getenv("FBPASSWORD")
+# driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 
 # #%%
 # ## Log in account version
 # fb_user_id = "KaiCenatOfficial"
 # url = "https://www.facebook.com/"
 # res = fb_graphql_scraper.get_user_posts(
 #     fb_username_or_userid=fb_user_id, 
@@ -22,14 +23,15 @@
 #     username_or_userid=username_or_userid,
 #     pwd=pwd
 # )
 # res
 #%%
 ## Without logging in account version
 fb_user_id = "KaiCenatOfficial"
+driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
     loop_times=50
 )
 res
 # %%
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/parser.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.7/setup.py` & `facebook-graphql-scraper-0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='0.7',
+    version='0.8',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
         "fb_graphql_scraper.resources"
```

