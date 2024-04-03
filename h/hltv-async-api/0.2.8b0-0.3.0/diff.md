# Comparing `tmp/hltv_async_api-0.2.8b0.tar.gz` & `tmp/hltv_async_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.2.8b0.tar", last modified: Tue Apr  2 22:44:05 2024, max compression
+gzip compressed data, was "hltv_async_api-0.3.0.tar", last modified: Wed Apr  3 12:58:03 2024, max compression
```

## Comparing `hltv_async_api-0.2.8b0.tar` & `hltv_async_api-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 22:44:05.307439 hltv_async_api-0.2.8b0/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.8b0/LICENSE
--rw-rw-rw-   0        0        0     4889 2024-04-02 22:44:05.306444 hltv_async_api-0.2.8b0/PKG-INFO
--rw-rw-rw-   0        0        0     4264 2024-04-02 21:01:52.000000 hltv_async_api-0.2.8b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 22:44:05.277444 hltv_async_api-0.2.8b0/hltv_async_api/
--rw-rw-rw-   0        0        0      125 2024-04-02 22:43:58.000000 hltv_async_api-0.2.8b0/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    28423 2024-04-02 22:41:21.000000 hltv_async_api-0.2.8b0/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:44:05.305444 hltv_async_api-0.2.8b0/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     4889 2024-04-02 22:44:05.000000 hltv_async_api-0.2.8b0/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-02 22:44:05.000000 hltv_async_api-0.2.8b0/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 22:44:05.000000 hltv_async_api-0.2.8b0/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 22:44:05.000000 hltv_async_api-0.2.8b0/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      538 2024-04-02 22:43:58.000000 hltv_async_api-0.2.8b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 22:44:05.308440 hltv_async_api-0.2.8b0/setup.cfg
--rw-rw-rw-   0        0        0      952 2024-04-02 22:43:58.000000 hltv_async_api-0.2.8b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:58:03.723019 hltv_async_api-0.3.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4887 2024-04-03 12:58:03.722016 hltv_async_api-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4264 2024-04-02 21:01:52.000000 hltv_async_api-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 12:58:03.693014 hltv_async_api-0.3.0/hltv_async_api/
+-rw-rw-rw-   0        0        0      125 2024-04-02 22:43:58.000000 hltv_async_api-0.3.0/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    28125 2024-04-03 12:56:34.000000 hltv_async_api-0.3.0/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:58:03.720022 hltv_async_api-0.3.0/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     4887 2024-04-03 12:58:03.000000 hltv_async_api-0.3.0/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-03 12:58:03.000000 hltv_async_api-0.3.0/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:58:03.000000 hltv_async_api-0.3.0/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-03 12:58:03.000000 hltv_async_api-0.3.0/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-03 12:57:58.000000 hltv_async_api-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 12:58:03.724017 hltv_async_api-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      951 2024-04-03 12:57:58.000000 hltv_async_api-0.3.0/setup.py
```

### Comparing `hltv_async_api-0.2.8b0/LICENSE` & `hltv_async_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.2.8b0/PKG-INFO` & `hltv_async_api-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.2.8b0
+Version: 0.3.0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.2.8b0/README.md` & `hltv_async_api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.2.8b0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.3.0/hltv_async_api/aiohltv.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,18 @@
         self.PROXY_LIST = proxy_list
         self.PROXY_PROTOCOL = proxy_protocol
         self.REMOVE_PROXY = remove_proxy
         self.DEBUG = debug
         self._configure_logging()
         self.logger = logging.getLogger(__name__)
 
+        if self.PROXY_PATH:
+            with open(self.PROXY_PATH, "r") as file:
+                self.PROXY_LIST = [line.strip() for line in file.readlines()]
+
     def _configure_logging(self):
         level = logging.DEBUG if self.DEBUG else logging.INFO
         logging.basicConfig(level=level, format="%(message)s")
 
     def config(self, max_delay: int | None = None,
                timeout: int | None = None,
                use_proxy: bool | None = None,
@@ -58,58 +62,45 @@
                ):
         if max_delay:
             self.MAX_DELAY = max_delay
         if timeout:
             self.timeout = timeout
         if use_proxy:
             self.USE_PROXY = use_proxy
