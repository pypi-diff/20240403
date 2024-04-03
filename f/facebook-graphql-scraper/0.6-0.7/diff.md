# Comparing `tmp/facebook-graphql-scraper-0.6.tar.gz` & `tmp/facebook-graphql-scraper-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-0.6.tar", last modified: Wed Apr  3 06:33:20 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-0.7.tar", last modified: Wed Apr  3 07:16:48 2024, max compression
```

## Comparing `facebook-graphql-scraper-0.6.tar` & `facebook-graphql-scraper-0.7.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:33:20.748245 facebook-graphql-scraper-0.6/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.6/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 06:33:20.747916 facebook-graphql-scraper-0.6/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.6/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:33:20.745099 facebook-graphql-scraper-0.6/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 06:33:20.000000 facebook-graphql-scraper-0.6/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      515 2024-04-03 06:33:20.000000 facebook-graphql-scraper-0.6/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 06:33:20.000000 facebook-graphql-scraper-0.6/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 06:33:20.000000 facebook-graphql-scraper-0.6/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:33:20.745821 facebook-graphql-scraper-0.6/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.6/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:33:20.746024 facebook-graphql-scraper-0.6/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)      852 2024-04-03 02:58:29.000000 facebook-graphql-scraper-0.6/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4835 2024-04-03 03:45:40.000000 facebook-graphql-scraper-0.6/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:33:20.746398 facebook-graphql-scraper-0.6/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)     4984 2024-04-03 03:45:03.000000 facebook-graphql-scraper-0.6/fb_graphql_scraper/pages/page_optional.py
--rw-r--r--   0 renren     (501) staff       (20)      748 2024-04-03 03:57:17.000000 facebook-graphql-scraper-0.6/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 06:33:20.747423 facebook-graphql-scraper-0.6/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.6/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3481 2024-04-03 03:45:21.000000 facebook-graphql-scraper-0.6/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.6/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 06:33:20.748318 facebook-graphql-scraper-0.6/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      908 2024-04-03 06:31:50.000000 facebook-graphql-scraper-0.6/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.769139 facebook-graphql-scraper-0.7/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.7/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 07:16:48.768777 facebook-graphql-scraper-0.7/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.7/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.763838 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 07:16:48.000000 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      750 2024-04-03 07:16:48.000000 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 07:16:48.000000 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 07:16:48.000000 facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.764740 facebook-graphql-scraper-0.7/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:14:38.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.765457 facebook-graphql-scraper-0.7/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)       23 2024-04-03 07:10:44.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      858 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4734 2024-04-03 07:15:48.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.766035 facebook-graphql-scraper-0.7/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     5001 2024-04-03 07:12:17.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.766638 facebook-graphql-scraper-0.7/fb_graphql_scraper/resources/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/resources/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/resources/test_resources.py
+-rw-r--r--   0 renren     (501) staff       (20)      807 2024-04-03 07:13:00.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.766826 facebook-graphql-scraper-0.7/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:16:48.768025 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:00:23.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 07:16:48.769213 facebook-graphql-scraper-0.7/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      907 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.7/setup.py
```

### Comparing `facebook-graphql-scraper-0.6/LICENSE` & `facebook-graphql-scraper-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.6/PKG-INFO` & `facebook-graphql-scraper-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.6
+Version: 0.7
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.6/README.md` & `facebook-graphql-scraper-0.7/README.md`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.6/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.6
+Version: 0.7
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.6/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-0.7/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,12 +4,18 @@
 facebook_graphql_scraper.egg-info/PKG-INFO
 facebook_graphql_scraper.egg-info/SOURCES.txt
 facebook_graphql_scraper.egg-info/dependency_links.txt
 facebook_graphql_scraper.egg-info/top_level.txt
 fb_graphql_scraper/__init__.py
 fb_graphql_scraper/facebook_graphql_scraper.py
 fb_graphql_scraper/test_program.py
+fb_graphql_scraper/base/__init__.py
 fb_graphql_scraper/base/base_page.py
+fb_graphql_scraper/pages/__init__.py
 fb_graphql_scraper/pages/page_optional.py
+fb_graphql_scraper/resources/__init__.py
+fb_graphql_scraper/resources/test_resources.py
+fb_graphql_scraper/tests/__init__.py
+fb_graphql_scraper/utils/__init__.py
 fb_graphql_scraper/utils/locator.py
 fb_graphql_scraper/utils/parser.py
 fb_graphql_scraper/utils/utils.py
```

