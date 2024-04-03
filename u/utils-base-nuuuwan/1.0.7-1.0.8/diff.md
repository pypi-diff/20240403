# Comparing `tmp/utils_base-nuuuwan-1.0.7.tar.gz` & `tmp/utils_base-nuuuwan-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_base-nuuuwan-1.0.7.tar", last modified: Sun Nov  5 13:18:02 2023, max compression
+gzip compressed data, was "utils_base-nuuuwan-1.0.8.tar", last modified: Wed Apr  3 13:34:09 2024, max compression
```

## Comparing `utils_base-nuuuwan-1.0.7.tar` & `utils_base-nuuuwan-1.0.8.tar`

### file list

```diff
@@ -1,61 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.335260 utils_base-nuuuwan-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-11-05 13:18:02.335260 utils_base-nuuuwan-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-05 13:18:02.335260 utils_base-nuuuwan-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.327260 utils_base-nuuuwan-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.327260 utils_base-nuuuwan-1.0.7/src/utils_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.327260 utils_base-nuuuwan-1.0.7/src/utils_base/console/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/console/Console.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/console/Log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/console/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.327260 utils_base-nuuuwan-1.0.7/src/utils_base/ds/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/ds/Dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/ds/Iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/ds/List.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/ds/String.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/ds/parses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.331261 utils_base-nuuuwan-1.0.7/src/utils_base/file/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/CSVFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/Directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/File.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/FileOrDirectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/FiledVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/JSONFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/PDFFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/TSVFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/XSVFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/Zip.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.331261 utils_base-nuuuwan-1.0.7/src/utils_base/geo/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/geo/LatLng.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/geo/LatLngLK.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/hashx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.331261 utils_base-nuuuwan-1.0.7/src/utils_base/image/
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/image/Image.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/mr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.331261 utils_base-nuuuwan-1.0.7/src/utils_base/time/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/time/TIMEZONE_OFFSET.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/time/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/time/TimeDelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/time/TimeFormat.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/time/TimeID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/time/TimeUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/src/utils_base/xmlx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.335260 utils_base-nuuuwan-1.0.7/src/utils_base_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-11-05 13:18:02.000000 utils_base-nuuuwan-1.0.7/src/utils_base_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-11-05 13:18:02.000000 utils_base-nuuuwan-1.0.7/src/utils_base_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-05 13:18:02.000000 utils_base-nuuuwan-1.0.7/src/utils_base_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-05 13:18:02.000000 utils_base-nuuuwan-1.0.7/src/utils_base_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-05 13:18:02.000000 utils_base-nuuuwan-1.0.7/src/utils_base_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:18:02.335260 utils_base-nuuuwan-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/tests/test_hashx.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/tests/test_mr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2023-11-05 13:17:30.000000 utils_base-nuuuwan-1.0.7/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.615722 utils_base-nuuuwan-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 13:34:09.615722 utils_base-nuuuwan-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:34:09.615722 utils_base-nuuuwan-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.603722 utils_base-nuuuwan-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.603722 utils_base-nuuuwan-1.0.8/src/utils_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.607722 utils_base-nuuuwan-1.0.8/src/utils_base/console/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/COLOR_BACKGROUND.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/COLOR_FOREGROUND.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/COLOR_FORMAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/Console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/LEVEL_TO_STYLE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/Log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.607722 utils_base-nuuuwan-1.0.8/src/utils_base/ds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/Dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/Iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/List.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/Parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/String.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.607722 utils_base-nuuuwan-1.0.8/src/utils_base/file/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/CSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/Directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/FileOrDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/FiledVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/JSONFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/PDFFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/TSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/XSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/Zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.607722 utils_base-nuuuwan-1.0.8/src/utils_base/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/geo/LatLng.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/geo/LatLngLK.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/hashx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.611722 utils_base-nuuuwan-1.0.8/src/utils_base/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/image/Image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/mr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.611722 utils_base-nuuuwan-1.0.8/src/utils_base/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/DAYS_IN.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/SECONDS_IN.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIMEZONE_OFFSET.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIME_FORMAT_DATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIME_FORMAT_DATE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIME_FORMAT_TIME.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIME_FORMAT_TIME_ID.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeDelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/get_date_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/get_time_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/xmlx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.615722 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.611722 utils_base-nuuuwan-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/tests/test_hashx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/tests/test_mr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/tests/test_time.py
```

### Comparing `utils_base-nuuuwan-1.0.7/LICENSE` & `utils_base-nuuuwan-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/PKG-INFO` & `utils_base-nuuuwan-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_base-nuuuwan
-Version: 1.0.7
+Version: 1.0.8
 Summary: Utilities that extend Standard Python.
 Home-page: https://github.com/nuuuwan/utils_base
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_base-nuuuwan-1.0.7/README.md` & `utils_base-nuuuwan-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 ```
 pip install utils_base-nuuuwan
 ```
 
 ## Version History
 
