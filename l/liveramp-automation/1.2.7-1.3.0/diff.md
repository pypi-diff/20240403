# Comparing `tmp/liveramp_automation-1.2.7.tar.gz` & `tmp/liveramp_automation-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-1.2.7.tar", last modified: Thu Mar 21 02:52:27 2024, max compression
+gzip compressed data, was "liveramp_automation-1.3.0.tar", last modified: Wed Apr  3 03:15:10 2024, max compression
```

## Comparing `liveramp_automation-1.2.7.tar` & `liveramp_automation-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-03-21 02:52:27.989904 liveramp_automation-1.2.7/
--rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.2.7/LICENSE
--rw-r--r--   0 jasqia     (503) staff       (20)     2881 2024-03-21 02:52:27.989607 liveramp_automation-1.2.7/PKG-INFO
--rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.2.7/README.md
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-03-21 02:52:27.974500 liveramp_automation-1.2.7/liveramp_automation/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.2.7/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-03-21 02:52:23.000000 liveramp_automation-1.2.7/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-03-21 02:52:27.978260 liveramp_automation-1.2.7/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.2.7/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.2.7/liveramp_automation/helpers/bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8133 2024-02-28 01:54:10.000000 liveramp_automation-1.2.7/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8905 2024-03-11 03:09:42.000000 liveramp_automation-1.2.7/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.2.7/liveramp_automation/helpers/fixture.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6158 2024-01-17 05:53:19.000000 liveramp_automation-1.2.7/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     9622 2024-03-20 08:56:22.000000 liveramp_automation-1.2.7/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-03-21 02:52:27.982586 liveramp_automation-1.2.7/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.2.7/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1934 2023-12-26 13:49:29.000000 liveramp_automation-1.2.7/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.2.7/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4960 2024-03-21 02:50:39.000000 liveramp_automation-1.2.7/liveramp_automation/utils/pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.2.7/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.2.7/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.2.7/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.2.7/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.2.7/liveramp_automation/utils/slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.2.7/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-03-21 02:52:27.989138 liveramp_automation-1.2.7/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (503) staff       (20)     2881 2024-03-21 02:52:27.000000 liveramp_automation-1.2.7/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-03-21 02:52:27.000000 liveramp_automation-1.2.7/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-03-21 02:52:27.000000 liveramp_automation-1.2.7/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (503) staff       (20)      415 2024-03-21 02:52:27.000000 liveramp_automation-1.2.7/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-03-21 02:52:27.000000 liveramp_automation-1.2.7/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-03-21 02:52:27.989945 liveramp_automation-1.2.7/setup.cfg
--rw-r--r--   0 jasqia     (503) staff       (20)     1413 2024-03-11 02:37:57.000000 liveramp_automation-1.2.7/setup.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-03-21 02:52:27.982992 liveramp_automation-1.2.7/tests/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.2.7/tests/__init__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-03-21 02:52:27.985272 liveramp_automation-1.2.7/tests/test_helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.2.7/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1086 2023-09-07 06:57:09.000000 liveramp_automation-1.2.7/tests/test_helpers/test_bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1948 2023-09-13 06:43:00.000000 liveramp_automation-1.2.7/tests/test_helpers/test_bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1666 2024-03-18 02:58:04.000000 liveramp_automation-1.2.7/tests/test_helpers/test_file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.2.7/tests/test_helpers/test_fixtures.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.2.7/tests/test_helpers/test_login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.2.7/tests/test_helpers/test_notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-03-21 02:52:27.988492 liveramp_automation-1.2.7/tests/test_utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.2.7/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1391 2024-03-18 02:37:40.000000 liveramp_automation-1.2.7/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-21 02:51:56.000000 liveramp_automation-1.2.7/tests/test_utils/test_pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2748 2024-03-14 07:02:47.000000 liveramp_automation-1.2.7/tests/test_utils/test_parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.2.7/tests/test_utils/test_playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1019 2024-03-19 01:28:39.000000 liveramp_automation-1.2.7/tests/test_utils/test_request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    39224 2023-12-27 03:33:09.000000 liveramp_automation-1.2.7/tests/test_utils/test_selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-21 01:05:58.000000 liveramp_automation-1.2.7/tests/test_utils/test_slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.2.7/tests/test_utils/test_version.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.598365 liveramp_automation-1.3.0/
+-rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.0/LICENSE
+-rw-r--r--   0 jasqia     (503) staff       (20)     2881 2024-04-03 03:15:10.598045 liveramp_automation-1.3.0/PKG-INFO
+-rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.0/README.md
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.582516 liveramp_automation-1.3.0/liveramp_automation/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.0/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-03 03:14:50.000000 liveramp_automation-1.3.0/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.586190 liveramp_automation-1.3.0/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8133 2024-02-28 01:54:10.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/fixture.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-03 03:14:23.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     9622 2024-03-20 08:56:22.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.590503 liveramp_automation-1.3.0/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.0/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.0/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.0/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4960 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/liveramp_automation/utils/pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.0/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.0/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.0/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.0/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.0/liveramp_automation/utils/slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.0/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.597522 liveramp_automation-1.3.0/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (503) staff       (20)     2881 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)      415 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-03 03:15:10.598416 liveramp_automation-1.3.0/setup.cfg
+-rw-r--r--   0 jasqia     (503) staff       (20)     1413 2024-03-11 02:37:57.000000 liveramp_automation-1.3.0/setup.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.590866 liveramp_automation-1.3.0/tests/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.0/tests/__init__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.593348 liveramp_automation-1.3.0/tests/test_helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.0/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.0/tests/test_helpers/test_bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.0/tests/test_helpers/test_bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.0/tests/test_helpers/test_file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.0/tests/test_helpers/test_fixtures.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.0/tests/test_helpers/test_login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.0/tests/test_helpers/test_notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.596951 liveramp_automation-1.3.0/tests/test_utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.0/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/tests/test_utils/test_pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.0/tests/test_utils/test_parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.0/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.0/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/tests/test_utils/test_selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/tests/test_utils/test_slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.0/tests/test_utils/test_version.py
```

### Comparing `liveramp_automation-1.2.7/LICENSE` & `liveramp_automation-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/PKG-INFO` & `liveramp_automation-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 1.2.7
+Version: 1.3.0
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.2.7/README.md` & `liveramp_automation-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/helpers/bigquery.py` & `liveramp_automation-1.3.0/liveramp_automation/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/helpers/bucket.py` & `liveramp_automation-1.3.0/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/helpers/file.py` & `liveramp_automation-1.3.0/liveramp_automation/helpers/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         :param file_path: Path to the testcase.json file.
         :return: Dictionary representing the testcase.
         """
 
         try:
             with open(file_path, "r") as file:
                 item = json.load(file)["tests"]
+            if len(item) > 0:
+                item = item[0]
             node_id = item["nodeid"]
             outcome = item["outcome"]
             groupName = node_id.split("/")[1]
             testcase = {}
             testcase["groupName"] = groupName
             testcase["className"] = node_id.split("/")[2].split("::")[0]
             testcase["caseName"] = node_id.split("/")[-1].split("::")[-1]
@@ -166,51 +168,25 @@
     def files_under_folder_with_suffix_xlsx(path_string):
         """
         Get a list of Excel files with ".xlsx" suffix in the specified folder.
 
         :param path_string: Path to the folder.
         :return: List of filenames with ".xlsx" suffix.
         """
-        try:
-            default_directory = os.path.join(os.getcwd(), path_string)
-            files = os.listdir(default_directory)
-            xlsx_files = [file for file in files if file.endswith(".xlsx")]
-            return xlsx_files
-        except FileNotFoundError:
-            Logger.error(f"Directory '{default_directory}' not found.")
-            return []
-        except PermissionError:
-            Logger.error(f"Permission denied to read files in '{default_directory}'.")
-            return []
-        except Exception as e:
-            Logger.error(f"An error occurred: {e}")
-            return []
+        return FileHelper.files_under_folder_with_suffix(".xlsx", path_string)
 
     @staticmethod
     def files_under_folder_with_suffix_csv(path_string):
         """
         Get a list of CSV files with ".csv" suffix in the specified folder.
 
         :param path_string: Path to the folder.
         :return: List of filenames with ".csv" suffix.
         """
-        try:
-            default_directory = os.path.join(os.getcwd(), path_string)
-            files = os.listdir(default_directory)
-            csv_files = [file for file in files if file.endswith(".csv")]
-            return csv_files
-        except FileNotFoundError:
-            Logger.error(f"Directory '{default_directory}' not found.")
-            return []
-        except PermissionError:
-            Logger.error(f"Permission denied to read files in '{default_directory}'.")
-            return []
-        except Exception as e:
-            Logger.error(f"An error occurred: {e}")
-            return []
+        return FileHelper.files_under_folder_with_suffix(".csv", path_string)
 
     @staticmethod
     def files_under_folder_with_suffix(file_suffix, path_string):
         """
         Get a list of files with the specified suffix in the specified folder.
 
         :param file_suffix: Suffix of the files to search for (e.g., ".txt").