### Comparing `facebook-graphql-scraper-0.6/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-0.7/fb_graphql_scraper/base/base_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding:utf-8 -*-
 from seleniumwire import webdriver
 from pathlib import Path
 
 
 class BasePage(object):
-    driver_path = str(Path(__file__).resolve().parent.parent/ 'resources' / 'chromedriver-mac-arm64' / 'chromedriver')
+    # driver_path = str(Path(__file__).resolve().parent.parent/ 'resources' / 'chromedriver-mac-arm64' / 'chromedriver')
     def __init__(self):
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_argument("--disable-blink-features")
         chrome_options.add_argument("--disable-notifications")
         chrome_options.add_argument("--disable-blink-features=AutomationControlled")
         chrome_options.add_argument("--headless=new")
         self.driver = webdriver.Chrome(options=chrome_options)
         self.driver.maximize_window()
 
 # from selenium.webdriver.chrome.service import Service
 # svc = Service(BasePage.driver_path)
-# self.driver = webdriver.Chrome(service=svc, options=chrome_options)
+# self.driver = webdriver.Chrome(service=svc, options=chrome_options)
+##
```

### Comparing `facebook-graphql-scraper-0.6/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-0.7/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import time
 from IPython.display import display
 from seleniumwire.utils import decode
-from .base.base_page import *
-from .pages.page_optional import *
-from .utils.locator import *
-from .utils.utils import *
-from .utils.parser import RequestsParser
+from fb_graphql_scraper.base.base_page import *
+from fb_graphql_scraper.pages.page_optional import *
+from fb_graphql_scraper.utils.locator import *
+from fb_graphql_scraper.utils.utils import *
+from fb_graphql_scraper.utils.parser import RequestsParser
 from tqdm import tqdm, trange
 
 
 class FacebookSettings:
     def __init__(self,url,username_or_userid:str=None,pwd:str=None):
         super().__init__()
         self.username_or_userid = username_or_userid
@@ -117,10 +117,8 @@
             'reaction_count.count',
             'comment_rendering_instance.comments.total_count',
             'share_count.count',
             'sub_reactions',
             'context',
             'video_view_count'
         ]]
-        final_res.to_csv(f"./resources/data/res/{fb_username_or_userid}.csv", index=False)
-        final_res.to_excel(f"./resources/data/res/{fb_username_or_userid}_excel.xlsx", index=False)
         return final_res
```

### Comparing `facebook-graphql-scraper-0.6/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-0.7/fb_graphql_scraper/pages/page_optional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from ..utils.locator import *
+from fb_graphql_scraper.utils.locator import *
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.keys import Keys
 import time
```

### Comparing `facebook-graphql-scraper-0.6/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.6/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 from seleniumwire.utils import decode
 import json
-from ..utils.utils import *
+from fb_graphql_scraper.utils.utils import *
 
 
 class RequestsParser(object):
     def __init__(self, driver) -> None:
         self.driver = driver
         self.res_new = []
         self.feedback_list = []
```

### Comparing `facebook-graphql-scraper-0.6/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-0.7/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.6/setup.py` & `facebook-graphql-scraper-0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='0.6',
+    version='0.7',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
-        "fb_graphql_scraper.resources",
+        "fb_graphql_scraper.resources"
         ],
     license='MIT',
     description='Implement Facebook scraper for post data retrieval',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='FaustRen',
     author_email='faustren1z@gmail.com',
```

