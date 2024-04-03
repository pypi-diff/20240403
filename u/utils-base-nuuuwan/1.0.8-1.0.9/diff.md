# Comparing `tmp/utils_base-nuuuwan-1.0.8.tar.gz` & `tmp/utils_base-nuuuwan-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_base-nuuuwan-1.0.8.tar", last modified: Wed Apr  3 13:34:09 2024, max compression
+gzip compressed data, was "utils_base-nuuuwan-1.0.9.tar", last modified: Wed Apr  3 15:36:57 2024, max compression
```

## Comparing `utils_base-nuuuwan-1.0.8.tar` & `utils_base-nuuuwan-1.0.9.tar`

### file list

```diff
@@ -1,73 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.615722 utils_base-nuuuwan-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 13:34:09.615722 utils_base-nuuuwan-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:34:09.615722 utils_base-nuuuwan-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.603722 utils_base-nuuuwan-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.603722 utils_base-nuuuwan-1.0.8/src/utils_base/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.607722 utils_base-nuuuwan-1.0.8/src/utils_base/console/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/COLOR_BACKGROUND.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/COLOR_FOREGROUND.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/COLOR_FORMAT.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/Console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/LEVEL_TO_STYLE.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/Log.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/console/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.607722 utils_base-nuuuwan-1.0.8/src/utils_base/ds/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/Dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/Iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/List.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/Parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/String.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/ds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.607722 utils_base-nuuuwan-1.0.8/src/utils_base/file/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/CSVFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/Directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/File.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/FileOrDirectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/FiledVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/JSONFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/PDFFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/TSVFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/XSVFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/Zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.607722 utils_base-nuuuwan-1.0.8/src/utils_base/geo/
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/geo/LatLng.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/geo/LatLngLK.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/hashx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.611722 utils_base-nuuuwan-1.0.8/src/utils_base/image/
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/image/Image.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/mr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.611722 utils_base-nuuuwan-1.0.8/src/utils_base/time/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/DAYS_IN.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/SECONDS_IN.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIMEZONE_OFFSET.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIME_FORMAT_DATE.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIME_FORMAT_DATE_ID.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIME_FORMAT_TIME.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TIME_FORMAT_TIME_ID.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeDelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeFormat.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/get_date_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/time/get_time_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/src/utils_base/xmlx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.615722 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 13:34:09.000000 utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:34:09.611722 utils_base-nuuuwan-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/tests/test_hashx.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/tests/test_mr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-03 13:33:51.000000 utils_base-nuuuwan-1.0.8/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.615350 utils_base-nuuuwan-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 15:36:57.611350 utils_base-nuuuwan-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:36:57.615350 utils_base-nuuuwan-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.603350 utils_base-nuuuwan-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.603350 utils_base-nuuuwan-1.0.9/src/utils_base/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/Hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/Parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.603350 utils_base-nuuuwan-1.0.9/src/utils_base/console/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/console/Console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/console/Log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.607350 utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/COLOR_BACKGROUND.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/COLOR_FOREGROUND.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/COLOR_FORMAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/LEVEL_TO_STYLE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.607350 utils_base-nuuuwan-1.0.9/src/utils_base/ds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/ds/Dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/ds/Iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/ds/List.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/ds/Parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/ds/String.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/ds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.607350 utils_base-nuuuwan-1.0.9/src/utils_base/file/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/CSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/Directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/FileOrDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/FiledVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/JSONFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/PDFFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/TSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/XSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/Zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.607350 utils_base-nuuuwan-1.0.9/src/utils_base/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/geo/LatLng.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/geo/LatLngLK.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.607350 utils_base-nuuuwan-1.0.9/src/utils_base/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/image/Image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.611350 utils_base-nuuuwan-1.0.9/src/utils_base/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/time/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/time/TimeDelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/time/TimeFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/time/TimeUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/time/TimeZoneOffset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.611350 utils_base-nuuuwan-1.0.9/src/utils_base/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/xml/XMLElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/xml/XMLUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/xml/_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/src/utils_base/xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.611350 utils_base-nuuuwan-1.0.9/src/utils_base_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 15:36:57.000000 utils_base-nuuuwan-1.0.9/src/utils_base_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-03 15:36:57.000000 utils_base-nuuuwan-1.0.9/src/utils_base_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:36:57.000000 utils_base-nuuuwan-1.0.9/src/utils_base_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 15:36:57.000000 utils_base-nuuuwan-1.0.9/src/utils_base_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 15:36:57.000000 utils_base-nuuuwan-1.0.9/src/utils_base_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:36:57.611350 utils_base-nuuuwan-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/tests/test_hashx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/tests/test_mr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-03 15:36:38.000000 utils_base-nuuuwan-1.0.9/tests/test_time.py
```

### Comparing `utils_base-nuuuwan-1.0.8/LICENSE` & `utils_base-nuuuwan-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/PKG-INFO` & `utils_base-nuuuwan-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_base-nuuuwan
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities that extend Standard Python.
 Home-page: https://github.com/nuuuwan/utils_base
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_base-nuuuwan-1.0.8/README.md` & `utils_base-nuuuwan-1.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,32 +8,48 @@
 
 ```
 pip install utils_base-nuuuwan
 ```
 
 ## Version History
 
