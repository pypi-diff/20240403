# Comparing `tmp/canada_holiday-1.1.3.tar.gz` & `tmp/canada_holiday-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canada_holiday-1.1.3.tar", max compression
+gzip compressed data, was "canada_holiday-1.1.4.tar", max compression
```

## Comparing `canada_holiday-1.1.3.tar` & `canada_holiday-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-07-09 19:27:30.778904 canada_holiday-1.1.3/LICENSE
--rw-r--r--   0        0        0     1584 2023-07-09 19:27:30.778996 canada_holiday-1.1.3/README.md
--rw-r--r--   0        0        0      115 2023-07-09 19:27:30.779141 canada_holiday-1.1.3/canada_holiday/__init__.py
--rw-r--r--   0        0        0     6456 2023-07-23 17:29:04.827449 canada_holiday-1.1.3/canada_holiday/holiday_class.py
--rw-r--r--   0        0        0        0 2023-07-09 19:27:30.779340 canada_holiday-1.1.3/canada_holiday/holiday_info/__init__.py
--rw-r--r--   0        0        0      812 2023-07-09 19:27:30.779448 canada_holiday-1.1.3/canada_holiday/holiday_info/ab.py
--rw-r--r--   0        0        0      846 2023-07-09 19:27:30.779546 canada_holiday-1.1.3/canada_holiday/holiday_info/all.py
--rw-r--r--   0        0        0      862 2023-07-09 19:27:30.779620 canada_holiday-1.1.3/canada_holiday/holiday_info/bc.py
--rw-r--r--   0        0        0      670 2023-07-09 19:27:30.779709 canada_holiday-1.1.3/canada_holiday/holiday_info/mb.py
--rw-r--r--   0        0        0      453 2023-07-09 19:27:30.779782 canada_holiday-1.1.3/canada_holiday/holiday_info/national.py
--rw-r--r--   0        0        0      524 2023-07-09 19:27:30.779849 canada_holiday-1.1.3/canada_holiday/holiday_info/nb.py
--rw-r--r--   0        0        0      671 2023-07-09 19:27:30.779923 canada_holiday-1.1.3/canada_holiday/holiday_info/nl.py
--rw-r--r--   0        0        0      357 2023-07-09 19:27:30.780002 canada_holiday-1.1.3/canada_holiday/holiday_info/ns.py
--rw-r--r--   0        0        0      706 2023-07-09 19:27:30.780089 canada_holiday-1.1.3/canada_holiday/holiday_info/nt.py
--rw-r--r--   0        0        0      584 2023-07-09 19:27:30.780164 canada_holiday-1.1.3/canada_holiday/holiday_info/nu.py
--rw-r--r--   0        0        0      888 2023-07-09 19:27:30.780244 canada_holiday-1.1.3/canada_holiday/holiday_info/on.py
--rw-r--r--   0        0        0      384 2023-07-09 19:27:30.780328 canada_holiday-1.1.3/canada_holiday/holiday_info/pe.py
--rw-r--r--   0        0        0      658 2023-07-09 19:27:30.780395 canada_holiday-1.1.3/canada_holiday/holiday_info/qc.py
--rw-r--r--   0        0        0      686 2023-07-09 19:27:30.780468 canada_holiday-1.1.3/canada_holiday/holiday_info/sk.py
--rw-r--r--   0        0        0      876 2023-07-09 19:27:30.780547 canada_holiday-1.1.3/canada_holiday/holiday_info/yt.py
--rwxr-xr-x   0        0        0     2744 2023-07-09 19:27:30.780648 canada_holiday-1.1.3/canada_holiday/holidays.py
--rw-r--r--   0        0        0     4599 2023-07-23 17:29:04.827740 canada_holiday-1.1.3/canada_holiday/utils.py
--rw-r--r--   0        0        0      482 2023-07-23 17:29:19.855091 canada_holiday-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2182 1970-01-01 00:00:00.000000 canada_holiday-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-09 19:27:30.778904 canada_holiday-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1584 2023-07-09 19:27:30.778996 canada_holiday-1.1.4/README.md
+-rw-r--r--   0        0        0      115 2023-07-09 19:27:30.779141 canada_holiday-1.1.4/canada_holiday/__init__.py
+-rw-r--r--   0        0        0     6456 2024-04-03 00:53:07.026249 canada_holiday-1.1.4/canada_holiday/holiday_class.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:27:30.779340 canada_holiday-1.1.4/canada_holiday/holiday_info/__init__.py
+-rw-r--r--   0        0        0      812 2023-07-09 19:27:30.779448 canada_holiday-1.1.4/canada_holiday/holiday_info/ab.py
+-rw-r--r--   0        0        0      846 2023-07-09 19:27:30.779546 canada_holiday-1.1.4/canada_holiday/holiday_info/all.py
+-rw-r--r--   0        0        0      862 2023-07-09 19:27:30.779620 canada_holiday-1.1.4/canada_holiday/holiday_info/bc.py
+-rw-r--r--   0        0        0      670 2023-07-09 19:27:30.779709 canada_holiday-1.1.4/canada_holiday/holiday_info/mb.py
+-rw-r--r--   0        0        0      453 2023-07-09 19:27:30.779782 canada_holiday-1.1.4/canada_holiday/holiday_info/national.py
+-rw-r--r--   0        0        0      524 2023-07-09 19:27:30.779849 canada_holiday-1.1.4/canada_holiday/holiday_info/nb.py
+-rw-r--r--   0        0        0      671 2023-07-09 19:27:30.779923 canada_holiday-1.1.4/canada_holiday/holiday_info/nl.py
+-rw-r--r--   0        0        0      357 2023-07-09 19:27:30.780002 canada_holiday-1.1.4/canada_holiday/holiday_info/ns.py
+-rw-r--r--   0        0        0      706 2023-07-09 19:27:30.780089 canada_holiday-1.1.4/canada_holiday/holiday_info/nt.py
+-rw-r--r--   0        0        0      584 2023-07-09 19:27:30.780164 canada_holiday-1.1.4/canada_holiday/holiday_info/nu.py
+-rw-r--r--   0        0        0      888 2023-07-09 19:27:30.780244 canada_holiday-1.1.4/canada_holiday/holiday_info/on.py
+-rw-r--r--   0        0        0      384 2023-07-09 19:27:30.780328 canada_holiday-1.1.4/canada_holiday/holiday_info/pe.py
+-rw-r--r--   0        0        0      658 2023-07-09 19:27:30.780395 canada_holiday-1.1.4/canada_holiday/holiday_info/qc.py
+-rw-r--r--   0        0        0      686 2023-07-09 19:27:30.780468 canada_holiday-1.1.4/canada_holiday/holiday_info/sk.py
+-rw-r--r--   0        0        0      876 2023-07-09 19:27:30.780547 canada_holiday-1.1.4/canada_holiday/holiday_info/yt.py
+-rwxr-xr-x   0        0        0     2744 2024-04-03 00:53:07.026480 canada_holiday-1.1.4/canada_holiday/holidays.py
+-rw-r--r--   0        0        0     4599 2023-07-23 17:29:04.827740 canada_holiday-1.1.4/canada_holiday/utils.py
+-rw-r--r--   0        0        0      482 2024-04-03 00:58:55.243186 canada_holiday-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2182 1970-01-01 00:00:00.000000 canada_holiday-1.1.4/PKG-INFO
```

### Comparing `canada_holiday-1.1.3/LICENSE` & `canada_holiday-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/README.md` & `canada_holiday-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_class.py` & `canada_holiday-1.1.4/canada_holiday/holiday_class.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/ab.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/ab.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/all.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/all.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/bc.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/bc.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/mb.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/mb.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/nb.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/nb.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/nl.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/nl.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/nt.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/nt.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/nu.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/nu.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/on.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/on.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/qc.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/qc.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/sk.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/sk.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holiday_info/yt.py` & `canada_holiday-1.1.4/canada_holiday/holiday_info/yt.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/holidays.py` & `canada_holiday-1.1.4/canada_holiday/holidays.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/canada_holiday/utils.py` & `canada_holiday-1.1.4/canada_holiday/utils.py`

 * *Files identical despite different names*

### Comparing `canada_holiday-1.1.3/PKG-INFO` & `canada_holiday-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canada-holiday
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python package for Canadian holidays
 Home-page: https://github.com/kmsunmin/canada-holiday
 Author: Sunmin Kim
 Author-email: kmsunmin@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

