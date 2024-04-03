# Comparing `tmp/facebook-graphql-scraper-0.8.tar.gz` & `tmp/facebook-graphql-scraper-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-0.8.tar", last modified: Wed Apr  3 07:38:41 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-0.9.tar", last modified: Wed Apr  3 07:57:54 2024, max compression
```

## Comparing `facebook-graphql-scraper-0.8.tar` & `facebook-graphql-scraper-0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.851220 facebook-graphql-scraper-0.8/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.8/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 07:38:41.850898 facebook-graphql-scraper-0.8/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4350 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.8/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.847979 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     4842 2024-04-03 07:38:41.000000 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 07:38:41.000000 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 07:38:41.000000 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 07:38:41.000000 facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.848631 facebook-graphql-scraper-0.8/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:14:38.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.848989 facebook-graphql-scraper-0.8/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:32:48.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4814 2024-04-03 07:38:12.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.849324 facebook-graphql-scraper-0.8/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     5001 2024-04-03 07:12:17.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/pages/page_optional.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.849568 facebook-graphql-scraper-0.8/fb_graphql_scraper/resources/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/resources/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     1076 2024-04-03 07:36:00.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.849727 facebook-graphql-scraper-0.8/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:38:41.850417 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:00:23.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 07:38:41.851304 facebook-graphql-scraper-0.8/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      907 2024-04-03 07:33:18.000000 facebook-graphql-scraper-0.8/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.914114 facebook-graphql-scraper-0.9/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-0.9/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     5180 2024-04-03 07:57:54.913808 facebook-graphql-scraper-0.9/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4688 2024-04-03 07:57:17.000000 facebook-graphql-scraper-0.9/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.910704 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     5180 2024-04-03 07:57:54.000000 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 07:57:54.000000 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 07:57:54.000000 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 07:57:54.000000 facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.911561 facebook-graphql-scraper-0.9/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.911957 facebook-graphql-scraper-0.9/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4726 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.912278 facebook-graphql-scraper-0.9/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     4953 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.912516 facebook-graphql-scraper-0.9/fb_graphql_scraper/resources/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/resources/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     1052 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.912667 facebook-graphql-scraper-0.9/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 07:57:54.913313 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 07:57:54.914191 facebook-graphql-scraper-0.9/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      907 2024-04-03 07:55:30.000000 facebook-graphql-scraper-0.9/setup.py
```

### Comparing `facebook-graphql-scraper-0.8/LICENSE` & `facebook-graphql-scraper-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.8/PKG-INFO` & `facebook-graphql-scraper-0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: facebook-graphql-scraper
-Version: 0.8
-Summary: Implement Facebook scraper for post data retrieval
-Home-page: https://github.com/FaustRen/facebook_graphql_scraper
-Author: FaustRen
-Author-email: faustren1z@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Facebook Graphql Scraper
 
 ## Install
 
 To install the latest release from PyPI:
 
 ```sh
@@ -34,44 +19,50 @@
 You can choose between two methods to collect user posts data. 
 
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
 
 ```python
-from facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
-from dotenv import load_dotenv
+# -*- coding: utf-8 -*-
 import os
+from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
+from dotenv import load_dotenv
 
 
-## Load account info
-load_dotenv()
-username_or_userid = os.getenv("FB_USERNAME_OR_USERID")
+# ## Load account info
+# load_dotenv()
+fb_account = os.getenv("FBACCOUNT") # Facebook帳號密碼
 pwd = os.getenv("FBPASSWORD")
 
-#%%
-## Log in account version
+# ## Log in account version
 fb_user_id = "KaiCenatOfficial"
+driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
-    username_or_userid=username_or_userid,
+    driver_path=driver_path,
+    fb_account=fb_account,
     pwd=pwd
 )
 res
-#%%
+
 ## Without logging in account version
 fb_user_id = "KaiCenatOfficial"
+driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
-    loop_times=50
+    loop_times=50,
+    driver_path=driver_path,
 )
 res
