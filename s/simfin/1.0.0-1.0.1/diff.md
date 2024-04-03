# Comparing `tmp/simfin-1.0.0.tar.gz` & `tmp/simfin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfin-1.0.0.tar", last modified: Fri Jan 19 21:30:30 2024, max compression
+gzip compressed data, was "simfin-1.0.1.tar", last modified: Wed Apr  3 11:30:52 2024, max compression
```

## Comparing `simfin-1.0.0.tar` & `simfin-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2024-01-19 21:30:30.529539 simfin-1.0.0/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1259 2023-02-22 12:33:47.000000 simfin-1.0.0/LICENSE.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2024-01-19 21:30:30.529321 simfin-1.0.0/PKG-INFO
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7352 2023-02-22 12:33:47.000000 simfin-1.0.0/README.md
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)       38 2024-01-19 21:30:30.529597 simfin-1.0.0/setup.cfg
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1008 2024-01-19 17:05:29.000000 simfin-1.0.0/setup.py
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2024-01-19 21:30:30.528019 simfin-1.0.0/simfin/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1621 2024-01-19 17:05:29.000000 simfin-1.0.0/simfin/__init__.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11769 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/cache.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     4917 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/config.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    10036 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/datasets.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     6944 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/derived.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11018 2024-01-19 17:05:29.000000 simfin-1.0.0/simfin/download.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      743 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/exceptions.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    31133 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/hubs.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     8872 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/info.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11940 2023-04-13 14:10:11.000000 simfin-1.0.0/simfin/load.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     2925 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/load_info.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    19450 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/names.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7990 2023-02-22 13:21:56.000000 simfin-1.0.0/simfin/names_extra.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     3830 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/paths.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    17189 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/rel_change.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14284 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/resample.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    37350 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/signals.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14331 2023-02-22 12:33:47.000000 simfin-1.0.0/simfin/transform.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    16713 2023-08-30 14:51:51.000000 simfin-1.0.0/simfin/utils.py
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2024-01-19 21:30:30.529100 simfin-1.0.0/simfin.egg-info/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2024-01-19 21:30:30.000000 simfin-1.0.0/simfin.egg-info/PKG-INFO
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      521 2024-01-19 21:30:30.000000 simfin-1.0.0/simfin.egg-info/SOURCES.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)        1 2024-01-19 21:30:30.000000 simfin-1.0.0/simfin.egg-info/dependency_links.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)       22 2024-01-19 21:30:30.000000 simfin-1.0.0/simfin.egg-info/requires.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)        7 2024-01-19 21:30:30.000000 simfin-1.0.0/simfin.egg-info/top_level.txt
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2024-04-03 11:30:52.125871 simfin-1.0.1/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1259 2023-02-22 12:33:47.000000 simfin-1.0.1/LICENSE.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2024-04-03 11:30:52.125659 simfin-1.0.1/PKG-INFO
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7352 2023-02-22 12:33:47.000000 simfin-1.0.1/README.md
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)       38 2024-04-03 11:30:52.125918 simfin-1.0.1/setup.cfg
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1008 2024-04-03 11:21:24.000000 simfin-1.0.1/setup.py
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2024-04-03 11:30:52.124388 simfin-1.0.1/simfin/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1621 2024-04-03 11:21:24.000000 simfin-1.0.1/simfin/__init__.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11769 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/cache.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     4917 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/config.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    10036 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/datasets.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     6944 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/derived.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11021 2024-04-03 11:20:58.000000 simfin-1.0.1/simfin/download.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      743 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/exceptions.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    31133 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/hubs.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     8872 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/info.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11940 2023-04-13 14:10:11.000000 simfin-1.0.1/simfin/load.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     2925 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/load_info.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    19450 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/names.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7990 2023-02-22 13:21:56.000000 simfin-1.0.1/simfin/names_extra.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     3830 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/paths.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    17189 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/rel_change.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14284 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/resample.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    37350 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/signals.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14331 2023-02-22 12:33:47.000000 simfin-1.0.1/simfin/transform.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    16713 2023-08-30 14:51:51.000000 simfin-1.0.1/simfin/utils.py
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2024-04-03 11:30:52.125453 simfin-1.0.1/simfin.egg-info/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2024-04-03 11:30:52.000000 simfin-1.0.1/simfin.egg-info/PKG-INFO
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      521 2024-04-03 11:30:52.000000 simfin-1.0.1/simfin.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)        1 2024-04-03 11:30:52.000000 simfin-1.0.1/simfin.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)       22 2024-04-03 11:30:52.000000 simfin-1.0.1/simfin.egg-info/requires.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)        7 2024-04-03 11:30:52.000000 simfin-1.0.1/simfin.egg-info/top_level.txt
```

### Comparing `simfin-1.0.0/LICENSE.txt` & `simfin-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/PKG-INFO` & `simfin-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfin
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple financial data for Python
 Home-page: https://github.com/simfin/simfin
 Author: SimFin
 Author-email: info@simfin.com
 License: MIT
 Keywords: financial data,finance
 Description-Content-Type: text/markdown
