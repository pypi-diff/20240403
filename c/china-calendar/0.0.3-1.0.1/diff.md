# Comparing `tmp/china-calendar-0.0.3.tar.gz` & `tmp/china-calendar-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "china-calendar-0.0.3.tar", last modified: Wed Apr  3 12:47:50 2024, max compression
+gzip compressed data, was "china-calendar-1.0.1.tar", last modified: Wed Apr  3 13:03:15 2024, max compression
```

## Comparing `china-calendar-0.0.3.tar` & `china-calendar-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:47:50.715875 china-calendar-0.0.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-04-03 12:47:40.000000 china-calendar-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 12:47:50.715875 china-calendar-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 12:47:40.000000 china-calendar-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:47:50.715875 china-calendar-0.0.3/china_calendar/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 12:47:40.000000 china-calendar-0.0.3/china_calendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-03 12:47:40.000000 china-calendar-0.0.3/china_calendar/calendar_util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      277 2024-04-03 12:47:40.000000 china-calendar-0.0.3/china_calendar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:47:50.715875 china-calendar-0.0.3/china_calendar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:47:50.000000 china-calendar-0.0.3/china_calendar.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:47:50.715875 china-calendar-0.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 12:47:40.000000 china-calendar-0.0.3/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:47:50.715875 china-calendar-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3196 2024-04-03 12:47:40.000000 china-calendar-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:15.129684 china-calendar-1.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-04-03 13:03:00.000000 china-calendar-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-03 13:03:15.129684 china-calendar-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-03 13:03:00.000000 china-calendar-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:15.129684 china-calendar-1.0.1/china_calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 13:03:00.000000 china-calendar-1.0.1/china_calendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-03 13:03:00.000000 china-calendar-1.0.1/china_calendar/calendar_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      277 2024-04-03 13:03:00.000000 china-calendar-1.0.1/china_calendar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:15.129684 china-calendar-1.0.1/china_calendar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-03 13:03:15.000000 china-calendar-1.0.1/china_calendar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 13:03:15.000000 china-calendar-1.0.1/china_calendar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:03:15.000000 china-calendar-1.0.1/china_calendar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 13:03:15.000000 china-calendar-1.0.1/china_calendar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 13:03:15.000000 china-calendar-1.0.1/china_calendar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:03:15.000000 china-calendar-1.0.1/china_calendar.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:15.129684 china-calendar-1.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 13:03:00.000000 china-calendar-1.0.1/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:03:15.129684 china-calendar-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3196 2024-04-03 13:03:00.000000 china-calendar-1.0.1/setup.py
```

### Comparing `china-calendar-0.0.3/china_calendar/calendar_util.py` & `china-calendar-1.0.1/china_calendar/calendar_util.py`

 * *Files identical despite different names*

### Comparing `china-calendar-0.0.3/setup.py` & `china-calendar-1.0.1/setup.py`

 * *Files identical despite different names*

