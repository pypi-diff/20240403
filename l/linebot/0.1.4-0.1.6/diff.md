# Comparing `tmp/linebot-0.1.4.tar.gz` & `tmp/linebot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linebot-0.1.4.tar", last modified: Wed Apr  3 09:21:27 2024, max compression
+gzip compressed data, was "linebot-0.1.6.tar", last modified: Thu Mar 21 06:04:24 2024, max compression
```

## Comparing `linebot-0.1.4.tar` & `linebot-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 09:21:27.526565 linebot-0.1.4/
--rw-rw-rw-   0        0        0     1077 2024-04-02 09:34:47.000000 linebot-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-02 09:34:47.000000 linebot-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1602 2024-04-03 09:21:27.525562 linebot-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      902 2024-04-02 09:34:47.000000 linebot-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 09:21:27.517159 linebot-0.1.4/line/
--rw-rw-rw-   0        0        0       22 2024-04-02 09:34:47.000000 linebot-0.1.4/line/__init__.py
--rw-rw-rw-   0        0        0     5465 2024-04-03 03:03:50.000000 linebot-0.1.4/line/authentications.py
--rw-rw-rw-   0        0        0    33222 2024-04-03 09:07:35.000000 linebot-0.1.4/line/core.py
--rw-rw-rw-   0        0        0      215 2024-04-03 03:11:50.000000 linebot-0.1.4/line/exceptions.py
--rw-rw-rw-   0        0        0      223 2024-04-03 08:52:24.000000 linebot-0.1.4/line/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:21:27.524275 linebot-0.1.4/linebot.egg-info/
--rw-rw-rw-   0        0        0     1602 2024-04-03 09:21:27.000000 linebot-0.1.4/linebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-03 09:21:27.000000 linebot-0.1.4/linebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 09:21:27.000000 linebot-0.1.4/linebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-03 09:21:27.000000 linebot-0.1.4/linebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-03 09:21:27.000000 linebot-0.1.4/linebot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 09:21:27.526565 linebot-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-03 08:52:24.000000 linebot-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-21 06:04:24.617132 linebot-0.1.6/
+-rw-rw-rw-   0        0        0     1077 2024-03-13 09:39:12.000000 linebot-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-03-21 03:51:46.000000 linebot-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1537 2024-03-21 06:04:24.617132 linebot-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2024-03-21 05:55:11.000000 linebot-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-03-21 06:04:24.600397 linebot-0.1.6/line/
+-rw-rw-rw-   0        0        0       22 2024-03-21 03:42:22.000000 linebot-0.1.6/line/__init__.py
+-rw-rw-rw-   0        0        0     4814 2024-03-21 05:49:13.000000 linebot-0.1.6/line/authentications.py
+-rw-rw-rw-   0        0        0    22668 2023-11-21 08:01:32.000000 linebot-0.1.6/line/core.py
+-rw-rw-rw-   0        0        0      156 2023-10-24 10:47:16.000000 linebot-0.1.6/line/exceptions.py
+-rw-rw-rw-   0        0        0      224 2023-10-30 02:12:32.000000 linebot-0.1.6/line/logger.py
+drwxrwxrwx   0        0        0        0 2024-03-21 06:04:24.616130 linebot-0.1.6/linebot.egg-info/
+-rw-rw-rw-   0        0        0     1537 2024-03-21 06:04:24.000000 linebot-0.1.6/linebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-03-21 06:04:24.000000 linebot-0.1.6/linebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-21 06:04:24.000000 linebot-0.1.6/linebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-03-21 06:04:24.000000 linebot-0.1.6/linebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-03-21 06:04:24.000000 linebot-0.1.6/linebot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-21 06:04:24.617132 linebot-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-03-21 06:03:35.000000 linebot-0.1.6/setup.py
```

### Comparing `linebot-0.1.4/LICENSE` & `linebot-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linebot-0.1.4/PKG-INFO` & `linebot-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: linebot
-Version: 0.1.4
+Version: 0.1.6
 Summary: Line chatbot framework.
 Home-page: https://github.com/miloira/line-bot
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: loguru
-Requires-Dist: pyee
 
 
-linebot
+line-bot
 ===============================================
 Line chatbot framework.
 
 Usage
 -----
 
 ```bash
-$ pip install linebot
+$ pip install line-bot
 ```
 
 
 ```python
 from line import Line
 from line.authentications import BusinessAuthentication
 
@@ -61,10 +58,10 @@
 ```
 
 
 Meta
 ----
 
 
-Distributed under the MIT license. See `LICENSE <https://github.com/miloira/linebot/LICENSE>` for more information.
+Distributed under the MIT license. See `LICENSE <https://github.com/miloira/line-bot/LICENSE>` for more information.
 