+# %%
+
 
 
 
 ```
 ### Optional parameters
 
 - **fb_user_id**: group id/fans page id/account id.
@@ -164,8 +155,8 @@
 
 
 ```python
 
 ## To-Do
 
 - Collect profile info
-- Collect image info
+- Collect image info
```

### Comparing `facebook-graphql-scraper-0.8/README.md` & `facebook-graphql-scraper-0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: facebook-graphql-scraper
+Version: 0.9
+Summary: Implement Facebook scraper for post data retrieval
+Home-page: https://github.com/FaustRen/facebook_graphql_scraper
+Author: FaustRen
+Author-email: faustren1z@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Facebook Graphql Scraper
 
 ## Install
 
 To install the latest release from PyPI:
 
 ```sh
@@ -19,44 +34,50 @@
 You can choose between two methods to collect user posts data. 
 
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
 
 ```python
-from facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
-from dotenv import load_dotenv
+# -*- coding: utf-8 -*-
 import os
+from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
+from dotenv import load_dotenv
 
 
-## Load account info
-load_dotenv()
-username_or_userid = os.getenv("FB_USERNAME_OR_USERID")
+# ## Load account info
+# load_dotenv()
+fb_account = os.getenv("FBACCOUNT") # Facebook帳號密碼
 pwd = os.getenv("FBPASSWORD")
 
-#%%
-## Log in account version
+# ## Log in account version
 fb_user_id = "KaiCenatOfficial"
+driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
-    username_or_userid=username_or_userid,
+    driver_path=driver_path,
+    fb_account=fb_account,
     pwd=pwd
 )
 res
-#%%
+
 ## Without logging in account version
 fb_user_id = "KaiCenatOfficial"
+driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
-    loop_times=50
+    loop_times=50,
+    driver_path=driver_path,
 )
 res
+# %%
+
 
 
 
 ```
 ### Optional parameters
 
 - **fb_user_id**: group id/fans page id/account id.
@@ -149,8 +170,8 @@
 
 
 ```python
 
 ## To-Do
 
 - Collect profile info
-- Collect image info
+- Collect image info
```

### Comparing `facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 0.8
+Version: 0.9
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/facebook_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -34,44 +34,50 @@
 You can choose between two methods to collect user posts data. 
 
 - **Log in with your account credentials**: login facebook account
 - **Without logging in**: Without logging in, click the X icon to 
 - **Difference**: The difference between these two methods is that for some personal accounts, you cannot browse the user's posts without logging into a Facebook account.
 
 ```python
-from facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
-from dotenv import load_dotenv
+# -*- coding: utf-8 -*-
 import os
+from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
+from dotenv import load_dotenv
 
 
-## Load account info
-load_dotenv()
-username_or_userid = os.getenv("FB_USERNAME_OR_USERID")
+# ## Load account info
+# load_dotenv()
+fb_account = os.getenv("FBACCOUNT") # Facebook帳號密碼
 pwd = os.getenv("FBPASSWORD")
 
-#%%
-## Log in account version
+# ## Log in account version
 fb_user_id = "KaiCenatOfficial"
+driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
-    username_or_userid=username_or_userid,
+    driver_path=driver_path,
+    fb_account=fb_account,
     pwd=pwd
 )
 res
-#%%
+
 ## Without logging in account version
 fb_user_id = "KaiCenatOfficial"
+driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
-    loop_times=50
+    loop_times=50,
+    driver_path=driver_path,
 )
 res
+# %%
+
 
 
 
 ```
 ### Optional parameters
 
 - **fb_user_id**: group id/fans page id/account id.
```

### Comparing `facebook-graphql-scraper-0.8/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-0.9/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.8/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-0.9/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.8/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-0.9/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 from fb_graphql_scraper.utils.locator import *
 from fb_graphql_scraper.utils.utils import *
 from fb_graphql_scraper.utils.parser import RequestsParser
 from tqdm import tqdm, trange
 
 
 class FacebookSettings:
-    def __init__(self,url,username_or_userid:str=None,pwd:str=None,driver_path:str=None):
+    def __init__(self,url,fb_account:str=None,pwd:str=None,driver_path:str=None):
         super().__init__()
