# Comparing `tmp/cryptopian_infra-0.1.1.tar.gz` & `tmp/cryptopian_infra-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptopian_infra-0.1.1.tar", last modified: Sun Mar 31 15:41:58 2024, max compression
+gzip compressed data, was "cryptopian_infra-0.1.2.tar", last modified: Wed Apr  3 04:37:30 2024, max compression
```

## Comparing `cryptopian_infra-0.1.1.tar` & `cryptopian_infra-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.666127 cryptopian_infra-0.1.1/
--rw-r--r--   0 wuhan      (501) staff       (20)     1063 2022-01-19 16:43:46.000000 cryptopian_infra-0.1.1/LICENSE
--rw-r--r--   0 wuhan      (501) staff       (20)     1187 2024-03-31 15:41:58.665792 cryptopian_infra-0.1.1/PKG-INFO
--rw-r--r--   0 wuhan      (501) staff       (20)      446 2024-03-07 06:40:10.000000 cryptopian_infra-0.1.1/README.md
--rw-r--r--   0 wuhan      (501) staff       (20)      690 2024-03-31 15:41:45.000000 cryptopian_infra-0.1.1/pyproject.toml
--rw-r--r--   0 wuhan      (501) staff       (20)       38 2024-03-31 15:41:58.666347 cryptopian_infra-0.1.1/setup.cfg
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.648647 cryptopian_infra-0.1.1/src/
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.650101 cryptopian_infra-0.1.1/src/cryptopian_infra/
--rw-r--r--   0 wuhan      (501) staff       (20)        0 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/__init__.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.652738 cryptopian_infra-0.1.1/src/cryptopian_infra/alert/
--rw-r--r--   0 wuhan      (501) staff       (20)      112 2024-03-31 08:31:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/alert/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1512 2024-01-15 10:05:02.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/alert/alert.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1819 2024-03-29 08:42:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/alert/alertwrapper.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1221 2024-03-31 08:31:29.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/alert/slackwebhook.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.656062 cryptopian_infra-0.1.1/src/cryptopian_infra/config/
--rw-r--r--   0 wuhan      (501) staff       (20)      278 2024-03-12 15:01:14.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/config/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2057 2024-03-05 08:29:11.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/config/apimanager.py
--rw-r--r--   0 wuhan      (501) staff       (20)      872 2023-07-22 01:54:36.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/config/configloader.py
--rw-r--r--   0 wuhan      (501) staff       (20)      902 2022-05-08 03:39:06.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/config/docencryptionfactory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2555 2024-01-23 06:24:43.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/config/influxfactory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2341 2024-01-28 08:42:04.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/config/mongofactory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2799 2024-03-31 15:39:56.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/config/secretmanagerbase.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1878 2024-03-31 08:39:28.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/config/slackwebhookfactory.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.658476 cryptopian_infra-0.1.1/src/cryptopian_infra/infra/
--rw-r--r--   0 wuhan      (501) staff       (20)      145 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/infra/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1403 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/infra/duration.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2112 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/infra/emailclient.py
--rw-r--r--   0 wuhan      (501) staff       (20)      169 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/infra/gracefullystopdocker.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1013 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/infra/stopwatch.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.659278 cryptopian_infra-0.1.1/src/cryptopian_infra/mongo/
--rw-r--r--   0 wuhan      (501) staff       (20)       45 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/mongo/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1591 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/mongo/mongoparameters.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1071 2024-03-29 08:43:35.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/sendalert.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.661235 cryptopian_infra-0.1.1/src/cryptopian_infra/threading/
--rw-r--r--   0 wuhan      (501) staff       (20)       80 2024-03-07 11:38:15.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/threading/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)      421 2024-03-07 12:56:51.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/threading/atomicaccstore.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1303 2024-03-10 04:46:21.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/threading/messagepump.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.664125 cryptopian_infra-0.1.1/src/cryptopian_infra/utils/
--rw-r--r--   0 wuhan      (501) staff       (20)       51 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/utils/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)      346 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/utils/asyncutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)      626 2024-03-20 03:40:17.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/utils/datetimeutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)      810 2024-02-04 12:54:21.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/utils/dictutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)      133 2024-01-17 10:32:22.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/utils/listutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1496 2024-03-05 04:22:42.000000 cryptopian_infra-0.1.1/src/cryptopian_infra/utils/mathutils.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.665345 cryptopian_infra-0.1.1/src/cryptopian_infra.egg-info/
--rw-r--r--   0 wuhan      (501) staff       (20)     1187 2024-03-31 15:41:58.000000 cryptopian_infra-0.1.1/src/cryptopian_infra.egg-info/PKG-INFO
--rw-r--r--   0 wuhan      (501) staff       (20)     1545 2024-03-31 15:41:58.000000 cryptopian_infra-0.1.1/src/cryptopian_infra.egg-info/SOURCES.txt
--rw-r--r--   0 wuhan      (501) staff       (20)        1 2024-03-31 15:41:58.000000 cryptopian_infra-0.1.1/src/cryptopian_infra.egg-info/dependency_links.txt
--rw-r--r--   0 wuhan      (501) staff       (20)       75 2024-03-31 15:41:58.000000 cryptopian_infra-0.1.1/src/cryptopian_infra.egg-info/requires.txt
--rw-r--r--   0 wuhan      (501) staff       (20)       17 2024-03-31 15:41:58.000000 cryptopian_infra-0.1.1/src/cryptopian_infra.egg-info/top_level.txt
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-03-31 15:41:58.664503 cryptopian_infra-0.1.1/tests/
--rw-r--r--   0 wuhan      (501) staff       (20)      601 2024-03-06 06:30:32.000000 cryptopian_infra-0.1.1/tests/test_random.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.183656 cryptopian_infra-0.1.2/
+-rw-r--r--   0 wuhan      (501) staff       (20)     1063 2022-01-19 16:43:46.000000 cryptopian_infra-0.1.2/LICENSE
+-rw-r--r--   0 wuhan      (501) staff       (20)     1187 2024-04-03 04:37:30.183373 cryptopian_infra-0.1.2/PKG-INFO
+-rw-r--r--   0 wuhan      (501) staff       (20)      446 2024-03-07 06:40:10.000000 cryptopian_infra-0.1.2/README.md
+-rw-r--r--   0 wuhan      (501) staff       (20)      690 2024-04-03 04:37:04.000000 cryptopian_infra-0.1.2/pyproject.toml
+-rw-r--r--   0 wuhan      (501) staff       (20)       38 2024-04-03 04:37:30.183852 cryptopian_infra-0.1.2/setup.cfg
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.172361 cryptopian_infra-0.1.2/src/
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.173713 cryptopian_infra-0.1.2/src/cryptopian_infra/
+-rw-r--r--   0 wuhan      (501) staff       (20)        0 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/__init__.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.176145 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/
+-rw-r--r--   0 wuhan      (501) staff       (20)      112 2024-03-31 08:31:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1512 2024-01-15 10:05:02.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/alert.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1819 2024-03-29 08:42:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/alertwrapper.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1221 2024-03-31 08:31:29.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/slackwebhook.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.178256 cryptopian_infra-0.1.2/src/cryptopian_infra/config/
+-rw-r--r--   0 wuhan      (501) staff       (20)      278 2024-03-12 15:01:14.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2057 2024-03-05 08:29:11.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/apimanager.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      872 2023-07-22 01:54:36.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/configloader.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      902 2022-05-08 03:39:06.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/docencryptionfactory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2555 2024-01-23 06:24:43.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/influxfactory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2341 2024-01-28 08:42:04.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/mongofactory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2799 2024-03-31 15:39:56.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/secretmanagerbase.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1878 2024-03-31 08:39:28.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/slackwebhookfactory.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.179263 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/
+-rw-r--r--   0 wuhan      (501) staff       (20)      145 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1403 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/duration.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2112 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/emailclient.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      169 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/gracefullystopdocker.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1013 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/stopwatch.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.179773 cryptopian_infra-0.1.2/src/cryptopian_infra/mongo/
+-rw-r--r--   0 wuhan      (501) staff       (20)       45 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/mongo/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1591 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/mongo/mongoparameters.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1071 2024-03-29 08:43:35.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/sendalert.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.180658 cryptopian_infra-0.1.2/src/cryptopian_infra/threading/
+-rw-r--r--   0 wuhan      (501) staff       (20)       80 2024-03-07 11:38:15.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/threading/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      421 2024-03-07 12:56:51.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/threading/atomicaccstore.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1303 2024-03-10 04:46:21.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/threading/messagepump.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.182297 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/
+-rw-r--r--   0 wuhan      (501) staff       (20)       51 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      346 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/asyncutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      626 2024-03-20 03:40:17.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/datetimeutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1017 2024-04-03 04:36:40.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/dictutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      133 2024-01-17 10:32:22.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/listutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1496 2024-03-05 04:22:42.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/mathutils.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.183061 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/
+-rw-r--r--   0 wuhan      (501) staff       (20)     1187 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/PKG-INFO
+-rw-r--r--   0 wuhan      (501) staff       (20)     1545 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/SOURCES.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)        1 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/dependency_links.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)       75 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/requires.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)       17 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/top_level.txt
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.182617 cryptopian_infra-0.1.2/tests/
+-rw-r--r--   0 wuhan      (501) staff       (20)      601 2024-03-06 06:30:32.000000 cryptopian_infra-0.1.2/tests/test_random.py
```

### Comparing `cryptopian_infra-0.1.1/LICENSE` & `cryptopian_infra-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/PKG-INFO` & `cryptopian_infra-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptopian_infra
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cryptopian Infrastructure Library
 Author-email: Han Wu <xjohnwu@gmail.com>
 Project-URL: Homepage, https://github.com/Cryptopian001/cryptopian_infrastructure_python
 Project-URL: Issues, https://github.com/Cryptopian001/cryptopian_infrastructure_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cryptopian_infra-0.1.1/pyproject.toml` & `cryptopian_infra-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cryptopian_infra"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "Han Wu", email = "xjohnwu@gmail.com" },
 ]
 dependencies = [
     "influxdb",
     "jsmin",
     "onepasswordconnectsdk",
```

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/alert/alert.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/alert/alert.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/alert/alertwrapper.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/alert/alertwrapper.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/alert/slackwebhook.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/alert/slackwebhook.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/config/apimanager.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/config/apimanager.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/config/configloader.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/config/configloader.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/config/docencryptionfactory.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/config/docencryptionfactory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/config/influxfactory.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/config/influxfactory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/config/mongofactory.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/config/mongofactory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/config/secretmanagerbase.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/config/secretmanagerbase.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/config/slackwebhookfactory.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/config/slackwebhookfactory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/infra/duration.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/infra/duration.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/infra/emailclient.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/infra/emailclient.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/infra/stopwatch.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/infra/stopwatch.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/mongo/mongoparameters.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/mongo/mongoparameters.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/sendalert.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/sendalert.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/threading/messagepump.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/threading/messagepump.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/utils/datetimeutils.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/utils/datetimeutils.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/utils/dictutils.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/utils/dictutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from copy import deepcopy
+from decimal import Decimal
 
 
 def merge_dict(base_dict: dict, override_dict: dict):
     result = deepcopy(base_dict)
     for key, value in override_dict.items():
         if key not in result:
             result[key] = value
         else:
-            assert isinstance(base_dict[key], type(value)) and isinstance(value, type(base_dict[key])), key
+            numeric_types = [int, float, Decimal]
+            assert ((isinstance(base_dict[key], type(value)) and isinstance(value, type(base_dict[key]))) or
+                    type(value) in numeric_types and type(base_dict[key]) in numeric_types), f"Unmatched types for key '{key}'"
             if type(value) is dict:
                 result[key] = merge_dict(base_dict[key], value)
             else:
                 result[key] = value
     return result
```

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra/utils/mathutils.py` & `cryptopian_infra-0.1.2/src/cryptopian_infra/utils/mathutils.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra.egg-info/PKG-INFO` & `cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptopian_infra
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cryptopian Infrastructure Library
 Author-email: Han Wu <xjohnwu@gmail.com>
 Project-URL: Homepage, https://github.com/Cryptopian001/cryptopian_infrastructure_python
 Project-URL: Issues, https://github.com/Cryptopian001/cryptopian_infrastructure_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cryptopian_infra-0.1.1/src/cryptopian_infra.egg-info/SOURCES.txt` & `cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.1/tests/test_random.py` & `cryptopian_infra-0.1.2/tests/test_random.py`

 * *Files identical despite different names*

