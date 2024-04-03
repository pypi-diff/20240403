# Comparing `tmp/pinterest-dl-0.0.17.tar.gz` & `tmp/pinterest-dl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinterest-dl-0.0.17.tar", last modified: Wed Apr  3 13:41:38 2024, max compression
+gzip compressed data, was "pinterest-dl-0.0.9.tar", last modified: Sun Mar 31 15:03:09 2024, max compression
```

## Comparing `pinterest-dl-0.0.17.tar` & `pinterest-dl-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:41:38.013002 pinterest-dl-0.0.17/
--rw-rw-rw-   0        0        0    11340 2024-03-30 14:57:38.000000 pinterest-dl-0.0.17/LICENSE
--rw-rw-rw-   0        0        0     4821 2024-04-03 13:41:38.012002 pinterest-dl-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     3995 2024-03-31 19:12:24.000000 pinterest-dl-0.0.17/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 13:41:38.002488 pinterest-dl-0.0.17/pinterest_dl/
--rw-rw-rw-   0        0        0        0 2024-03-31 15:22:58.000000 pinterest-dl-0.0.17/pinterest_dl/__init__.py
--rw-rw-rw-   0        0        0     4432 2024-04-03 13:38:41.000000 pinterest-dl-0.0.17/pinterest_dl/api.py
--rw-rw-rw-   0        0        0     2119 2024-04-03 13:14:00.000000 pinterest-dl-0.0.17/pinterest_dl/cli_parser.py
--rw-rw-rw-   0        0        0     2248 2024-04-03 12:22:45.000000 pinterest-dl-0.0.17/pinterest_dl/downloader.py
--rw-rw-rw-   0        0        0     1535 2024-03-31 15:22:58.000000 pinterest-dl-0.0.17/pinterest_dl/driver_installer.py
--rw-rw-rw-   0        0        0     2358 2024-03-31 15:22:58.000000 pinterest-dl-0.0.17/pinterest_dl/io.py
--rw-rw-rw-   0        0        0     1371 2024-04-03 13:14:49.000000 pinterest-dl-0.0.17/pinterest_dl/main.py
--rw-rw-rw-   0        0        0      237 2024-04-03 13:30:54.000000 pinterest-dl-0.0.17/pinterest_dl/manifest.json
--rw-rw-rw-   0        0        0     6228 2024-04-03 12:43:30.000000 pinterest-dl-0.0.17/pinterest_dl/scraper.py
--rw-rw-rw-   0        0        0     1455 2024-04-03 13:23:40.000000 pinterest-dl-0.0.17/pinterest_dl/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:41:38.012002 pinterest-dl-0.0.17/pinterest_dl.egg-info/
--rw-rw-rw-   0        0        0     4821 2024-04-03 13:41:37.000000 pinterest-dl-0.0.17/pinterest_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2024-04-03 13:41:37.000000 pinterest-dl-0.0.17/pinterest_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:41:37.000000 pinterest-dl-0.0.17/pinterest_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-03 13:41:37.000000 pinterest-dl-0.0.17/pinterest_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2024-04-03 13:41:37.000000 pinterest-dl-0.0.17/pinterest_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-03 13:41:37.000000 pinterest-dl-0.0.17/pinterest_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 13:41:38.013002 pinterest-dl-0.0.17/setup.cfg
--rw-rw-rw-   0        0        0     1395 2024-04-03 11:49:16.000000 pinterest-dl-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-31 15:03:09.870368 pinterest-dl-0.0.9/
+-rw-rw-rw-   0        0        0    11340 2024-03-30 14:57:38.000000 pinterest-dl-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4596 2024-03-31 15:03:09.869861 pinterest-dl-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3879 2024-03-31 15:02:25.000000 pinterest-dl-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-31 15:03:09.854436 pinterest-dl-0.0.9/pinterest_dl/
+-rw-rw-rw-   0        0        0        0 2024-03-29 16:53:40.000000 pinterest-dl-0.0.9/pinterest_dl/__init__.py
+-rw-rw-rw-   0        0        0     2024 2024-03-31 14:55:58.000000 pinterest-dl-0.0.9/pinterest_dl/cli_parser.py
+-rw-rw-rw-   0        0        0     1947 2024-03-31 11:57:09.000000 pinterest-dl-0.0.9/pinterest_dl/downloader.py
+-rw-rw-rw-   0        0        0     1535 2024-03-31 14:55:58.000000 pinterest-dl-0.0.9/pinterest_dl/driver_installer.py
+-rw-rw-rw-   0        0        0     2358 2024-03-30 12:01:50.000000 pinterest-dl-0.0.9/pinterest_dl/io.py
+-rw-rw-rw-   0        0        0     2253 2024-03-31 14:55:58.000000 pinterest-dl-0.0.9/pinterest_dl/main.py
+-rw-rw-rw-   0        0        0      236 2024-03-31 15:01:02.000000 pinterest-dl-0.0.9/pinterest_dl/manifest.json
+-rw-rw-rw-   0        0        0     5528 2024-03-31 14:55:58.000000 pinterest-dl-0.0.9/pinterest_dl/scraper.py
+-rw-rw-rw-   0        0        0      425 2024-03-31 11:18:06.000000 pinterest-dl-0.0.9/pinterest_dl/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-31 15:03:09.869354 pinterest-dl-0.0.9/pinterest_dl.egg-info/
+-rw-rw-rw-   0        0        0     4596 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-31 15:03:09.870368 pinterest-dl-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1376 2024-03-31 14:56:39.000000 pinterest-dl-0.0.9/setup.py
```

### Comparing `pinterest-dl-0.0.17/LICENSE` & `pinterest-dl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pinterest-dl-0.0.17/PKG-INFO` & `pinterest-dl-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinterest-dl
-Version: 0.0.17
+Version: 0.0.9
 Summary: An unofficial Pinterest image downloader
 Home-page: https://github.com/sean1832/pinterest-dl
 Author: Zeke Zhang
 License: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,20 +12,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Console
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: selenium>=4.9.0
-Requires-Dist: pillow>=10.1.0
-Requires-Dist: tqdm
-Requires-Dist: pyexiv2
 
