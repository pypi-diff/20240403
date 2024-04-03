# Comparing `tmp/instagram-location-search-1.4.1.tar.gz` & `tmp/instagram-location-search-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-location-search-1.4.1.tar", last modified: Wed Apr  3 11:42:32 2024, max compression
+gzip compressed data, was "instagram-location-search-1.4.2.tar", last modified: Wed Apr  3 13:25:53 2024, max compression
```

## Comparing `instagram-location-search-1.4.1.tar` & `instagram-location-search-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:42:32.553620 instagram-location-search-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-03 11:42:32.549620 instagram-location-search-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:42:32.549620 instagram-location-search-1.4.1/instagram_location_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:42:32.549620 instagram-location-search-1.4.1/instagram_locations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/instagram_locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/instagram_locations/instagram_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/instagram_locations/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:42:32.553620 instagram-location-search-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/instagram_location_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/instagram_locations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/instagram_locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/instagram_locations/instagram_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/instagram_locations/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/setup.py
```

### Comparing `instagram-location-search-1.4.1/LICENSE` & `instagram-location-search-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram-location-search-1.4.1/PKG-INFO` & `instagram-location-search-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-location-search
-Version: 1.4.1
+Version: 1.4.2
 Summary: Finds Instagram location IDs near a specified latitude and longitude.
 Home-page: https://www.bellingcat.com
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT License
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `instagram-location-search-1.4.1/README.md` & `instagram-location-search-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `instagram-location-search-1.4.1/instagram_location_search.egg-info/PKG-INFO` & `instagram-location-search-1.4.2/instagram_location_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-location-search
-Version: 1.4.1
+Version: 1.4.2
 Summary: Finds Instagram location IDs near a specified latitude and longitude.
 Home-page: https://www.bellingcat.com
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT License
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `instagram-location-search-1.4.1/instagram_locations/instagram_locations.py` & `instagram-location-search-1.4.2/instagram_locations/instagram_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return []
     except requests.exceptions.Timeout:
         print(f"Connections timed out after {timeout} seconds")
         return []
 
     try:
         locations = response.json()
-    except json.JSONDecodeError:
+    except json.decoder.JSONDecodeError:
         print(f"Failed to get location data for {lat_long}: please check you have a valid cookie")
         return []
 
     if not isinstance(locations, dict):
         print(f"Got invalid response for {lat_long}")
         return []
```

### Comparing `instagram-location-search-1.4.1/setup.py` & `instagram-location-search-1.4.2/setup.py`

 * *Files identical despite different names*

