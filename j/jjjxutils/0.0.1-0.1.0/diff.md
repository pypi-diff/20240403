# Comparing `tmp/jjjxutils-0.0.1.tar.gz` & `tmp/jjjxutils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "jjjxutils-0.1.0.tar", max compression
```

## Comparing `jjjxutils-0.0.1.tar` & `jjjxutils-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/src/jjjxutils/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/src/jjjxutils/imports.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/src/jjjxutils/archive/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/src/jjjxutils/archive/zip.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/src/jjjxutils/rendering/__init__.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/src/jjjxutils/rendering/html.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/src/jjjxutils/web/__init__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/src/jjjxutils/web/browser_client.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/tests/generate_pdf.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/tests/generate_png.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jjjxutils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-04-03 18:47:30.321170 jjjxutils-0.1.0/jjjxutils/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-03 18:47:30.323170 jjjxutils-0.1.0/jjjxutils/archive/__init__.py
+-rw-r--r--   0        0        0      524 2024-04-03 18:47:30.323170 jjjxutils-0.1.0/jjjxutils/archive/zip.py
+-rw-r--r--   0        0        0     1611 2024-04-03 19:05:31.202048 jjjxutils-0.1.0/jjjxutils/decorators.py
+-rw-r--r--   0        0        0     1207 2024-04-03 18:47:30.324170 jjjxutils-0.1.0/jjjxutils/imports.py
+-rw-r--r--   0        0        0       18 2024-04-03 18:47:30.325170 jjjxutils-0.1.0/jjjxutils/rendering/__init__.py
+-rw-r--r--   0        0        0     1523 2024-04-03 18:49:20.746411 jjjxutils-0.1.0/jjjxutils/rendering/html.py
+-rw-r--r--   0        0        0       28 2024-04-03 18:47:30.327170 jjjxutils-0.1.0/jjjxutils/web/__init__.py
+-rw-r--r--   0        0        0     2142 2024-04-03 18:47:30.328170 jjjxutils-0.1.0/jjjxutils/web/browser_client.py
+-rw-r--r--   0        0        0     1093 2024-04-03 18:47:30.318170 jjjxutils-0.1.0/LICENSE
+-rw-r--r--   0        0        0      303 2024-04-03 19:06:23.477752 jjjxutils-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      580 2024-04-03 19:09:19.424558 jjjxutils-0.1.0/README.md
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 jjjxutils-0.1.0/PKG-INFO
```

### Comparing `jjjxutils-0.0.1/src/jjjxutils/rendering/html.py` & `jjjxutils-0.1.0/jjjxutils/rendering/html.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,43 @@
-import base64
-import os
-import shutil
-import requests
-import zipfile
-import io
-import platform
-import json
-from urllib.parse import parse_qs
-
-from ..web.browser_client import BrowserClient
-
-
-class HtmlRenderer:
-    def __init__(self, browser_client: BrowserClient):
-        self.browser_client = browser_client
-        self.driver = browser_client.driver
-
-    def save_current_pdf(self, dest, landscape=False):
-        resource = "/session/%s/chromium/send_command_and_get_result" % self.driver.session_id
-        url = self.driver.command_executor._url + resource
-        body = json.dumps(
-            {
-                "cmd": "Page.printToPDF",
-                "params": {
-                    "landscape": landscape,
-                    "displayHeaderFooter": False,
-                    "printBackground": True,
-                    "preferCSSPageSize": False,
-                },
-            }
-        )
-        response = self.driver.command_executor._request("POST", url, body)
-        with open(dest, "wb") as file:
-            file.write(base64.b64decode(response.get("value")["data"]))
-
-    def save_current_png(self, dest, landscape=False):
-        if landscape:
-            self.driver.set_window_size(1414, 1000)
-        else:
-            self.driver.set_window_size(1000, 1414)
-        self.driver.save_screenshot(dest)
-
-    def save_as_pdf(self, uri, dest, landscape=False):
-        self.driver.get(uri)
-        self.save_current_pdf(dest, landscape)
-
-    def save_as_png(self, uri, dest, landscape=False):
-        self.driver.get(uri)
-        self.save_current_png(dest, landscape)
+import base64
+import json
+
+from ..web.browser_client import BrowserClient
+
+
+class HtmlRenderer:
+    def __init__(self, browser_client: BrowserClient):
+        self.browser_client = browser_client
+        self.driver = browser_client.driver
+
+    def save_current_pdf(self, dest, landscape=False):
+        resource = "/session/%s/chromium/send_command_and_get_result" % self.driver.session_id
+        url = self.driver.command_executor._url + resource
+        body = json.dumps(
+            {
+                "cmd": "Page.printToPDF",
+                "params": {
+                    "landscape": landscape,
+                    "displayHeaderFooter": False,
+                    "printBackground": True,
+                    "preferCSSPageSize": False,
+                },
+            }
+        )
+        response = self.driver.command_executor._request("POST", url, body)
+        with open(dest, "wb") as file:
+            file.write(base64.b64decode(response.get("value")["data"]))
+
+    def save_current_png(self, dest, landscape=False):
+        if landscape:
+            self.driver.set_window_size(1414, 1000)
+        else:
+            self.driver.set_window_size(1000, 1414)
+        self.driver.save_screenshot(dest)
+
+    def save_as_pdf(self, uri, dest, landscape=False):
+        self.driver.get(uri)
+        self.save_current_pdf(dest, landscape)
+
+    def save_as_png(self, uri, dest, landscape=False):
+        self.driver.get(uri)
+        self.save_current_png(dest, landscape)
```

### Comparing `jjjxutils-0.0.1/src/jjjxutils/web/browser_client.py` & `jjjxutils-0.1.0/jjjxutils/web/browser_client.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import requests
-import platform
-
-from ..archive.zip import extract_ignoring_folders
-from ..imports import import_rel
-
-class BrowserClient:
-    driver = None
-    selenium = None
-
-    def __init__(self):
-        raise NotImplementedError
-
-
-class ChromeClient(BrowserClient):
-    def __init__(self, selenium):
-        self.selenium = selenium
-        self.download_chromedriver()
-        options = self.selenium.webdriver.chrome.options.Options()
-        options.add_argument("--headless")
-        options.add_argument("--disable-gpu")
-        options.add_argument("--no-sandbox")
-        options.add_argument("--disable-dev-shm-usage")
-        self.driver = self.selenium.webdriver.Chrome(options=options)
-
-    def download_chromedriver(self):
-        chrome_version_data = requests.get(
-            "https://googlechromelabs.github.io/chrome-for-testing/last-known-good-versions-with-downloads.json",
-            timeout=30
-        ).json()
-        stable_chromedriver_downloads = chrome_version_data["channels"]["Stable"][
-            "downloads"
-        ]["chromedriver"]
-
-        system = platform.system()
-        if system == "Linux":
-            found_platform = "linux64"
-        elif system == "Darwin":
-            found_platform = "mac-x64"
-        elif system == "Windows":
-            if "64bit" in platform.architecture():
-                found_platform = "win64"
-            else:
-                found_platform = "win32"
-        else:
-            raise NotImplementedError(f"Unsupported platform {system}")
-
-        for possible_donwload in stable_chromedriver_downloads:
-            if possible_donwload["platform"] == found_platform:
-                chromedriver_download = possible_donwload
-                break
-        else:
-            raise FileNotFoundError(
-                f"Could not find chromedriver for {found_platform}")
-
-        chromedriver_zip = requests.get(
-            chromedriver_download["url"], timeout=30)
-
-        return extract_ignoring_folders(chromedriver_zip.content)
-
-
-def get_selenium():
-    return import_rel("selenium.webdriver")
+import requests
+import platform
+
+from ..archive.zip import extract_ignoring_folders
+from ..imports import import_rel
+
+class BrowserClient:
+    driver = None
+    selenium = None
+
+    def __init__(self):
+        raise NotImplementedError
+
+
+class ChromeClient(BrowserClient):
+    def __init__(self, selenium):
+        self.selenium = selenium
+        self.download_chromedriver()
+        options = self.selenium.webdriver.chrome.options.Options()
+        options.add_argument("--headless")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-dev-shm-usage")
+        self.driver = self.selenium.webdriver.Chrome(options=options)
+
+    def download_chromedriver(self):
+        chrome_version_data = requests.get(
+            "https://googlechromelabs.github.io/chrome-for-testing/last-known-good-versions-with-downloads.json",
+            timeout=30
+        ).json()
+        stable_chromedriver_downloads = chrome_version_data["channels"]["Stable"][
+            "downloads"
+        ]["chromedriver"]
+
+        system = platform.system()
+        if system == "Linux":
+            found_platform = "linux64"
+        elif system == "Darwin":
+            found_platform = "mac-x64"
+        elif system == "Windows":
+            if "64bit" in platform.architecture():
+                found_platform = "win64"
+            else:
+                found_platform = "win32"
+        else:
+            raise NotImplementedError(f"Unsupported platform {system}")
+
+        for possible_donwload in stable_chromedriver_downloads:
+            if possible_donwload["platform"] == found_platform:
+                chromedriver_download = possible_donwload
+                break
+        else:
+            raise FileNotFoundError(
+                f"Could not find chromedriver for {found_platform}")
+
+        chromedriver_zip = requests.get(
+            chromedriver_download["url"], timeout=30)
+
+        return extract_ignoring_folders(chromedriver_zip.content)
+
+
+def get_selenium():
+    return import_rel("selenium.webdriver")
```

### Comparing `jjjxutils-0.0.1/LICENSE` & `jjjxutils-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Johannes Hartel
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Johannes Hartel
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