-https://github.com/miloira/linebot
+https://github.com/miloira/line-bot
```

### Comparing `linebot-0.1.4/README.md` & `linebot-0.1.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-linebot
+line-bot
 ===============================================
 Line chatbot framework.
 
 Usage
 -----
 
 ```bash
-$ pip install linebot
+$ pip install line-bot
 ```
 
 
 ```python
 from line import Line
 from line.authentications import BusinessAuthentication
 
@@ -39,10 +39,10 @@
 ```
 
 
 Meta
 ----
 
 
-Distributed under the MIT license. See `LICENSE <https://github.com/miloira/linebot/LICENSE>` for more information.
+Distributed under the MIT license. See `LICENSE <https://github.com/miloira/line-bot/LICENSE>` for more information.
 
-https://github.com/miloira/linebot
+https://github.com/miloira/line-bot
```

### Comparing `linebot-0.1.4/line/authentications.py` & `linebot-0.1.6/line/authentications.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import os
 from pathlib import Path
 
 import requests
 
-class Authentication:
-
-    def login(self):
-        raise NotImplementedError
 
-
-class CookieAuthentication(Authentication):
+class CookieAuthentication:
 
     def __init__(self, cookies):
         self.cookies = cookies
 
     @classmethod
     def cookie_str_to_dict(cls, cookie_str):
         cookie_dict = {}
@@ -26,19 +21,16 @@
     def login(self):
         cookies = self.cookie_str_to_dict(self.cookies)
         return {
             "ses": cookies["ses"],
             "xsrf_token": cookies["XSRF-TOKEN"]
         }
 
-    def __str__(self):
-        return f"<CookieAuthentication(cookies=\"{self.cookies}\")>"
-
 
-class BusinessAuthentication(Authentication):
+class BusinessAuthentication:
 
     def __init__(self, username, password):
         self.username = username
         self.password = password
 
     @classmethod
     def get_login_cookies(cls):
@@ -76,19 +68,16 @@
         }
         response = session.post(url, headers=headers, cookies=cookies, json=data)
         return {
             "ses": session.cookies["ses"],
             "xsrf_token": self.csrf_token(session)["token"]
         }
 
-    def __str__(self):
-        return f"<BusinessAuthentication(username=\"{self.username}\",password=\"{self.password}\")>"
 
-
-class PersonQRCodeAuthentication(Authentication):
+class PersonQRCodeAuthentication:
 
     def __init__(self, qrcode_path=None):
         if qrcode_path is None:
             self.qrcode_path = '.'
         else:
             self.qrcode_path = qrcode_path
 
@@ -140,38 +129,32 @@
         self.qr_wait(qr_ses)
 
         return {
             "ses": "",
             "xsrf_token": ""
         }
 
-    def __str__(self):
-        return f"<PersonQRCodeAuthentication(qrcode_path=\"{self.qrcode_path}\")>"
-
 
-class BrowserAuthentication(Authentication):
+class BrowserAuthentication:
 
     def __init__(self, page):
         self.page = page
         self.page.goto("https://manager.line.biz/")
 
         while self.page.url.startswith("https://account.line.biz") or self.page.url.startswith(
                 "https://access.line.me"):
             self.page.wait_for_timeout(1 * 1000)
 
         self.cookies = {item["name"]: item["value"] for item in self.page.context.cookies()}
-        self.csrf_token = self.get_csrf_token()
 
-    def get_csrf_token(self):
+    @property
+    def csrf_token(self):
         url = "https://chat.line.biz/api/v1/csrfToken"
         response = requests.get(url, cookies=self.cookies)
         return response.json()
 
     def login(self):
         data = {
             "ses": self.cookies["ses"],
             "xsrf_token": self.csrf_token["token"]
         }
         return data
-
-    def __str__(self):
-        return f"<BrowserAuthentication(cookies=\"{self.cookies}\",csrf_token=\"{self.csrf_token}\")>"
```

### Comparing `linebot-0.1.4/linebot.egg-info/PKG-INFO` & `linebot-0.1.6/linebot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: linebot
-Version: 0.1.4
+Version: 0.1.6
 Summary: Line chatbot framework.
 Home-page: https://github.com/miloira/line-bot
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: loguru
-Requires-Dist: pyee
 
 
-linebot
+line-bot
 ===============================================
 Line chatbot framework.
 
 Usage
 -----
 
 ```bash
-$ pip install linebot
+$ pip install line-bot
 ```
 
 
 ```python
 from line import Line
 from line.authentications import BusinessAuthentication
 
@@ -61,10 +58,10 @@
 ```
 
 
 Meta
 ----
 
 
-Distributed under the MIT license. See `LICENSE <https://github.com/miloira/linebot/LICENSE>` for more information.
+Distributed under the MIT license. See `LICENSE <https://github.com/miloira/line-bot/LICENSE>` for more information.
 
-https://github.com/miloira/linebot
+https://github.com/miloira/line-bot
```

### Comparing `linebot-0.1.4/setup.py` & `linebot-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'linebot'
 DESCRIPTION = 'Line chatbot framework.'
 URL = 'https://github.com/miloira/line-bot'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.4'
+VERSION = '0.1.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'loguru',
     'pyee'
 ]
```

