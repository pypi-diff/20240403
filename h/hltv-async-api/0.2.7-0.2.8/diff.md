# Comparing `tmp/hltv_async_api-0.2.7.tar.gz` & `tmp/hltv_async_api-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.2.7.tar", last modified: Tue Apr  2 21:03:23 2024, max compression
+gzip compressed data, was "hltv_async_api-0.2.8.tar", last modified: Tue Apr  2 22:42:18 2024, max compression
```

## Comparing `hltv_async_api-0.2.7.tar` & `hltv_async_api-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 21:03:23.127077 hltv_async_api-0.2.7/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     4887 2024-04-02 21:03:23.125095 hltv_async_api-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4264 2024-04-02 21:01:52.000000 hltv_async_api-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 21:03:23.080078 hltv_async_api-0.2.7/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-02 16:33:09.000000 hltv_async_api-0.2.7/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    28348 2024-04-02 21:00:56.000000 hltv_async_api-0.2.7/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:03:23.124075 hltv_async_api-0.2.7/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     4887 2024-04-02 21:03:22.000000 hltv_async_api-0.2.7/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-02 21:03:22.000000 hltv_async_api-0.2.7/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 21:03:22.000000 hltv_async_api-0.2.7/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 21:03:22.000000 hltv_async_api-0.2.7/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-02 21:03:16.000000 hltv_async_api-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 21:03:23.128086 hltv_async_api-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-02 21:03:16.000000 hltv_async_api-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:42:18.346463 hltv_async_api-0.2.8/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     4887 2024-04-02 22:42:18.345479 hltv_async_api-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4264 2024-04-02 21:01:52.000000 hltv_async_api-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 22:42:18.297070 hltv_async_api-0.2.8/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-02 22:42:16.000000 hltv_async_api-0.2.8/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    28423 2024-04-02 22:41:21.000000 hltv_async_api-0.2.8/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:42:18.344466 hltv_async_api-0.2.8/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     4887 2024-04-02 22:42:18.000000 hltv_async_api-0.2.8/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-02 22:42:18.000000 hltv_async_api-0.2.8/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:42:18.000000 hltv_async_api-0.2.8/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-02 22:42:18.000000 hltv_async_api-0.2.8/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-02 22:42:16.000000 hltv_async_api-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 22:42:18.347464 hltv_async_api-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-04-02 22:42:16.000000 hltv_async_api-0.2.8/setup.py
```

### Comparing `hltv_async_api-0.2.7/LICENSE` & `hltv_async_api-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.2.7/PKG-INFO` & `hltv_async_api-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.2.7
+Version: 0.2.8
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.2.7/README.md` & `hltv_async_api-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.2.7/hltv_async_api/aiohltv.py` & `hltv_async_api-0.2.8/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, List
 from datetime import date, datetime, timedelta
 import pytz
-
+import aiofiles
 from bs4 import BeautifulSoup
 import asyncio
 from asyncio import get_running_loop
 from functools import partial
 
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientProxyConnectionError, ClientResponseError, ClientOSError, \
@@ -72,42 +72,42 @@
             self.PROXY_PROTOCOL = proxy_protocol
         if remove_proxy:
             self.REMOVE_PROXY = remove_proxy
         if debug:
             self.DEBUG = debug
             self._configure_logging()
 
-    def get_proxy(self):
+    async def get_proxy(self):
         proxy = ''
         if self.PROXY_PATH:
-            with open(self.PROXY_PATH, "r") as file:
-                new_proxy = file.readline().strip()
+            async with aiofiles.open(self.PROXY_PATH, "r") as file:
+                new_proxy = await file.readline().strip()
                 if new_proxy:
                     proxy = new_proxy
 
         else:
             proxy = self.PROXY_LIST[0]
 
         if self.PROXY_PROTOCOL and proxy != '' and self.PROXY_PROTOCOL not in proxy:
-       	    proxy = self.PROXY_PROTOCOL + '://' + proxy
+            proxy = self.PROXY_PROTOCOL + '://' + proxy
 
         return proxy
 
     async def switch_proxy(self, proxy):
         if self.PROXY_PATH:
             if self.PROXY_PROTOCOL:
                 proxy = proxy.replace(self.PROXY_PROTOCOL + '://', '')
-            with open(self.PROXY_PATH, "r+") as file:
-                proxies = file.readlines()
-                file.seek(0)
+            async with aiofiles.open(self.PROXY_PATH, "r+") as file:
+                proxies = await file.readlines()
+                await file.seek(0)
                 for line in proxies:
                     if line.strip() != proxy:
-                        file.write(line)
+                        await file.write(line)
                 if not self.REMOVE_PROXY:
-                    file.write(proxy + "\n")
+                    await file.write(proxy + "\n")
         else:
             self.PROXY_LIST = self.PROXY_LIST[1:] + [self.PROXY_LIST[0]]
 
     def f(self, result):
         return BeautifulSoup(result, "lxml")
 
     async def cloudflare_check(self, result) -> bool:
@@ -119,29 +119,29 @@
                 return True
         return False
 
     async def parse_error_handler(self, proxy, delay: int = 0) -> int:
         if self.USE_PROXY:
             self.logger.debug(f"Switching proxy {proxy}")
             await self.switch_proxy(proxy)
-            self.logger.info(f"New proxy: {self.get_proxy()}")
+            self.logger.info(f"New proxy: {await self.get_proxy()}")
         else:
             if delay < self.MAX_DELAY:
                 delay += 1
             else:
                 self.logger.debug("Reached max delay limit, try to use proxy")
             self.logger.info(f"Calling again, increasing delay to {delay}s")
 
         return delay
 
     async def parse(self, session, url, delay):
         proxy = ''
         # setup new proxy, cuz old one was switched
         if self.USE_PROXY:
-            proxy = self.get_proxy()
+            proxy = await self.get_proxy()
         else:
             # delay, only for non proxy users. (default = 1-15s)
             await asyncio.sleep(delay)
         try:
             async with session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout, ) as response:
                 self.logger.info(f"Fetching {url}, code: {response.status}")
                 if response.status == 403 or response.status == 404:
@@ -629,15 +629,14 @@
                 if rank > top:
                     break
         except AttributeError:
             raise AttributeError("Top players parsing error, probably page not fully loaded")
 
         return players
 
-    # TODO WRITE
     async def get_last_news(self, max_reg_news=2, only_today=True, only_featured=False):
         r = await self.fetch('https://www.hltv.org/')
 
         today = datetime.now(tz=pytz.timezone('Europe/Copenhagen'))
         article_days = {
             1: today.strftime('%d-%m'),
             2: (today - timedelta(days=1)).strftime('%d-%m'),
```

### Comparing `hltv_async_api-0.2.7/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.2.8/hltv_async_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.2.7
+Version: 0.2.8
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.2.7/pyproject.toml` & `hltv_async_api-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.2.7/setup.py` & `hltv_async_api-0.2.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.2.7',
+    version='0.2.8',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