```

### Comparing `liveramp_automation-1.2.7/liveramp_automation/helpers/fixture.py` & `liveramp_automation-1.3.0/liveramp_automation/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/helpers/login.py` & `liveramp_automation-1.3.0/liveramp_automation/helpers/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         page.goto(url)
         page.wait_for_load_state()
         url_new = page.url
         Logger.info("The current url is {}.".format(url_new))
         if url_new.__contains__(url):
             Logger.info("Already logged in to OKTA.")
         else:
-            page.get_by_label("Username").fill(username)
-            page.get_by_label("Username").press("Enter")
+            page.locator("id=idp-discovery-username").fill(username)
+            page.locator("id=idp-discovery-submit").press("Enter")
             allure_page_screenshot(page, "username_filled")
             page.get_by_label("Username").fill(username)
             allure_page_screenshot(page, "username_filled_again")
             page.get_by_label("Password").fill(password)
             page.get_by_label("Password").press("Enter")
             allure_page_screenshot(page, "password_filled")
             Logger.info("Logging in to OKTA...")
```

### Comparing `liveramp_automation-1.2.7/liveramp_automation/helpers/notification.py` & `liveramp_automation-1.3.0/liveramp_automation/helpers/notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/allure.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/log.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/pagerduty.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/parsers.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/playwright.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/request.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/selenium.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/slack.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation/utils/time.py` & `liveramp_automation-1.3.0/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-1.3.0/liveramp_automation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 1.2.7
+Version: 1.3.0
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.2.7/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-1.3.0/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/setup.py` & `liveramp_automation-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/tests/test_helpers/test_bucket.py` & `liveramp_automation-1.3.0/tests/test_helpers/test_bucket.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from liveramp_automation.helpers.bucket import BucketHelper
 from liveramp_automation.utils.time import MACROS
