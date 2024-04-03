# Comparing `tmp/facebook-graphql-scraper-0.2.tar.gz` & `tmp/facebook-graphql-scraper-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-0.2.tar", last modified: Wed Apr  3 03:29:59 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-0.3.tar", last modified: Wed Apr  3 03:52:23 2024, max compression
```

## Comparing `facebook-graphql-scraper-0.2.tar` & `facebook-graphql-scraper-0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:29:59.276609 facebook-graphql-scraper-0.2/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.2/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 03:29:59.276270 facebook-graphql-scraper-0.2/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.2/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:29:59.272952 facebook-graphql-scraper-0.2/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 03:29:59.000000 facebook-graphql-scraper-0.2/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      515 2024-04-03 03:29:59.000000 facebook-graphql-scraper-0.2/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 03:29:59.000000 facebook-graphql-scraper-0.2/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 03:29:59.000000 facebook-graphql-scraper-0.2/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:29:59.273656 facebook-graphql-scraper-0.2/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.2/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:29:59.273924 facebook-graphql-scraper-0.2/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)      852 2024-04-03 02:58:29.000000 facebook-graphql-scraper-0.2/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4830 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.2/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:29:59.274355 facebook-graphql-scraper-0.2/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)     4982 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.2/fb_graphql_scraper/pages/page_optional.py
--rw-r--r--   0 renren     (501) staff       (20)      748 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.2/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:29:59.275507 facebook-graphql-scraper-0.2/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.2/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3479 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.2/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.2/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 03:29:59.276679 facebook-graphql-scraper-0.2/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      846 2024-04-03 03:29:57.000000 facebook-graphql-scraper-0.2/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:52:23.394567 facebook-graphql-scraper-0.3/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.3/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 03:52:23.394249 facebook-graphql-scraper-0.3/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.3/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:52:23.391092 facebook-graphql-scraper-0.3/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 03:52:23.000000 facebook-graphql-scraper-0.3/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      515 2024-04-03 03:52:23.000000 facebook-graphql-scraper-0.3/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 03:52:23.000000 facebook-graphql-scraper-0.3/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 03:52:23.000000 facebook-graphql-scraper-0.3/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:52:23.391865 facebook-graphql-scraper-0.3/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.3/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:52:23.392183 facebook-graphql-scraper-0.3/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)      852 2024-04-03 02:58:29.000000 facebook-graphql-scraper-0.3/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4835 2024-04-03 03:45:40.000000 facebook-graphql-scraper-0.3/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:52:23.392607 facebook-graphql-scraper-0.3/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)     4984 2024-04-03 03:45:03.000000 facebook-graphql-scraper-0.3/fb_graphql_scraper/pages/page_optional.py
+-rw-r--r--   0 renren     (501) staff       (20)      748 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.3/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 03:52:23.393701 facebook-graphql-scraper-0.3/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.3/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3481 2024-04-03 03:45:21.000000 facebook-graphql-scraper-0.3/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.3/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 03:52:23.394644 facebook-graphql-scraper-0.3/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)     1007 2024-04-03 03:52:08.000000 facebook-graphql-scraper-0.3/setup.py
```

### Comparing `facebook-graphql-scraper-0.2/LICENSE` & `facebook-graphql-scraper-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.2/PKG-INFO` & `facebook-graphql-scraper-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.2
+Version: 0.3
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.2/README.md` & `facebook-graphql-scraper-0.3/README.md`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.2/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-0.3/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.2
+Version: 0.3
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-0.2/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-0.3/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.2/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-0.3/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.2/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-0.3/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import time
 from IPython.display import display
 from seleniumwire.utils import decode
-from base.base_page import *
-from pages.page_optional import *
-from utils.locator import *
-from utils.utils import *
-from utils.parser import RequestsParser
+from .base.base_page import *
+from .pages.page_optional import *
+from .utils.locator import *
+from .utils.utils import *
+from .utils.parser import RequestsParser
 from tqdm import tqdm, trange
 
 
 class FacebookSettings:
     def __init__(self,url,username_or_userid:str=None,pwd:str=None):
         super().__init__()
         self.username_or_userid = username_or_userid
```

### Comparing `facebook-graphql-scraper-0.2/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-0.3/fb_graphql_scraper/pages/page_optional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from utils.locator import *
+from ..utils.locator import *
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.keys import Keys
 import time
```

### Comparing `facebook-graphql-scraper-0.2/fb_graphql_scraper/test_program.py` & `facebook-graphql-scraper-0.3/fb_graphql_scraper/test_program.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.2/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-0.3/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.2/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-0.3/fb_graphql_scraper/utils/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 from seleniumwire.utils import decode
 import json
-from utils.utils import *
+from ..utils.utils import *
 
 
 class RequestsParser(object):
     def __init__(self, driver) -> None:
         self.driver = driver
         self.res_new = []
         self.feedback_list = []
```

### Comparing `facebook-graphql-scraper-0.2/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-0.3/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.2/setup.py` & `facebook-graphql-scraper-0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='0.2',
-    packages=["fb_graphql_scraper","fb_graphql_scraper.pages","fb_graphql_scraper.base", "fb_graphql_scraper.tests", "fb_graphql_scraper.resources", "fb_graphql_scraper.utils"],
+    version='0.3',
+    packages=[
+        "fb_graphql_scraper",
+        "fb_graphql_scraper.pages",
+        "fb_graphql_scraper.base",
+        "fb_graphql_scraper.tests", 
+        "fb_graphql_scraper.resources", 
+        "fb_graphql_scraper.utils",
+        "fb_graphql_scraper.resources.data",
+        "fb_graphql_scraper.resources.chromedriver-mac-arm64"],
     license='MIT',
     description='Implement Facebook scraper for post data retrieval',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='FaustRen',
     author_email='faustren1z@gmail.com',
     url='https://github.com/FaustRen/facebook_graphql_scraper',
```