-        if proxy_file_path:
-            self.PROXY_PATH = proxy_file_path
         if proxy_list:
             self.PROXY_LIST = proxy_list
         if max_retries:
             self.max_retries = max_retries
         if proxy_protocol:
             self.PROXY_PROTOCOL = proxy_protocol
         if remove_proxy:
             self.REMOVE_PROXY = remove_proxy
         if debug:
             self.DEBUG = debug
             self._configure_logging()
+        if proxy_file_path:
+            with open(self.PROXY_PATH, "r") as file:
+                self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
     async def get_proxy(self):
-        proxy = ''
-        if self.PROXY_PATH:
-            async with aiofiles.open(self.PROXY_PATH, "r") as file:
-                new_proxy = await file.readline().strip()
-                if new_proxy:
-                    proxy = new_proxy
-
-        else:
-            proxy = self.PROXY_LIST[0]
+        proxy = self.PROXY_LIST[0]
 
         if self.PROXY_PROTOCOL and proxy != '' and self.PROXY_PROTOCOL not in proxy:
             proxy = self.PROXY_PROTOCOL + '://' + proxy
 
         return proxy
 
-    async def switch_proxy(self, proxy):
-        if self.PROXY_PATH:
-            if self.PROXY_PROTOCOL:
-                proxy = proxy.replace(self.PROXY_PROTOCOL + '://', '')
-            async with aiofiles.open(self.PROXY_PATH, "r+") as file:
-                proxies = await file.readlines()
-                await file.seek(0)
-                for line in proxies:
-                    if line.strip() != proxy:
-                        await file.write(line)
-                if not self.REMOVE_PROXY:
-                    await file.write(proxy + "\n")
+    async def switch_proxy(self):
+        if self.REMOVE_PROXY:
+            self.logger.debug(f'Removing proxy {self.PROXY_LIST[0]}')
+            self.PROXY_LIST = self.PROXY_LIST[1:]
         else:
-            self.PROXY_LIST = self.PROXY_LIST[1:] + [self.PROXY_LIST[0]]
+            self.logger.debug(f"Switching proxy {self.PROXY_LIST[0]}")
+            self.PROXY_LIST = self.PROXY_LIST[1:] + self.PROXY_LIST[0]
+            self.logger.info(f"New proxy: {self.PROXY_LIST[0]}")
 
     def f(self, result):
         return BeautifulSoup(result, "lxml")
 
     async def cloudflare_check(self, result) -> bool:
         page = self.f(result)
         challenge_page = page.find(id="challenge-error-title")
@@ -117,17 +108,15 @@
             if "Enable JavaScript and cookies to continue" in challenge_page.get_text():
                 self.logger.debug("Got cloudflare challange page")
                 return True
         return False
 
     async def parse_error_handler(self, proxy, delay: int = 0) -> int:
         if self.USE_PROXY:
-            self.logger.debug(f"Switching proxy {proxy}")
-            await self.switch_proxy(proxy)
-            self.logger.info(f"New proxy: {await self.get_proxy()}")
+            await self.switch_proxy()
         else:
             if delay < self.MAX_DELAY:
                 delay += 1
             else:
                 self.logger.debug("Reached max delay limit, try to use proxy")
             self.logger.info(f"Calling again, increasing delay to {delay}s")
 
@@ -685,13 +674,13 @@
             if only_today:
                 break
 
         return news
 
 
 async def test():
-    hltv = Hltv()
+    hltv = Hltv(use_proxy=True, proxy_path='proxies.txt', debug=True, remove_proxy=True, proxy_protocol='http')
     print(await hltv.get_last_news(only_today=True, max_reg_news=1))
 
 
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.2.8b0/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.3.0/hltv_async_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.2.8b0
+Version: 0.3.0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.2.8b0/pyproject.toml` & `hltv_async_api-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.2.8b"
+version = "0.3.0"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.2.8b0/setup.py` & `hltv_async_api-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.2.8b',
+    version='0.3.0',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