+from unittest.mock import patch
 
 project_id = "liveramp-eng-qa-reliability"
 bucket_name = "liveramp_automation_test"
-file = "test.ini"
+file = "../resources/test.ini"
 download_folder = "reports"
 download_folder_1 = "reports/001"
 download_folder_2 = "reports/002"
 number_lines = 3
 search_by_string = "test_download"
 source_file_path = "tests"
 source_file_name = "tests/test_utils/test_selenium.py"
@@ -30,14 +31,22 @@
     assert result
 
 
 def test_download_files():
     result = bucket_helper.download_files(destination_blob_name, download_folder_1)
     assert result
 
+def mocked_requests_response_throw_Exception(*args, **kwargs):
+    raise Exception("Test")
+
+@patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_throw_Exception)
+def test_download_files_exception(mock):
+    result = bucket_helper.download_files(destination_blob_name, download_folder_1)
+    assert len(result) == 0
+
 
 def test_download_files_with_structure():
     result = bucket_helper.download_files_with_structure(destination_blob_name, download_folder_2)
     assert result
 
 
 def test_download_file():
```

### Comparing `liveramp_automation-1.2.7/tests/test_helpers/test_fixtures.py` & `liveramp_automation-1.3.0/tests/test_helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/tests/test_helpers/test_login.py` & `liveramp_automation-1.3.0/tests/test_helpers/test_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/tests/test_helpers/test_notification.py` & `liveramp_automation-1.3.0/tests/test_helpers/test_notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/tests/test_utils/test_log.py` & `liveramp_automation-1.3.0/tests/test_utils/test_log.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import pytest
+from unittest.mock import patch, mock_open
 from liveramp_automation.utils.log import LoggerUtils, MyFormatter, Logger
 
 def test_log_info():
     Logger.info("info")
 
 
 def test_log_critical():
@@ -22,15 +24,15 @@
 
 def test_get_logger_returns_same_instance():
     logger_utils = LoggerUtils()
     logger1 = logger_utils.get_logger()
     logger2 = logger_utils.get_logger()
     assert logger1 == logger2
 
-def test_configure_logging_returns_logger_instance(monkeypatch):
+def test_configure_logging_returns_logger_instance():
     logger_utils = LoggerUtils()
     logger = logger_utils._configure_logging()
     assert isinstance(logger, logging.Logger)
 
 def test_get_log_format_returns_my_formatter_when_scenario_included(monkeypatch):
     logger_utils = LoggerUtils()
     monkeypatch.setenv("SCENARIO_NAME", "test_scenario")
@@ -41,7 +43,18 @@
 
 def test_get_log_format_returns_default_formatter_when_scenario_not_included(monkeypatch):
     logger_utils = LoggerUtils()
     monkeypatch.delenv("SCENARIO_NAME", raising=False)
     log_format = logger_utils.get_log_format("false")
     assert isinstance(log_format, logging.Formatter)
     assert "test_case_name" not in log_format._fmt