-### 1.0.8 (CURRENT VERSION)
+### 1.0.10 (NEXT VERSION)
+
+### 1.0.9 (CURRENT VERSION)
+
+* Moved console constants to constants folder
+* Removed _log, added Log.main etc
+* Added TimeFormat(...).formatNow
+* Cleaned-up TimeUnit and TimeId functions
+* Refactored Hash, Parallel (mr) and XML
+
+### 1.0.8 
+
 * Enable Log to process non strings
 * Use new pyl_build_inits (MIGHT BREAK)
 
 ### 1.0.7 
+
 * Fix log ignore BUG (Take 2)
 
 ### 1.0.6 
+
 * Fix log ignore BUG
 
 ### 1.0.5
+
 * Added Console, improved Log
 * Added TimeFormat.format
 
 ### 1.0.4 
+
 * Fixed geo init bug
 
 ### 1.0.3 
+
 * Added image
 * Deprecated Color
 * Deprecated Table
 * List: Added map and filter
 * Added parse_int and parse_float
 * Added Geo
```

### Comparing `utils_base-nuuuwan-1.0.8/setup.py` & `utils_base-nuuuwan-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils_base'
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 DESCRIPTION = "Utilities that extend Standard Python."
 INSTALL_REQUIRES = [
     'camelot-py',
     'opencv-python',
     'PyPDF2==2.0.0',
     'Pillow',
     'geopy',
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/_.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/xml/XMLElement.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     },
     'svg': {
         'xmlns': 'http://www.w3.org/2000/svg',
     },
 }
 
 