-        self.username_or_userid = username_or_userid
+        self.fb_account = fb_account
         self.pwd = pwd
         self.url=url
         self.set_spider(driver_path=driver_path)
         self.set_container()
     
     def set_spider(self, driver_path):
         """>> Description: Auto login account or click "X" button to continue, 
         but some account can't not be display info if you don't login account
         >> Args: url (_str_): target user which you want to collect data."""
         self.base_page = BasePage(driver_path=driver_path)
         self.page_optional = PageOptional(
             url_in=self.url, 
             driver=self.base_page.driver,
-            username_or_userid=self.username_or_userid,
+            fb_account=self.fb_account,
             pwd=self.pwd
         )
         time.sleep(5)
         self.requests_parser = RequestsParser(driver=self.page_optional.driver)
         
     def set_container(self):
         self.post_id_list = []
@@ -43,16 +43,16 @@
             "post_likes": [],
             "comment_share_type": [],
             "comment_share_value": []
         }
 
 
 class FacebookGraphqlScraper(FacebookSettings):
-    def __init__(self,url="https://www.facebook.com/",username_or_userid:str=None, pwd:str=None):
-        super().__init__(url=url, username_or_userid=username_or_userid, pwd=pwd)
+    def __init__(self,url="https://www.facebook.com/",fb_account:str=None, pwd:str=None):
+        super().__init__(url=url, fb_account=fb_account, pwd=pwd)
 
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
-    def get_user_posts(cls, fb_username_or_userid:str, loop_times:int=50, username_or_userid:str=None, pwd:str=None):
+    def get_user_posts(cls, fb_username_or_userid:str, loop_times:int=50, fb_account:str=None, pwd:str=None):
         url = "https://www.facebook.com/"+fb_username_or_userid
-        spider = cls(url=url,username_or_userid=username_or_userid,pwd=pwd)
+        spider = cls(url=url,fb_account=fb_account,pwd=pwd)
         # Scroll page
         for round in tqdm(range(loop_times)): # 滾動次數
             spider.page_optional.scroll_window()
             spider.pause()
 
         # Collect data
         driver_requests = spider.page_optional.driver.requests
```

### Comparing `facebook-graphql-scraper-0.8/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-0.9/fb_graphql_scraper/pages/page_optional.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.keys import Keys
 import time
 
 
 class PageOptional(object):
-    def __init__(self, url_in: str, driver=None, username_or_userid: str = None, pwd: str = None):
+    def __init__(self, url_in: str, driver=None, fb_account: str = None, pwd: str = None):
         self.locator = PageLocators
         self.xpath_elements = PageXpath
         self.class_elements = PageClass
         self.page_text = PageText
         self.driver = driver
         self.url = url_in
         self.driver.get(url=self.url)
-        self.username_or_userid = username_or_userid
+        self.fb_account = fb_account
         self.pwd = pwd
         time.sleep(3)
 
         # Loggin account
-        if self.username_or_userid and self.pwd:
+        if self.fb_account and self.pwd:
             self.login_page()
 
         # 免登入帳號, 適用不需登入帳號的爬蟲目標 / Without logging, click X button
         else:
             self.click_reject_login_button()
 
     def login_page(self):
         try:
-            self.login_account(user=self.username_or_userid, password=self.pwd,
+            self.login_account(user=self.fb_account, password=self.pwd,
                                user_element=self.locator.LOGGINUSR1, pwd_element=self.locator.LOGGINPWD1)
         except:
-            self.login_account(user=self.username_or_userid, password=self.pwd,
+            self.login_account(user=self.fb_account, password=self.pwd,
                                user_element=self.locator.LOGGINUSR2, pwd_element=self.locator.LOGGINPWD2)
 
     def clean_requests(self):
         try:
             print("Try to clear driver requests..")
             del self.driver.requests
             print("Clear")
```

### Comparing `facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/parser.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.8/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-0.9/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-0.8/setup.py` & `facebook-graphql-scraper-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='0.8',
+    version='0.9',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
         "fb_graphql_scraper.resources"
```