```

### Comparing `simfin-1.0.0/README.md` & `simfin-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/setup.py` & `simfin-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 # This is also defined in simfin/__init__.py and must be
 # updated in both places.
-MY_VERSION = '1.0.0'
+MY_VERSION = '1.0.1'
 
 setup(
     name='simfin',
     packages=['simfin'],
     version=MY_VERSION,
     description='Simple financial data for Python',
     long_description='SimFin makes it easy to obtain and use financial and '
```

### Comparing `simfin-1.0.0/simfin/__init__.py` & `simfin-1.0.1/simfin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This is also defined in setup.py and must be updated in both places.
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 # Expose the following as top-level imports.
 
 from simfin.cache import cache
 from simfin.config import set_api_key, load_api_key, get_api_key
 from simfin.config import set_data_dir, get_data_dir, get_download_dir
 from simfin.derived import ebitda, free_cash_flow, shares
```

### Comparing `simfin-1.0.0/simfin/cache.py` & `simfin-1.0.1/simfin/cache.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/config.py` & `simfin-1.0.1/simfin/config.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/datasets.py` & `simfin-1.0.1/simfin/datasets.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/derived.py` & `simfin-1.0.1/simfin/derived.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/download.py` & `simfin-1.0.1/simfin/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         args += '&variant=' + variant
 
     # Market.
     if market is not None:
         args += '&market=' + market
 
     # Base URL for the bulk-download API on the SimFin server.
-    base_url = 'https://prod.simfin.com/api/bulk-download?'
+    base_url = 'https://prod.simfin.com/api/bulk-download/s3?'
     # Combine base URL and arguments.
     url = base_url + args
 
     return url
 
 
 def _url_info(name):
```

### Comparing `simfin-1.0.0/simfin/exceptions.py` & `simfin-1.0.1/simfin/exceptions.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/hubs.py` & `simfin-1.0.1/simfin/hubs.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/info.py` & `simfin-1.0.1/simfin/info.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/load.py` & `simfin-1.0.1/simfin/load.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/load_info.py` & `simfin-1.0.1/simfin/load_info.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/names.py` & `simfin-1.0.1/simfin/names.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/names_extra.py` & `simfin-1.0.1/simfin/names_extra.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/paths.py` & `simfin-1.0.1/simfin/paths.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/rel_change.py` & `simfin-1.0.1/simfin/rel_change.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/resample.py` & `simfin-1.0.1/simfin/resample.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/signals.py` & `simfin-1.0.1/simfin/signals.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/transform.py` & `simfin-1.0.1/simfin/transform.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin/utils.py` & `simfin-1.0.1/simfin/utils.py`

 * *Files identical despite different names*

### Comparing `simfin-1.0.0/simfin.egg-info/PKG-INFO` & `simfin-1.0.1/simfin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfin
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple financial data for Python
 Home-page: https://github.com/simfin/simfin
 Author: SimFin
 Author-email: info@simfin.com
 License: MIT
 Keywords: financial data,finance
 Description-Content-Type: text/markdown
```

### Comparing `simfin-1.0.0/simfin.egg-info/SOURCES.txt` & `simfin-1.0.1/simfin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