-class _:
+class XMLElement:
     def __init__(
         self,
         tag: str,
         child_list_or_str_or_other=None,
         attrib_custom={},
     ):
         self.tag = tag
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/console/COLOR_BACKGROUND.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/COLOR_BACKGROUND.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/console/COLOR_FOREGROUND.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/COLOR_FOREGROUND.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/console/Console.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/console/Console.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from utils_base.console.COLOR_BACKGROUND import COLOR_BACKGROUND
-from utils_base.console.COLOR_FOREGROUND import COLOR_FOREGROUND
-from utils_base.console.COLOR_FORMAT import COLOR_FORMAT
+from utils_base.console.constants import (COLOR_BACKGROUND, COLOR_FOREGROUND,
+                                          COLOR_FORMAT)
 
 
 class Console:
     @staticmethod
     def format(*args, **kwargs) -> str:
         foreground = kwargs.get('foreground', '')
         background = kwargs.get('background', '')
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/console/LEVEL_TO_STYLE.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/console/constants/LEVEL_TO_STYLE.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
-from utils_base.console.COLOR_BACKGROUND import COLOR_BACKGROUND
-from utils_base.console.COLOR_FOREGROUND import COLOR_FOREGROUND
-from utils_base.console.COLOR_FORMAT import COLOR_FORMAT
+from utils_base.console.constants.COLOR_BACKGROUND import COLOR_BACKGROUND
+from utils_base.console.constants.COLOR_FOREGROUND import COLOR_FOREGROUND
+from utils_base.console.constants.COLOR_FORMAT import COLOR_FORMAT
 
 LEVEL_TO_STYLE = {
     logging.CRITICAL: dict(
         foreground=COLOR_FOREGROUND.WHITE,
         background=COLOR_BACKGROUND.RED,
         format=COLOR_FORMAT.BOLD,
     ),
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/console/Log.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/console/Log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utils."""
 
 import logging
 
 from utils_base.console.Console import Console
-from utils_base.console.LEVEL_TO_STYLE import LEVEL_TO_STYLE
+from utils_base.console.constants import LEVEL_TO_STYLE
 
 
 class CustomLoggingFormatter(logging.Formatter):
     def format(self, record):
         style = LEVEL_TO_STYLE[record.levelno]
         return Console.format(
             (f'[{record.name}]' if record.name else ''),
@@ -22,7 +22,12 @@
         self.propagate = False
 
         formatter = CustomLoggingFormatter()
         sh = logging.StreamHandler()
         sh.setLevel(logging.DEBUG)
         sh.setFormatter(formatter)
         self.handlers = [sh]  # noqa
+
+
+Log.default = Log('default')
+Log.main = Log('main')
+Log.pipeline = Log('pipeline')
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/ds/Dict.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/ds/Dict.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/ds/List.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/ds/List.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/ds/String.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/ds/String.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/file/Directory.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/file/Directory.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/file/File.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/file/File.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/file/FiledVariable.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/file/FiledVariable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import tempfile
 
 from utils_base.file.JSONFile import JSONFile
-from utils_base.hashx import hashx
+from utils_base.Hash import Hash
 
 FILE_VARIABLE_CACHE = {}
 
 
 class FiledVariable:
     def __init__(self, key: str, func_get):
         self.key = key
         self.func_get = func_get
 
     @property
     def cache_key(self):
-        return hashx.md5(self.key)
+        return Hash.md5(self.key)
 
     @property
     def file_path(self):
         return tempfile.NamedTemporaryFile(
             prefix="cache.", suffix=".json"
         ).name
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/file/PDFFile.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/file/PDFFile.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/file/XSVFile.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/file/XSVFile.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/file/Zip.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/file/Zip.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/file/__init__.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/file/__init__.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/geo/LatLng.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/geo/LatLng.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/geo/LatLngLK.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/geo/LatLngLK.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/image/Image.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/image/Image.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/mr.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/Parallel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Map-Reduce utils_base."""
 
 import concurrent.futures
 
 DEFAULT_MAX_THREADS = 4
 
 
-class mr:
+class Parallel:
     @staticmethod
-    def _run_parallel(workers, max_threads=DEFAULT_MAX_THREADS):
+    def run(workers, max_threads=DEFAULT_MAX_THREADS):
         """Run workers in parallel."""
         with concurrent.futures.ThreadPoolExecutor(
             max_threads
         ) as thread_pool:
             future_list = []
             for worker in workers:
                 future = thread_pool.submit(worker)
@@ -22,15 +22,15 @@
 
             output_list = []
             for future in future_list:
                 output_list.append(future.result())
             return output_list
 
     @staticmethod
-    def map_parallel(func_map, params_list, max_threads=DEFAULT_MAX_THREADS):
+    def map(func_map, params_list, max_threads=DEFAULT_MAX_THREADS):
         """Run list(map(...)) in parallel.
 
         Args:
             func_map (function): Mapper function
             params_list (list): Params to be mapped
             max_threads (int, optional): Maximum parallel threads.
                 DEFAULT_MAX_THREADS = 4
@@ -51,8 +51,8 @@
 
         workers = list(
             map(
                 lambda params: get_worker(params=params),
                 params_list,
             )
         )
-        return mr._run_parallel(workers, max_threads)
+        return Parallel.run(workers, max_threads)
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/time/Time.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/time/Time.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeDelta.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/time/TimeDelta.py`

 * *Files identical despite different names*

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeFormat.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/time/TimeFormat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 
 from utils_base.time.Time import Time
-from utils_base.time.TIMEZONE_OFFSET import TIMEZONE_OFFSET
+from utils_base.time.TimeZoneOffset import TimeZoneOffset
 
 
 class TimeFormat:
-    def __init__(self, format_str: str, timezone_offset=TIMEZONE_OFFSET.LK):
+    def __init__(self, format_str: str, timezone_offset=TimeZoneOffset.LK):
         self.format_str = format_str
         self.timezone_offset = timezone_offset
 
     @property
     def dut_timezone(self):
         return time.timezone - self.timezone_offset
 
@@ -22,13 +22,17 @@
         return time.strftime(
             self.format_str, time.localtime(t.ut + self.dut_timezone)
         )
 
     def format(self, t: Time) -> str:
         return self.stringify(t)
 
+    @property
+    def formatNow(self) -> str:
+        return self.format(Time.now())
+
 
 TimeFormat.DATE = TimeFormat('%Y-%m-%d')  # noqa
 TimeFormat.TIME = TimeFormat('%Y-%m-%d %H:%M:%S')  # noqa
 
 TimeFormat.DATE_ID = TimeFormat('%Y%m%d')  # noqa
 TimeFormat.TIME_ID = TimeFormat('%Y%m%d.%H%M%S')  # noqa
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/time/TimeUnit.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/time/TimeUnit.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,7 +26,31 @@
 TimeUnit.DAY = TimeUnit.HOUR * 24
 TimeUnit.WEEK = TimeUnit.DAY * 7
 TimeUnit.FORTNIGHT = TimeUnit.WEEK * 7
 
 TimeUnit.AVG_YEAR = TimeUnit.DAY * 365.25
 TimeUnit.AVG_QTR = TimeUnit.AVG_YEAR / 4
 TimeUnit.AVG_MONTH = TimeUnit.AVG_YEAR / 12
+
+
+class SECONDS_IN:  # noqa
+    MINUTE = TimeUnit.MINUTE / TimeUnit.SECOND
+    HOUR = TimeUnit.HOUR / TimeUnit.SECOND
+    DAY = TimeUnit.DAY / TimeUnit.SECOND
+    WEEK = TimeUnit.WEEK / TimeUnit.SECOND
+    FORTNIGHT = TimeUnit.FORTNIGHT / TimeUnit.SECOND
+
+    AVG_MONTH = TimeUnit.AVG_MONTH / TimeUnit.SECOND
+    AVG_QTR = TimeUnit.AVG_QTR / TimeUnit.SECOND
+    AVG_YEAR = TimeUnit.AVG_YEAR / TimeUnit.SECOND
+
+
+TimeUnit.SECOND_IN = SECONDS_IN
+
+
+class DAYS_IN:  # noqa
+    AVG_MONTH = TimeUnit.AVG_MONTH / TimeUnit.DAY
+    AVG_QTR = TimeUnit.AVG_QTR / TimeUnit.DAY
+    AVG_YEAR = TimeUnit.AVG_YEAR / TimeUnit.DAY
+
+
+TimeUnit.DAYS_IN = DAYS_IN
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base/xmlx.py` & `utils_base-nuuuwan-1.0.9/src/utils_base/xml/XMLUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from utils_base._ import _
 from utils_base.ds.String import String
+from utils_base.xml._ import _
 
 FONT_FAMILY = 'sans-serif'
 DEFAULT_ATTRIB_MAP = {
     'html': {
         'style': 'font-family: %s;' % FONT_FAMILY,
     },
     'svg': {
         'xmlns': 'http://www.w3.org/2000/svg',
     },
 }
 
 
-class xmlx:
+class XMLUtils:
     @staticmethod
     def render_link_styles(css_file='styles.css'):
         return _('link', None, {'rel': 'stylesheet', 'href': css_file})
 
     @staticmethod
     def style(**kwargs):
         style_content = ''.join(
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/PKG-INFO` & `utils_base-nuuuwan-1.0.9/src/utils_base_nuuuwan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_base-nuuuwan
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities that extend Standard Python.
 Home-page: https://github.com/nuuuwan/utils_base
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_base-nuuuwan-1.0.8/src/utils_base_nuuuwan.egg-info/SOURCES.txt` & `utils_base-nuuuwan-1.0.9/src/utils_base_nuuuwan.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 LICENSE
 README.md
 setup.py
-src/utils_base/_.py
+src/utils_base/Hash.py
+src/utils_base/Parallel.py
 src/utils_base/__init__.py
-src/utils_base/hashx.py
-src/utils_base/mr.py
-src/utils_base/xmlx.py
-src/utils_base/console/COLOR_BACKGROUND.py
-src/utils_base/console/COLOR_FOREGROUND.py
-src/utils_base/console/COLOR_FORMAT.py
 src/utils_base/console/Console.py
-src/utils_base/console/LEVEL_TO_STYLE.py
 src/utils_base/console/Log.py
 src/utils_base/console/__init__.py
-src/utils_base/console/_log.py
+src/utils_base/console/constants/COLOR_BACKGROUND.py
+src/utils_base/console/constants/COLOR_FOREGROUND.py
+src/utils_base/console/constants/COLOR_FORMAT.py
+src/utils_base/console/constants/LEVEL_TO_STYLE.py
+src/utils_base/console/constants/__init__.py
 src/utils_base/ds/Dict.py
 src/utils_base/ds/Iter.py
 src/utils_base/ds/List.py
 src/utils_base/ds/Parse.py
 src/utils_base/ds/String.py
 src/utils_base/ds/__init__.py
 src/utils_base/file/CSVFile.py
@@ -32,28 +30,24 @@
 src/utils_base/file/Zip.py
 src/utils_base/file/__init__.py
 src/utils_base/geo/LatLng.py
 src/utils_base/geo/LatLngLK.py
 src/utils_base/geo/__init__.py
 src/utils_base/image/Image.py
 src/utils_base/image/__init__.py
-src/utils_base/time/DAYS_IN.py
-src/utils_base/time/SECONDS_IN.py
-src/utils_base/time/TIMEZONE_OFFSET.py
-src/utils_base/time/TIME_FORMAT_DATE.py
-src/utils_base/time/TIME_FORMAT_DATE_ID.py
-src/utils_base/time/TIME_FORMAT_TIME.py
-src/utils_base/time/TIME_FORMAT_TIME_ID.py
 src/utils_base/time/Time.py
 src/utils_base/time/TimeDelta.py
 src/utils_base/time/TimeFormat.py
 src/utils_base/time/TimeUnit.py
+src/utils_base/time/TimeZoneOffset.py
 src/utils_base/time/__init__.py
-src/utils_base/time/get_date_id.py
-src/utils_base/time/get_time_id.py
+src/utils_base/xml/XMLElement.py
+src/utils_base/xml/XMLUtils.py
+src/utils_base/xml/_.py
+src/utils_base/xml/__init__.py
 src/utils_base_nuuuwan.egg-info/PKG-INFO
 src/utils_base_nuuuwan.egg-info/SOURCES.txt
 src/utils_base_nuuuwan.egg-info/dependency_links.txt
 src/utils_base_nuuuwan.egg-info/requires.txt
 src/utils_base_nuuuwan.egg-info/top_level.txt
 tests/test_hashx.py
 tests/test_mr.py
```

### Comparing `utils_base-nuuuwan-1.0.8/tests/test_time.py` & `utils_base-nuuuwan-1.0.9/tests/test_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 from unittest import TestCase
 
-from utils_base import (TIMEZONE_OFFSET, Time, TimeDelta, TimeFormat, TimeUnit,
-                        get_date_id, get_time_id)
+from utils_base import Time, TimeDelta, TimeFormat, TimeUnit, TimeZoneOffset
 
 
 class TestTime(TestCase):
     def test_init(self):
         ut = 1234567890
         t = Time(ut)
         self.assertEqual(t.ut, ut)
@@ -51,32 +50,32 @@
     def test_format_stringify(self):
         t = Time(1234567890)
         for format_str, expected_time_str, ut2 in [
             ['%Y-%m-%d', '2009-02-14', 1234549800],
             ['%Y-%m-%d %H:%M', '2009-02-14 05:01', 1234567860],
             ['%Y-%m-%d %H:%M:%S', '2009-02-14 05:01:30', 1234567890],
         ]:
-            tf = TimeFormat(format_str, TIMEZONE_OFFSET.LK)
+            tf = TimeFormat(format_str, TimeZoneOffset.LK)
             self.assertEqual(
                 expected_time_str,
                 tf.stringify(t),
             )
 
             t2 = Time(ut2)
             self.assertEqual(
                 t2,
                 tf.parse(expected_time_str),
             )
 
     def test_time_id(self):
-        time_id = get_time_id()
+        time_id = TimeFormat.TIME_ID.formatNow
         self.assertEqual(len(time_id), 15)
 
     def test_date_id(self):
-        date_id = get_date_id()
+        date_id = TimeFormat.DATE_ID.formatNow
         self.assertEqual(len(date_id), 8)
 
     def test_time_unit_truediv(self):
         self.assertEqual(TimeUnit(1) / 2, TimeUnit(0.5))
         self.assertEqual(TimeUnit(1) / TimeUnit(0.5), 2.0)
 
         with self.assertRaises(TypeError):
```

