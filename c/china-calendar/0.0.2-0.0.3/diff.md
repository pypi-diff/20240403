# Comparing `tmp/china-calendar-0.0.2.tar.gz` & `tmp/china-calendar-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "china-calendar-0.0.2.tar", last modified: Wed Apr  3 12:42:46 2024, max compression
+gzip compressed data, was "china-calendar-0.0.3.tar", last modified: Wed Apr  3 12:47:50 2024, max compression
```

## Comparing `china-calendar-0.0.2.tar` & `china-calendar-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:46.026693 china-calendar-0.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-04-03 12:42:34.000000 china-calendar-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-03 12:42:46.026693 china-calendar-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 12:42:34.000000 china-calendar-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:46.026693 china-calendar-0.0.2/china_calendar/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 12:42:34.000000 china-calendar-0.0.2/china_calendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-03 12:42:34.000000 china-calendar-0.0.2/china_calendar/calendar_util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      277 2024-04-03 12:42:34.000000 china-calendar-0.0.2/china_calendar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:46.026693 china-calendar-0.0.2/china_calendar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-03 12:42:45.000000 china-calendar-0.0.2/china_calendar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 12:42:46.000000 china-calendar-0.0.2/china_calendar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:42:45.000000 china-calendar-0.0.2/china_calendar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 12:42:45.000000 china-calendar-0.0.2/china_calendar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 12:42:45.000000 china-calendar-0.0.2/china_calendar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:42:45.000000 china-calendar-0.0.2/china_calendar.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:46.026693 china-calendar-0.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 12:42:34.000000 china-calendar-0.0.2/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:42:46.026693 china-calendar-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3196 2024-04-03 12:42:34.000000 china-calendar-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:47:50.715875 china-calendar-0.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-04-03 12:47:40.000000 china-calendar-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 12:47:50.715875 china-calendar-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 12:47:40.000000 china-calendar-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:47:50.715875 china-calendar-0.0.3/china_calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 12:47:40.000000 china-calendar-0.0.3/china_calendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-03 12:47:40.000000 china-calendar-0.0.3/china_calendar/calendar_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      277 2024-04-03 12:47:40.000000 china-calendar-0.0.3/china_calendar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:47:50.715875 china-calendar-0.0.3/china_calendar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:47:50.715875 china-calendar-0.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 12:47:40.000000 china-calendar-0.0.3/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:47:50.715875 china-calendar-0.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3196 2024-04-03 12:47:40.000000 china-calendar-0.0.3/setup.py
```

### Comparing `china-calendar-0.0.2/PKG-INFO` & `china-calendar-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: china-calendar
-Version: 0.0.2
+Version: 0.0.3
 Summary: a calendar about china
 Home-page: https://github.com/mouday/china-calendar
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: china,calendar,workday,holiday
 Platform: any
@@ -31,7 +31,18 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: parsel
 
 # china-calendar
 
+a calendar about china
+
+判断某一天是否为工作日或者是法定节假日，仅适用于中国
+
+安装
+
+使用示例：
+
+```python
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `china-calendar-0.0.2/china_calendar/calendar_util.py` & `china-calendar-0.0.3/china_calendar/calendar_util.py`

 * *Files identical despite different names*

### Comparing `china-calendar-0.0.2/china_calendar.egg-info/PKG-INFO` & `china-calendar-0.0.3/china_calendar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: china-calendar
-Version: 0.0.2
+Version: 0.0.3
 Summary: a calendar about china
 Home-page: https://github.com/mouday/china-calendar
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: china,calendar,workday,holiday
 Platform: any
@@ -31,7 +31,18 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: parsel
 
 # china-calendar
 
+a calendar about china
+
+判断某一天是否为工作日或者是法定节假日，仅适用于中国
+
+安装
+
+使用示例：
+
+```python
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `china-calendar-0.0.2/setup.py` & `china-calendar-0.0.3/setup.py`

 * *Files identical despite different names*

