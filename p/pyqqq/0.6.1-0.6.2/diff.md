# Comparing `tmp/pyqqq-0.6.1.tar.gz` & `tmp/pyqqq-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.6.1.tar", max compression
+gzip compressed data, was "pyqqq-0.6.2.tar", max compression
```

## Comparing `pyqqq-0.6.1.tar` & `pyqqq-0.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.6.1/README.md
--rw-r--r--   0        0        0      770 2024-04-02 08:55:02.798521 pyqqq-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.6.1/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.6.1/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.6.1/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    35704 2024-03-28 00:52:30.410040 pyqqq-0.6.1/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.6.1/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    23893 2024-03-15 08:38:18.946138 pyqqq-0.6.1/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.6.1/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.6.1/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   185553 2024-03-25 09:55:40.950355 pyqqq-0.6.1/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.6.1/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.6.1/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    23713 2024-03-18 01:27:17.145321 pyqqq-0.6.1/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.6.1/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.6.1/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.6.1/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.6.1/pyqqq/data/daily.py
--rw-r--r--   0        0        0     4674 2024-03-25 05:39:48.241915 pyqqq-0.6.1/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     3993 2024-04-02 08:54:34.966109 pyqqq-0.6.1/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.6.1/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.6.1/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.6.1/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.6.1/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.6.1/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.6.1/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.6.1/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.6.1/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-27 01:29:00.427186 pyqqq-0.6.2/README.md
+-rw-r--r--   0        0        0      770 2024-04-03 03:31:06.637683 pyqqq-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-27 01:29:00.428734 pyqqq-0.6.2/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681470 pyqqq-0.6.2/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 00:30:01.958621 pyqqq-0.6.2/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    35704 2024-03-27 03:32:53.313494 pyqqq-0.6.2/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-27 01:29:00.428888 pyqqq-0.6.2/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    23893 2024-03-21 21:27:23.752968 pyqqq-0.6.2/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-27 03:32:53.313827 pyqqq-0.6.2/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681703 pyqqq-0.6.2/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   185553 2024-03-27 01:29:00.429675 pyqqq-0.6.2/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-27 01:29:00.429820 pyqqq-0.6.2/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-06 00:30:01.960145 pyqqq-0.6.2/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    23713 2024-04-03 03:29:49.352039 pyqqq-0.6.2/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-13 01:10:46.718207 pyqqq-0.6.2/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-27 01:29:00.429926 pyqqq-0.6.2/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:23:32.374681 pyqqq-0.6.2/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-02 21:29:24.457028 pyqqq-0.6.2/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     4674 2024-03-27 01:29:00.430134 pyqqq-0.6.2/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     6801 2024-04-03 03:29:20.431477 pyqqq-0.6.2/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     1254 2024-03-12 13:30:35.556769 pyqqq-0.6.2/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:23:38.166158 pyqqq-0.6.2/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-02 21:29:24.457837 pyqqq-0.6.2/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 13:30:35.556892 pyqqq-0.6.2/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-28 02:16:13.684707 pyqqq-0.6.2/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-27 01:29:00.430437 pyqqq-0.6.2/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-02 21:29:24.458374 pyqqq-0.6.2/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-28 02:16:13.684870 pyqqq-0.6.2/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.2/PKG-INFO
```

### Comparing `pyqqq-0.6.1/README.md` & `pyqqq-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyproject.toml` & `pyqqq-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.6.1"
+version = "0.6.2"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.6.1/pyqqq/__init__.py` & `pyqqq-0.6.2/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.6.2/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.6.2/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.6.2/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.6.2/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.6.2/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.6.2/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.6.2/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.6.2/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.6.2/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/data/daily.py` & `pyqqq-0.6.2/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/data/domestic.py` & `pyqqq-0.6.2/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/datatypes.py` & `pyqqq-0.6.2/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/utils/display.py` & `pyqqq-0.6.2/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/utils/kvstore.py` & `pyqqq-0.6.2/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/utils/limiter.py` & `pyqqq-0.6.2/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/utils/logger.py` & `pyqqq-0.6.2/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/utils/market_schedule.py` & `pyqqq-0.6.2/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/pyqqq/utils/retry.py` & `pyqqq-0.6.2/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.1/PKG-INFO` & `pyqqq-0.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.6.1
+Version: 0.6.2
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```
