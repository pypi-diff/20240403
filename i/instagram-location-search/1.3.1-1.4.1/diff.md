# Comparing `tmp/instagram-location-search-1.3.1.tar.gz` & `tmp/instagram-location-search-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-location-search-1.3.1.tar", last modified: Thu Nov 16 16:12:28 2023, max compression
+gzip compressed data, was "instagram-location-search-1.4.1.tar", last modified: Wed Apr  3 11:42:32 2024, max compression
```

## Comparing `instagram-location-search-1.3.1.tar` & `instagram-location-search-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 16:12:28.283573 instagram-location-search-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-16 16:11:51.000000 instagram-location-search-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2023-11-16 16:12:28.283573 instagram-location-search-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2023-11-16 16:11:51.000000 instagram-location-search-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 16:12:28.283573 instagram-location-search-1.3.1/instagram_location_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2023-11-16 16:12:28.000000 instagram-location-search-1.3.1/instagram_location_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-11-16 16:12:28.000000 instagram-location-search-1.3.1/instagram_location_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 16:12:28.000000 instagram-location-search-1.3.1/instagram_location_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-16 16:12:28.000000 instagram-location-search-1.3.1/instagram_location_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-16 16:12:28.000000 instagram-location-search-1.3.1/instagram_location_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-16 16:12:28.000000 instagram-location-search-1.3.1/instagram_location_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 16:12:28.283573 instagram-location-search-1.3.1/instagram_locations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 16:11:51.000000 instagram-location-search-1.3.1/instagram_locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2023-11-16 16:11:51.000000 instagram-location-search-1.3.1/instagram_locations/instagram_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-16 16:11:51.000000 instagram-location-search-1.3.1/instagram_locations/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 16:12:28.283573 instagram-location-search-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-16 16:11:51.000000 instagram-location-search-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:42:32.553620 instagram-location-search-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-03 11:42:32.549620 instagram-location-search-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:42:32.549620 instagram-location-search-1.4.1/instagram_location_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 11:42:32.000000 instagram-location-search-1.4.1/instagram_location_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:42:32.549620 instagram-location-search-1.4.1/instagram_locations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/instagram_locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/instagram_locations/instagram_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/instagram_locations/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:42:32.553620 instagram-location-search-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 11:41:53.000000 instagram-location-search-1.4.1/setup.py
```

### Comparing `instagram-location-search-1.3.1/LICENSE` & `instagram-location-search-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram-location-search-1.3.1/PKG-INFO` & `instagram-location-search-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-location-search
-Version: 1.3.1
+Version: 1.4.1
 Summary: Finds Instagram location IDs near a specified latitude and longitude.
 Home-page: https://www.bellingcat.com
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT License
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `instagram-location-search-1.3.1/README.md` & `instagram-location-search-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `instagram-location-search-1.3.1/instagram_location_search.egg-info/PKG-INFO` & `instagram-location-search-1.4.1/instagram_location_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-location-search
-Version: 1.3.1
+Version: 1.4.1
 Summary: Finds Instagram location IDs near a specified latitude and longitude.
 Home-page: https://www.bellingcat.com
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT License
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `instagram-location-search-1.3.1/instagram_locations/instagram_locations.py` & `instagram-location-search-1.4.1/instagram_locations/instagram_locations.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,25 +112,26 @@
     max_id_num = insta_epoch << 23
 
     return str(max_id_num)
 
 
 def get_insta_cookies():
     from selenium import webdriver
-    from selenium.webdriver.chrome.service import Service as ChromiumService
-    from webdriver_manager.chrome import ChromeDriverManager
-    from webdriver_manager.core.utils import ChromeType
+    from selenium.webdriver.chrome.service import Service
+    import os.path
     """
     Attempts to run selenium, provide user with the login form and extract cookies from page to be used in program.
     Returns cookies formatted as name=value;name=value;...
      """
     options = webdriver.ChromeOptions()
-    options.add_argument(r"--user-data-dir=~/.instagram_location_searcher/data")
-    options.add_argument(r'--profile-directory=~/.instagram_location_searcher/profile')
-    driver = webdriver.Chrome(options=options, service=ChromiumService(ChromeDriverManager(chrome_type=ChromeType.CHROMIUM).install()))
+    options.add_argument(r"--user-data-dir=" + os.path.expanduser("~/.instagram-location-search/chrome-data/"))
+    options.add_argument(r"--profile-directory=instagram-location-profile")
+
+    service = Service()
+    driver = webdriver.Chrome(options=options, service=service)
     driver.get("https://www.instagram.com/")
     # Check that there is cookie with name sessionid (mean we logged in)
     cookies = driver.get_cookies()
     while not any([cookie.get("name") == "sessionid" for cookie in cookies]):
         sleep(1)
         cookies = driver.get_cookies()
     return "; ".join([f"{cookie['name']}={cookie['value'] }"for cookie in cookies])
@@ -257,8 +258,8 @@
     if args.dump_ids:
         ids = map(lambda loc: str(loc["external_id"]), locations)
         with open(args.dump_ids, "w") as f:
             f.write("\n".join(ids))
             
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `instagram-location-search-1.3.1/setup.py` & `instagram-location-search-1.4.1/setup.py`

 * *Files identical despite different names*