-### 1.0.7
+### 1.0.8 (CURRENT VERSION)
+* Enable Log to process non strings
+* Use new pyl_build_inits (MIGHT BREAK)
+
+### 1.0.7 
 * Fix log ignore BUG (Take 2)
 
 ### 1.0.6 
 * Fix log ignore BUG
 
 ### 1.0.5
 * Added Console, improved Log
```

### Comparing `utils_base-nuuuwan-1.0.7/setup.py` & `utils_base-nuuuwan-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils_base'
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 DESCRIPTION = "Utilities that extend Standard Python."
 INSTALL_REQUIRES = [
     'camelot-py',
     'opencv-python',
     'PyPDF2==2.0.0',
     'Pillow',
     'geopy',
```

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/console/Console.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/console/Console.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from utils_base.console.constants import (COLOR_BACKGROUND, COLOR_FOREGROUND,
-                                          COLOR_FORMAT)
+from utils_base.console.COLOR_BACKGROUND import COLOR_BACKGROUND
+from utils_base.console.COLOR_FOREGROUND import COLOR_FOREGROUND
+from utils_base.console.COLOR_FORMAT import COLOR_FORMAT
 
 
 class Console:
     @staticmethod
     def format(*args, **kwargs) -> str:
         foreground = kwargs.get('foreground', '')
         background = kwargs.get('background', '')
```

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/console/Log.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/console/Log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Utils."""
 
 import logging
 
 from utils_base.console.Console import Console
-from utils_base.console.constants import LEVEL_TO_STYLE
+from utils_base.console.LEVEL_TO_STYLE import LEVEL_TO_STYLE
 
 
 class CustomLoggingFormatter(logging.Formatter):
     def format(self, record):
         style = LEVEL_TO_STYLE[record.levelno]
         return Console.format(
-            (f'[{record.name}] ' if record.name else ''),
-            record.msg,
+            (f'[{record.name}]' if record.name else ''),
+            str(record.msg),
             **style,
         )
 
 
 class Log(logging.Logger):
     def __init__(self, name: str, level: int = logging.DEBUG):
         super(Log, self).__init__(name, level)
         self.propagate = False
 
         formatter = CustomLoggingFormatter()
         sh = logging.StreamHandler()
         sh.setLevel(logging.DEBUG)
         sh.setFormatter(formatter)
         self.handlers = [sh]  # noqa
-
-
-_log = Log('')
```

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/ds/Dict.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/ds/Dict.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/ds/List.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/ds/List.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/ds/String.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/ds/String.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/file/Directory.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/file/Directory.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/file/File.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/file/File.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/file/FiledVariable.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/file/FiledVariable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tempfile
 
-from utils_base import hashx
 from utils_base.file.JSONFile import JSONFile
+from utils_base.hashx import hashx
 
 FILE_VARIABLE_CACHE = {}
 
 
 class FiledVariable:
     def __init__(self, key: str, func_get):
         self.key = key
```

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/file/PDFFile.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/file/PDFFile.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/file/XSVFile.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/file/XSVFile.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/file/Zip.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/file/Zip.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/geo/LatLng.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/geo/LatLng.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 
 import geopy.distance
 
-from utils_base.ds.parses import parse_float
+from utils_base.ds import Parse
 
 
 class LatLng:
     def __init__(self, lat: float, lng: float):
         self.lat = lat
         self.lng = lng
 
@@ -26,16 +26,16 @@
 
     @staticmethod
     def parse(latlng_str_original: str) -> str:
         latlng_str = latlng_str_original.replace('°', ' ').strip()
         for x in ['N', 'S', 'E', 'W']:
             latlng_str = latlng_str.replace(x, '')
         lat_str, lng_str = latlng_str.split(',')
-        lat = parse_float(lat_str) * (-1 if 'S' in latlng_str_original else 1)
-        lng = parse_float(lng_str) * (-1 if 'W' in latlng_str_original else 1)
+        lat = Parse.float(lat_str) * (-1 if 'S' in latlng_str_original else 1)
+        lng = Parse.float(lng_str) * (-1 if 'W' in latlng_str_original else 1)
         return LatLng(lat, lng)
 
     def distance(self, other: 'LatLng') -> float:
         return geopy.distance.geodesic(
             (self.lat, self.lng), (other.lat, other.lng)
         ).km
```

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/geo/LatLngLK.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/geo/LatLngLK.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/image/Image.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/image/Image.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/mr.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/mr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 """Map-Reduce utils_base."""
 
 import concurrent.futures
 
 DEFAULT_MAX_THREADS = 4
 
 
-def _run_parallel(workers, max_threads=DEFAULT_MAX_THREADS):
-    """Run workers in parallel."""
-    with concurrent.futures.ThreadPoolExecutor(max_threads) as thread_pool:
-        future_list = []
-        for worker in workers:
-            future = thread_pool.submit(worker)
-            future_list.append(future)
-
-        for future in future_list:
-            future.done()
-
-        output_list = []
-        for future in future_list:
-            output_list.append(future.result())
-        return output_list
-
-
-def map_parallel(func_map, params_list, max_threads=DEFAULT_MAX_THREADS):
-    """Run list(map(...)) in parallel.
-
-    Args:
-        func_map (function): Mapper function
-        params_list (list): Params to be mapped
-        max_threads (int, optional): Maximum parallel threads.
-            DEFAULT_MAX_THREADS = 4
-
-    .. code-block:: python
-
-        >>> from utils_base import mr
-        >>> print(mr.map_parallel(lambda x: x ** 2, [1, 2, 3, 4]))
-        [1, 4, 9, 16]
-
-    """
-
-    def get_worker(params):
-        def worker():
-            return func_map(params)
-
-        return worker
-
-    workers = list(
-        map(
-            lambda params: get_worker(params=params),
-            params_list,
+class mr:
+    @staticmethod
+    def _run_parallel(workers, max_threads=DEFAULT_MAX_THREADS):
+        """Run workers in parallel."""
+        with concurrent.futures.ThreadPoolExecutor(
+            max_threads
+        ) as thread_pool:
+            future_list = []
+            for worker in workers:
+                future = thread_pool.submit(worker)
+                future_list.append(future)
+
+            for future in future_list:
+                future.done()
+
+            output_list = []
+            for future in future_list:
+                output_list.append(future.result())
+            return output_list
+
+    @staticmethod
+    def map_parallel(func_map, params_list, max_threads=DEFAULT_MAX_THREADS):
+        """Run list(map(...)) in parallel.
+
+        Args:
+            func_map (function): Mapper function
+            params_list (list): Params to be mapped
+            max_threads (int, optional): Maximum parallel threads.
+                DEFAULT_MAX_THREADS = 4
+
+        .. code-block:: python
+
+            >>> from utils_base import mr
+            >>> print(mr.map_parallel(lambda x: x ** 2, [1, 2, 3, 4]))
+            [1, 4, 9, 16]
+
+        """
+
+        def get_worker(params):
+            def worker():
+                return func_map(params)
+
+            return worker
+
+        workers = list(
+            map(
+                lambda params: get_worker(params=params),
+                params_list,
+            )
         )
-    )
-    return _run_parallel(workers, max_threads)
+        return mr._run_parallel(workers, max_threads)
```

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/time/Time.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/time/Time.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/time/TimeDelta.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeDelta.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base/time/TimeFormat.py` & `utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeFormat.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,12 +23,12 @@
             self.format_str, time.localtime(t.ut + self.dut_timezone)
         )
 
     def format(self, t: Time) -> str:
         return self.stringify(t)
 
 
-TIME_FORMAT_DATE = TimeFormat('%Y-%m-%d')  # noqa
-TIME_FORMAT_TIME = TimeFormat('%Y-%m-%d %H:%M:%S')  # noqa
+TimeFormat.DATE = TimeFormat('%Y-%m-%d')  # noqa
+TimeFormat.TIME = TimeFormat('%Y-%m-%d %H:%M:%S')  # noqa
 
-TIME_FORMAT_DATE_ID = TimeFormat('%Y%m%d')  # noqa
-TIME_FORMAT_TIME_ID = TimeFormat('%Y%m%d.%H%M%S')  # noqa
+TimeFormat.DATE_ID = TimeFormat('%Y%m%d')  # noqa
+TimeFormat.TIME_ID = TimeFormat('%Y%m%d.%H%M%S')  # noqa
```

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base_nuuuwan.egg-info/PKG-INFO` & `utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: utils-base-nuuuwan
-Version: 1.0.7
+Name: utils_base-nuuuwan
+Version: 1.0.8
 Summary: Utilities that extend Standard Python.
 Home-page: https://github.com/nuuuwan/utils_base
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_base-nuuuwan-1.0.7/src/utils_base_nuuuwan.egg-info/SOURCES.txt` & `utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 LICENSE
 README.md
 setup.py
+src/utils_base/_.py
 src/utils_base/__init__.py
 src/utils_base/hashx.py
 src/utils_base/mr.py
 src/utils_base/xmlx.py
+src/utils_base/console/COLOR_BACKGROUND.py
+src/utils_base/console/COLOR_FOREGROUND.py
+src/utils_base/console/COLOR_FORMAT.py
 src/utils_base/console/Console.py
+src/utils_base/console/LEVEL_TO_STYLE.py
 src/utils_base/console/Log.py
 src/utils_base/console/__init__.py
-src/utils_base/console/constants.py
+src/utils_base/console/_log.py
 src/utils_base/ds/Dict.py
 src/utils_base/ds/Iter.py
 src/utils_base/ds/List.py
+src/utils_base/ds/Parse.py
 src/utils_base/ds/String.py
 src/utils_base/ds/__init__.py
-src/utils_base/ds/parses.py
 src/utils_base/file/CSVFile.py
 src/utils_base/file/Directory.py
 src/utils_base/file/File.py
 src/utils_base/file/FileOrDirectory.py
 src/utils_base/file/FiledVariable.py
 src/utils_base/file/JSONFile.py
 src/utils_base/file/PDFFile.py
@@ -27,21 +32,28 @@
 src/utils_base/file/Zip.py
 src/utils_base/file/__init__.py
 src/utils_base/geo/LatLng.py
 src/utils_base/geo/LatLngLK.py
 src/utils_base/geo/__init__.py
 src/utils_base/image/Image.py
 src/utils_base/image/__init__.py
+src/utils_base/time/DAYS_IN.py
+src/utils_base/time/SECONDS_IN.py
 src/utils_base/time/TIMEZONE_OFFSET.py
+src/utils_base/time/TIME_FORMAT_DATE.py
+src/utils_base/time/TIME_FORMAT_DATE_ID.py
+src/utils_base/time/TIME_FORMAT_TIME.py
+src/utils_base/time/TIME_FORMAT_TIME_ID.py
 src/utils_base/time/Time.py
 src/utils_base/time/TimeDelta.py
 src/utils_base/time/TimeFormat.py
-src/utils_base/time/TimeID.py
 src/utils_base/time/TimeUnit.py
 src/utils_base/time/__init__.py
+src/utils_base/time/get_date_id.py
+src/utils_base/time/get_time_id.py
 src/utils_base_nuuuwan.egg-info/PKG-INFO
 src/utils_base_nuuuwan.egg-info/SOURCES.txt
 src/utils_base_nuuuwan.egg-info/dependency_links.txt
 src/utils_base_nuuuwan.egg-info/requires.txt
 src/utils_base_nuuuwan.egg-info/top_level.txt
 tests/test_hashx.py
 tests/test_mr.py
```

### Comparing `utils_base-nuuuwan-1.0.7/tests/test_mr.py` & `utils_base-nuuuwan-1.0.8/tests/test_mr.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.7/tests/test_time.py` & `utils_base-nuuuwan-1.0.8/tests/test_time.py`

 * *Files identical despite different names*

