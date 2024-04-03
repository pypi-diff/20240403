# Comparing `tmp/utils_www-nuuuwan-1.2.7.tar.gz` & `tmp/utils_www-nuuuwan-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_www-nuuuwan-1.2.7.tar", last modified: Wed Sep 27 02:13:59 2023, max compression
+gzip compressed data, was "utils_www-nuuuwan-1.2.8.tar", last modified: Wed Apr  3 16:01:34 2024, max compression
```

## Comparing `utils_www-nuuuwan-1.2.7.tar` & `utils_www-nuuuwan-1.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:13:59.253153 utils_www-nuuuwan-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-09-27 02:13:09.000000 utils_www-nuuuwan-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-09-27 02:13:59.253153 utils_www-nuuuwan-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-09-27 02:13:09.000000 utils_www-nuuuwan-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-27 02:13:59.253153 utils_www-nuuuwan-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-09-27 02:13:09.000000 utils_www-nuuuwan-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:13:59.249153 utils_www-nuuuwan-1.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:13:59.253153 utils_www-nuuuwan-1.2.7/src/utils_www/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-27 02:13:09.000000 utils_www-nuuuwan-1.2.7/src/utils_www/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2023-09-27 02:13:09.000000 utils_www-nuuuwan-1.2.7/src/utils_www/www.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:13:59.253153 utils_www-nuuuwan-1.2.7/src/utils_www_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-09-27 02:13:59.000000 utils_www-nuuuwan-1.2.7/src/utils_www_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-09-27 02:13:59.000000 utils_www-nuuuwan-1.2.7/src/utils_www_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 02:13:59.000000 utils_www-nuuuwan-1.2.7/src/utils_www_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-27 02:13:59.000000 utils_www-nuuuwan-1.2.7/src/utils_www_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-27 02:13:59.000000 utils_www-nuuuwan-1.2.7/src/utils_www_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:13:59.253153 utils_www-nuuuwan-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-09-27 02:13:09.000000 utils_www-nuuuwan-1.2.7/tests/test_www.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:01:34.435006 utils_www-nuuuwan-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 16:01:11.000000 utils_www-nuuuwan-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-03 16:01:34.435006 utils_www-nuuuwan-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-03 16:01:11.000000 utils_www-nuuuwan-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:01:34.435006 utils_www-nuuuwan-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-03 16:01:11.000000 utils_www-nuuuwan-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:01:34.435006 utils_www-nuuuwan-1.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:01:34.435006 utils_www-nuuuwan-1.2.8/src/utils_www/
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-03 16:01:11.000000 utils_www-nuuuwan-1.2.8/src/utils_www/WWW.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 16:01:11.000000 utils_www-nuuuwan-1.2.8/src/utils_www/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:01:34.435006 utils_www-nuuuwan-1.2.8/src/utils_www_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-03 16:01:34.000000 utils_www-nuuuwan-1.2.8/src/utils_www_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 16:01:34.000000 utils_www-nuuuwan-1.2.8/src/utils_www_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:01:34.000000 utils_www-nuuuwan-1.2.8/src/utils_www_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 16:01:34.000000 utils_www-nuuuwan-1.2.8/src/utils_www_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 16:01:34.000000 utils_www-nuuuwan-1.2.8/src/utils_www_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:01:34.435006 utils_www-nuuuwan-1.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 16:01:11.000000 utils_www-nuuuwan-1.2.8/tests/test_www.py
```

### Comparing `utils_www-nuuuwan-1.2.7/LICENSE` & `utils_www-nuuuwan-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_www-nuuuwan-1.2.7/PKG-INFO` & `utils_www-nuuuwan-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_www-nuuuwan
-Version: 1.2.7
+Version: 1.2.8
 Summary: Utilities for accessing webpages
 Home-page: https://github.com/nuuuwan/utils_www
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_www/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_www-nuuuwan-1.2.7/setup.py` & `utils_www-nuuuwan-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils_www'
-VERSION = "1.2.7"
+VERSION = "1.2.8"
 DESCRIPTION = "Utilities for accessing webpages"
 
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
```

### Comparing `utils_www-nuuuwan-1.2.7/src/utils_www/www.py` & `utils_www-nuuuwan-1.2.8/src/utils_www/WWW.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import ssl
 import tempfile
 
 import requests
 from bs4 import BeautifulSoup
 from selenium import webdriver
 from selenium.webdriver.firefox.options import Options
-from utils_base import CSVFile, File, JSONFile, Log, TSVFile, hashx
+from utils_base import CSVFile, File, Hash, JSONFile, Log, TSVFile
 
 log = Log('WWW')
 
 USER_AGENT = ''.join(
     [
         'Mozilla/5.0 (Macintosh; Intel Mac OS X 10.14; rv:65.0) ',
         'Gecko/20100101 Firefox/65.0',
@@ -36,15 +36,15 @@
 
 class WWW:
     def __init__(self, url: str):
         self.url = url
 
     @property
     def hash_id(self):
-        return hashx.md5(self.url)[:HASH_LENGTH]
+        return Hash.md5(self.url)[:HASH_LENGTH]
 
     @property
     def ext(self):
         for ext in CUSTOM_EXT_LIST + HTML_EXT_LIST:
             if self.url.endswith(ext):
                 return ext
         return 'htm'
```

### Comparing `utils_www-nuuuwan-1.2.7/src/utils_www_nuuuwan.egg-info/PKG-INFO` & `utils_www-nuuuwan-1.2.8/src/utils_www_nuuuwan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: utils-www-nuuuwan
-Version: 1.2.7
+Name: utils_www-nuuuwan
+Version: 1.2.8
 Summary: Utilities for accessing webpages
 Home-page: https://github.com/nuuuwan/utils_www
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_www/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