-# Pinterest Image Downloader CLI (pinterest-dl)
+# Pinterest Image Scraper CLI
 ![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)
 ![Static Badge](https://img.shields.io/badge/python-3.10%2B-yellow)
 ![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)
 
 
 
 This CLI (Command Line Interface) tool facilitates the scraping and downloading of images from [Pinterest](https://pinterest.com). Using [Selenium](https://selenium.dev) for automation, it enables users to extract images from a specified Pinterest URL and save them to a chosen directory.
@@ -94,15 +90,14 @@
 - `-t`, `--threshold [number]`: Set the number of page scrolls (default: 20).
 - `-p`, `--persistence [seconds]`: Wait time for page loading (default: 120 seconds).
 - `-r`, `--resolution [width]x[height]`: Minimum image resolution for download (e.g., 512x512).
 - `--incognito`: Activate incognito mode for scraping.
 - `--dry-run`: Execute scrape without downloading images.
 - `--firefox`: Opt for Firefox as the scraping browser.
 - `--verbose`: Enable detailed output for debugging.
-- `--headless`: Run the browser in headless mode. (no scraping progress output in headless mode)
 
 #### 2. Download
 Download images from a list of URLs provided in a file.
 
 **Syntax:**
 ```bash
 pinterest-dl download [url_list] [options]
```

### Comparing `pinterest-dl-0.0.17/README.md` & `pinterest-dl-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Pinterest Image Downloader CLI (pinterest-dl)
+# Pinterest Image Scraper CLI
 ![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)
 ![Static Badge](https://img.shields.io/badge/python-3.10%2B-yellow)
 ![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)
 
 
 
 This CLI (Command Line Interface) tool facilitates the scraping and downloading of images from [Pinterest](https://pinterest.com). Using [Selenium](https://selenium.dev) for automation, it enables users to extract images from a specified Pinterest URL and save them to a chosen directory.
@@ -71,15 +71,14 @@
 - `-t`, `--threshold [number]`: Set the number of page scrolls (default: 20).
 - `-p`, `--persistence [seconds]`: Wait time for page loading (default: 120 seconds).
 - `-r`, `--resolution [width]x[height]`: Minimum image resolution for download (e.g., 512x512).
 - `--incognito`: Activate incognito mode for scraping.
 - `--dry-run`: Execute scrape without downloading images.
 - `--firefox`: Opt for Firefox as the scraping browser.
 - `--verbose`: Enable detailed output for debugging.
-- `--headless`: Run the browser in headless mode. (no scraping progress output in headless mode)
 
 #### 2. Download
 Download images from a list of URLs provided in a file.
 
 **Syntax:**
 ```bash
 pinterest-dl download [url_list] [options]
```

### Comparing `pinterest-dl-0.0.17/pinterest_dl/cli_parser.py` & `pinterest-dl-0.0.9/pinterest_dl/cli_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,27 +10,26 @@
     parser.add_argument("-v", "--version", action="version", version="v"+meta["version"])
 
     cmd = parser.add_subparsers(dest="cmd", help="Command to run")
 
     # scrape command
     scrape_cmd = cmd.add_parser("scrape", help="Scrape images from Pinterest")
     scrape_cmd.add_argument("url", help="URL to scrape images from")
-    scrape_cmd.add_argument("output", help="Output directory")
-    scrape_cmd.add_argument("-l", "--limit", type=int, default=100, help="Max number of image to scrape (default: 100)")
-    scrape_cmd.add_argument("-r", "--resolution", type=str, help="Minimum resolution to keep (e.g. 512x512).")
-    scrape_cmd.add_argument("--persistence", type=int, default=120, help="Retry count if page does not load new content (default: 120)")
+    scrape_cmd.add_argument("-o", "--output", default="imgs", help="Output directory (default: imgs)")
+    scrape_cmd.add_argument("-w", "--write", help="Write urls to json file")
+    scrape_cmd.add_argument("-t", "--threshold", type=int, default=20, help="Number of scroll to perform (default: 20)")
+    scrape_cmd.add_argument("-p", "--persistence", type=int, default=120, help="Time to wait for page to load (default: 120)")
+    scrape_cmd.add_argument("-r", "--resolution", type=str, help="minimum resolution to keep (e.g. 512x512).")
     scrape_cmd.add_argument("--incognito", action="store_true", help="Incognito mode")
-    scrape_cmd.add_argument("--json", action="store_true", help="Write urls to json file")
     scrape_cmd.add_argument("--dry-run", action="store_true", help="Run without download")
     scrape_cmd.add_argument("--firefox", action="store_true", help="Use Firefox browser")
-    scrape_cmd.add_argument("--headful", action="store_true", help="Run in headful mode with browser window")
     scrape_cmd.add_argument("--verbose", action="store_true", help="Print verbose output")
 
     # download command
     download_cmd = cmd.add_parser("download", help="Download images")
-    download_cmd.add_argument("input", help="Input json file containing image urls")
-    download_cmd.add_argument("-o", "--output", help="Output directory (default: ./<json_filename>})")
+    download_cmd.add_argument("url_list", help="Input file containing image urls")
+    download_cmd.add_argument("-o", "--output", default="imgs", help="Output directory (default: imgs)")
     download_cmd.add_argument("-r", "--resolution", type=str, help="minimum resolution to keep (e.g. 512x512).")
     download_cmd.add_argument("--verbose", action="store_true", help="Print verbose output")
 
     return parser
 # fmt: on
```

### Comparing `pinterest-dl-0.0.17/pinterest_dl/downloader.py` & `pinterest-dl-0.0.9/pinterest_dl/downloader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,54 @@
 import concurrent.futures
 from pathlib import Path
 
 import requests
-from tqdm import tqdm
 
 
-def download(url: str, output_dir, chunk_size=2048):
+def download(url: str, output_dir, chunk_size=2048, verbose=False):
     if isinstance(url, str):
         req = requests.get(url)
         req.raise_for_status()
 
         filename = Path(url).name
         outfile = Path.joinpath(Path(output_dir), filename)
         # create directory if not exist
         outfile.parent.mkdir(parents=True, exist_ok=True)
         with open(outfile, "wb") as payload:
             for chunk in req.iter_content(chunk_size):
                 payload.write(chunk)
+        print(f"Downloaded {filename}")
         return outfile
     else:
         print("URL must be a string.")
 
 
-def download_with_fallback(url: str, output_dir, fallback_url, chunk_size=2048):
+def download_with_fallback(url: str, output_dir, fallback_url, chunk_size=2048, verbose=False):
     try:
-        return download(url, output_dir, chunk_size)
+        return download(url, output_dir, chunk_size, verbose)
     except requests.exceptions.HTTPError:
-        return download(fallback_url, output_dir, chunk_size)
+        return download(fallback_url, output_dir, chunk_size, verbose)
 
 
 def download_concurrent(urls: list, output_dir, chunk_size=2048, verbose=False):
     results = []
-    with concurrent.futures.ThreadPoolExecutor() as executor, tqdm(
-        total=len(urls), desc="Downloading"
-    ) as pbar:
+    with concurrent.futures.ThreadPoolExecutor() as executor:
         futures = [executor.submit(download, url, output_dir, chunk_size, verbose) for url in urls]
         for future in concurrent.futures.as_completed(futures):
-            outfile = future.result()
-            pbar.update(1)
-            if verbose:
-                print(f"Downloaded {outfile.name}")
-            results.append(outfile)
+            results.append(future.result())
     return results
 
 
 def download_concurrent_with_fallback(
     urls: list, output_dir, fallback_urls, chunk_size=2048, verbose=False
 ):
     results = []
-    with concurrent.futures.ThreadPoolExecutor() as executor, tqdm(
-        total=len(urls), desc="Downloading"
-    ) as pbar:
+    with concurrent.futures.ThreadPoolExecutor() as executor:
         futures = [
-            executor.submit(download_with_fallback, url, output_dir, fallback_url, chunk_size)
+            executor.submit(
+                download_with_fallback, url, output_dir, fallback_url, chunk_size, verbose
+            )
             for url, fallback_url in zip(urls, fallback_urls)
         ]
         for future in concurrent.futures.as_completed(futures):
-            outfile = future.result()
-            pbar.update(1)
-            if verbose:
-                print(f"Downloaded {outfile.name}")
-            results.append(outfile)
+            results.append(future.result())
     return results
```

### Comparing `pinterest-dl-0.0.17/pinterest_dl/driver_installer.py` & `pinterest-dl-0.0.9/pinterest_dl/driver_installer.py`

 * *Files identical despite different names*

### Comparing `pinterest-dl-0.0.17/pinterest_dl/io.py` & `pinterest-dl-0.0.9/pinterest_dl/io.py`

 * *Files identical despite different names*

### Comparing `pinterest-dl-0.0.17/pinterest_dl/scraper.py` & `pinterest-dl-0.0.9/pinterest_dl/scraper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 import copy
 import os
 import random
 import socket
 import time
+from pathlib import Path
 
 from selenium import webdriver
 from selenium.common.exceptions import StaleElementReferenceException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
-from tqdm import tqdm
 
-from pinterest_dl import driver_installer, utils
+from pinterest_dl import downloader, driver_installer, utils
 
 
 def randdelay(a, b):
     time.sleep(random.uniform(a, b))
 
 
 class Browser(object):
     def __init__(self):
         self.browser = None
 
-    def Chrome(
-        self, image_enable=False, incognito=False, exe_path="chromedriver.exe", headful=False
-    ):
+    def Chrome(self, image_enable=False, incognito=False, exe_path="chromedriver.exe"):
         if not os.path.exists(exe_path):
             driver_installer.install_chrome_driver(
-                utils.get_appdata_dir(), version="123.0.6312.86", platform="win64"
+                Path(exe_path).parent, version="123.0.6312.86", platform="win64"
             )
 
         service = webdriver.chrome.service.Service(exe_path)
         chrome_options = webdriver.ChromeOptions()
         # Disable images
         # https://scrapeops.io/selenium-web-scraping-playbook/python-selenium-disable-image-loading/
         chrome_options.add_argument(
             "--blink-settings=imagesEnabled=true"
             if image_enable
             else "--blink-settings=imagesEnabled=false"
         )
-        chrome_options.add_argument("--log-level=3")  # Suppress most logs
         if incognito:
-            print("Running in incognito mode")
             chrome_options.add_argument("--incognito")
-        if not headful:
-            print("Running in headless mode")
-            chrome_options.add_argument("--headless=new")
         browser = webdriver.Chrome(options=chrome_options, service=service)
         return browser
 
-    def Firefox(self, image_enable=False, incognito=False, headful=False):
-        firefox_options = webdriver.FirefoxOptions()
+    def Firefox(self, image_enable=False, incognito=False):
+        firefox_profile = webdriver.FirefoxProfile()
         # Disable images
         if image_enable:
-            firefox_options.set_preference("permissions.default.image", 1)
+            firefox_profile.set_preference("permissions.default.image", 1)
         else:
-            firefox_options.set_preference("permissions.default.image", 2)
+            firefox_profile.set_preference("permissions.default.image", 2)
         if incognito:
-            firefox_options.set_preference("browser.privatebrowsing.autostart", True)
-        if not headful:
-            print("Running in headless mode")
-            firefox_options.add_argument("--headless")
-        browser = webdriver.Firefox(options=firefox_options)
+            firefox_profile.set_preference("browser.privatebrowsing.autostart", True)
+        browser = webdriver.Firefox(firefox_profile=firefox_profile)
         return browser
 
+    def _download_chrome_driver_not_exist(self, exe_path):
+        if not utils.file_exists(exe_path):
+            print("Chrome driver does not exist. Downloading...")
+
+            downloader.download_curl()
+        else:
+            print("Chrome driver exists.")
+
 
 class Pinterest(object):
     def __init__(self, browser=None):
         self.browser: WebDriver = browser
 
     # currently not used
     def login(self, email, password):
@@ -79,74 +77,65 @@
         password_field.send_keys(password)
         randdelay(1, 2)  # delay between 1 and 2 seconds
         password_field.send_keys(Keys.RETURN)
 
     def scrape(
         self,
         url,
-        limit=20,
+        threshold=20,
         presistence=120,
         verbose=False,
     ):
-        unique_results = set()  # Use a set to store unique results
-        imgs_data = []  # Store image data
+        final_results = []
         previous_divs = []
         tries = 0
-        pbar = tqdm(total=limit, desc="Scraping")
+
         try:
             self.browser.get(url)
-            while len(unique_results) < limit:
+            while threshold > 0:
                 try:
                     divs = self.browser.find_elements(By.CSS_SELECTOR, "div[data-test-id='pin']")
                     if divs == previous_divs:
                         tries += 1
                     else:
                         tries = 0
                     if tries > presistence:
                         if verbose:
                             print("Exiting: persistence exceeded")
-                        break
+                        return final_results
 
                     for div in divs:
-                        if self._is_div_ad(div) or len(unique_results) >= limit:
+                        # if div is an ad, skip
+                        if self._is_div_ad(div):
                             continue
                         images = div.find_elements(By.TAG_NAME, "img")
                         for image in images:
-                            alt = image.get_attribute("alt")
                             src = image.get_attribute("src")
                             if src and "/236x/" in src:
                                 src = src.replace("/236x/", "/originals/")
-                                src_763 = src.replace("/originals/", "/736x/")
-                                if src not in unique_results:
-                                    unique_results.add(src)
-                                    img_data = {"src": src, "alt": alt, "fallback": src_763}
-                                    imgs_data.append(img_data)
-                                    pbar.update(1)
-                                    if verbose:
-                                        print(src, alt)
-                                    if len(unique_results) >= limit:
-                                        break
-
+                                final_results.append(src)
+                                if verbose:
+                                    print(src)
                     previous_divs = copy.copy(divs)  # copy to avoid reference
+                    final_results = list(set(final_results))  # remove duplicates
 
                     # Scroll down
                     dummy = self.browser.find_element(By.TAG_NAME, "a")
                     dummy.send_keys(Keys.PAGE_DOWN)
                     randdelay(1, 2)  # delay between 1 and 2 seconds
+                    threshold -= 1
 
                 except StaleElementReferenceException:
                     print("StaleElementReferenceException")
-
+                    threshold -= 1
         except (socket.error, socket.timeout):
             print("Socket Error")
-        finally:
-            pbar.close()
-            if verbose:
-                print(f"Scraped {len(imgs_data)} images")
-            return imgs_data
+        except KeyboardInterrupt:
+            return final_results
+        return final_results
 
     def _is_div_ad(self, div: WebElement):
         """Check if div is an ad.
 
         Args:
             div (webElement): div element.
         """
```

### Comparing `pinterest-dl-0.0.17/pinterest_dl.egg-info/PKG-INFO` & `pinterest-dl-0.0.9/pinterest_dl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinterest-dl
-Version: 0.0.17
+Version: 0.0.9
 Summary: An unofficial Pinterest image downloader
 Home-page: https://github.com/sean1832/pinterest-dl
 Author: Zeke Zhang
 License: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,20 +12,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Console
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: selenium>=4.9.0
-Requires-Dist: pillow>=10.1.0
-Requires-Dist: tqdm
-Requires-Dist: pyexiv2
 
-# Pinterest Image Downloader CLI (pinterest-dl)
+# Pinterest Image Scraper CLI
 ![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)
 ![Static Badge](https://img.shields.io/badge/python-3.10%2B-yellow)
 ![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)
 
 
 
 This CLI (Command Line Interface) tool facilitates the scraping and downloading of images from [Pinterest](https://pinterest.com). Using [Selenium](https://selenium.dev) for automation, it enables users to extract images from a specified Pinterest URL and save them to a chosen directory.
@@ -94,15 +90,14 @@
 - `-t`, `--threshold [number]`: Set the number of page scrolls (default: 20).
 - `-p`, `--persistence [seconds]`: Wait time for page loading (default: 120 seconds).
 - `-r`, `--resolution [width]x[height]`: Minimum image resolution for download (e.g., 512x512).
 - `--incognito`: Activate incognito mode for scraping.
 - `--dry-run`: Execute scrape without downloading images.
 - `--firefox`: Opt for Firefox as the scraping browser.
 - `--verbose`: Enable detailed output for debugging.
-- `--headless`: Run the browser in headless mode. (no scraping progress output in headless mode)
 
 #### 2. Download
 Download images from a list of URLs provided in a file.
 
 **Syntax:**
 ```bash
 pinterest-dl download [url_list] [options]
```

### Comparing `pinterest-dl-0.0.17/setup.py` & `pinterest-dl-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     packages=find_packages(),
     include_package_data=True,
     package_data={
         "": [
             "manifest.json",
         ]
     },
-    install_requires=["selenium>=4.9.0", "pillow>=10.1.0", "tqdm", "pyexiv2"],
+    install_requires=["selenium>=4.9.0", "pillow>=10.1.0"],
     entry_points={
         "console_scripts": [
             "pinterest-dl = pinterest_dl.main:main",
         ],
     },
     python_rquires=">=3.10",
     # https://pypi.org/classifiers/
```