+
+def test_logger_utils_get_log_format_invalid_value():
+    with pytest.raises(ValueError):
+        LoggerUtils.get_log_format('invalid')
+
+def test_configure_logging_file_property_not_found():
+    with patch('builtins.open', mock_open(read_data="[data]")):
+        logger_utils = LoggerUtils()
+        logger = logger_utils._configure_logging()
+        assert isinstance(logger, logging.Logger)
+
```

### Comparing `liveramp_automation-1.2.7/tests/test_utils/test_pagerduty.py` & `liveramp_automation-1.3.0/tests/test_utils/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/tests/test_utils/test_parsers.py` & `liveramp_automation-1.3.0/tests/test_utils/test_parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import pytest
+from unittest.mock import patch
 from liveramp_automation.utils.parsers import ParseUtils
 
 
 @pytest.fixture(autouse=True)
 def setup_parser_simple():
     return ParseUtils("I want to test {str} cases")
 
+def mocked_requests_response_throw_Exception(*args, **kwargs):
+    raise ValueError("Test")
 
 def test_is_matching_simple(setup_parser_simple):
     assert setup_parser_simple.is_matching('I want to test all cases')
     assert setup_parser_simple.is_matching('I want to test "all" cases')
     assert setup_parser_simple.is_matching('I want to test {all} cases')
     assert setup_parser_simple.is_matching('I want to test the first and third cases')
 
@@ -35,14 +38,20 @@
 
 
 def test_is_matching_with_curly_brace(setup_parser_with_curly_brace):
     assert setup_parser_with_curly_brace.is_matching('I search {username} from the box')
     assert setup_parser_with_curly_brace.is_matching('I search {username} and password from the box')
     assert setup_parser_with_curly_brace.is_matching('I search {5} from the box')
 
+@patch('builtins.bool', side_effect=mocked_requests_response_throw_Exception)
+def test_is_matching_with_curly_brace_exception(mock, setup_parser_with_curly_brace):
+    assert setup_parser_with_curly_brace.is_matching('I search {username} from the box') is False
+    assert setup_parser_with_curly_brace.is_matching('I search {username} and password from the box') is False
+    assert setup_parser_with_curly_brace.is_matching('I search {5} from the box') is False
+
 
 @pytest.fixture(autouse=True)
 def setup_parser_with_digital():
     return ParseUtils("I have {number:d} apples")
 
 
 def test_parse_arguments(setup_parser_with_digital):
```

### Comparing `liveramp_automation-1.2.7/tests/test_utils/test_playwright.py` & `liveramp_automation-1.3.0/tests/test_utils/test_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/tests/test_utils/test_selenium.py` & `liveramp_automation-1.3.0/tests/test_utils/test_selenium.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from unittest.mock import Mock
+from unittest.mock import Mock, patch
 from liveramp_automation.utils.selenium import SeleniumUtils
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.common.keys import Keys
 
 
 @pytest.fixture
@@ -34,14 +34,26 @@
     # mock_chrome_driver.url.assert_called_once()
 
 
 def test_navigate_to_url(mock_chrome_driver):
     my_selenium_instance = SeleniumUtils(mock_chrome_driver)
     my_selenium_instance.navigate_to_url(path='/test', query='param=value')
 
+def test_navigate_to_url_no_path_no_query(mock_chrome_driver):
+    my_selenium_instance = SeleniumUtils(mock_chrome_driver)
+    my_selenium_instance.navigate_to_url(path=None, query=None)
+
+
+def mocked_exception_response(*args, **kwargs):
+    raise Exception("Test Exception")
+
+@patch('urllib.parse.urlparse', side_effect=mocked_exception_response)
+def test_navigate_to_url_no_path_no_query(mock_chrome_driver):
+    my_selenium_instance = SeleniumUtils(mock_chrome_driver)
+    my_selenium_instance.navigate_to_url(path=None, query=None)
 
 def test_refresh_page_url(mock_chrome_driver):
     my_selenium_instance = SeleniumUtils(mock_chrome_driver)
     my_selenium_instance.refresh_page()
     bbb = my_selenium_instance.get_page_url()
     assert bbb == mock_chrome_driver.current_url
```

### Comparing `liveramp_automation-1.2.7/tests/test_utils/test_slack.py` & `liveramp_automation-1.3.0/tests/test_utils/test_slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.2.7/tests/test_utils/test_version.py` & `liveramp_automation-1.3.0/tests/test_utils/test_version.py`

 * *Files identical despite different names*

