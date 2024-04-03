# Comparing `tmp/hio-0.6.8.tar.gz` & `tmp/hio-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hio-0.6.8.tar", last modified: Wed Nov  2 22:01:42 2022, max compression
+gzip compressed data, was "hio-0.6.9.tar", last modified: Sun Nov 27 03:09:46 2022, max compression
```

## Comparing `hio-0.6.8.tar` & `hio-0.6.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.067170 hio-0.6.8/
--rw-rw-r--   0 samuel    (2020) staff       (20)    11357 2022-04-25 16:20:18.000000 hio-0.6.8/LICENSE
--rw-rw-r--   0 samuel    (2020) staff       (20)     1151 2022-11-02 22:01:42.067040 hio-0.6.8/PKG-INFO
--rw-rw-r--   0 samuel    (2020) staff       (20)     3742 2022-04-25 16:20:18.000000 hio-0.6.8/README.md
--rw-rw-r--   0 samuel    (2020) staff       (20)       38 2022-11-02 22:01:42.067203 hio-0.6.8/setup.cfg
--rw-rw-r--   0 samuel    (2020) staff       (20)     3420 2022-11-02 21:45:04.000000 hio-0.6.8/setup.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.058175 hio-0.6.8/src/
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.059890 hio-0.6.8/src/hio/
--rw-rw-r--   0 samuel    (2020) staff       (20)      164 2022-11-02 21:44:56.000000 hio-0.6.8/src/hio/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)      310 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/__main__.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.062327 hio-0.6.8/src/hio/base/
--rw-rw-r--   0 samuel    (2020) staff       (20)      194 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/base/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)      282 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/base/basing.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    56182 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/base/doing.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    17164 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/base/filing.py
--rw-rw-r--   0 samuel    (2020) staff       (20)     9022 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/base/tyming.py
--rw-rw-r--   0 samuel    (2020) staff       (20)      971 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/cli.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.063048 hio-0.6.8/src/hio/core/
--rw-rw-r--   0 samuel    (2020) staff       (20)      101 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)     4945 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/coring.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.063960 hio-0.6.8/src/hio/core/http/
--rw-rw-r--   0 samuel    (2020) staff       (20)      217 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/http/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    50573 2022-11-02 21:30:59.000000 hio-0.6.8/src/hio/core/http/clienting.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    32568 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/http/httping.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    48034 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/http/serving.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.064306 hio-0.6.8/src/hio/core/serial/
--rw-rw-r--   0 samuel    (2020) staff       (20)       89 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/serial/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    20300 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/serial/serialing.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.065225 hio-0.6.8/src/hio/core/tcp/
--rw-rw-r--   0 samuel    (2020) staff       (20)      209 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/tcp/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    24684 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/tcp/clienting.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    36354 2022-06-17 01:11:17.000000 hio-0.6.8/src/hio/core/tcp/serving.py
--rw-rw-r--   0 samuel    (2020) staff       (20)      408 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/tcp/tcping.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.065452 hio-0.6.8/src/hio/core/udp/
--rw-rw-r--   0 samuel    (2020) staff       (20)       57 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/udp/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)     5082 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/udp/udping.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    18975 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/core/wiring.py
--rw-rw-r--   0 samuel    (2020) staff       (20)      391 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/daemon.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.065568 hio-0.6.8/src/hio/demo/
--rw-rw-r--   0 samuel    (2020) staff       (20)       85 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/demo/__init__.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.065897 hio-0.6.8/src/hio/demo/web/
--rw-rw-r--   0 samuel    (2020) staff       (20)       93 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/demo/web/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)     1383 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/demo/web/demo_web.py
--rw-rw-r--   0 samuel    (2020) staff       (20)      202 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/demo/web/demoing.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.066842 hio-0.6.8/src/hio/help/
--rw-rw-r--   0 samuel    (2020) staff       (20)      602 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/help/__init__.py
--rw-rw-r--   0 samuel    (2020) staff       (20)     3216 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/help/decking.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    13292 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/help/helping.py
--rw-rw-r--   0 samuel    (2020) staff       (20)     6976 2022-05-05 19:38:33.000000 hio-0.6.8/src/hio/help/hicting.py
--rw-rw-r--   0 samuel    (2020) staff       (20)    13762 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/help/ogling.py
--rw-rw-r--   0 samuel    (2020) staff       (20)     6777 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/help/timing.py
--rw-rw-r--   0 samuel    (2020) staff       (20)     1269 2022-04-25 16:20:18.000000 hio-0.6.8/src/hio/hioing.py
-drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-02 22:01:42.061037 hio-0.6.8/src/hio.egg-info/
--rw-rw-r--   0 samuel    (2020) staff       (20)     1151 2022-11-02 22:01:42.000000 hio-0.6.8/src/hio.egg-info/PKG-INFO
--rw-rw-r--   0 samuel    (2020) staff       (20)     1130 2022-11-02 22:01:42.000000 hio-0.6.8/src/hio.egg-info/SOURCES.txt
--rw-rw-r--   0 samuel    (2020) staff       (20)        1 2022-11-02 22:01:42.000000 hio-0.6.8/src/hio.egg-info/dependency_links.txt
--rw-rw-r--   0 samuel    (2020) staff       (20)       60 2022-11-02 22:01:42.000000 hio-0.6.8/src/hio.egg-info/entry_points.txt
--rw-rw-r--   0 samuel    (2020) staff       (20)        1 2022-04-25 16:22:45.000000 hio-0.6.8/src/hio.egg-info/not-zip-safe
--rw-rw-r--   0 samuel    (2020) staff       (20)      139 2022-11-02 22:01:42.000000 hio-0.6.8/src/hio.egg-info/requires.txt
--rw-rw-r--   0 samuel    (2020) staff       (20)        4 2022-11-02 22:01:42.000000 hio-0.6.8/src/hio.egg-info/top_level.txt
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.360010 hio-0.6.9/
+-rw-rw-r--   0 samuel    (2020) staff       (20)    11357 2022-04-25 16:20:18.000000 hio-0.6.9/LICENSE
+-rw-rw-r--   0 samuel    (2020) staff       (20)     1151 2022-11-27 03:09:46.359896 hio-0.6.9/PKG-INFO
+-rw-rw-r--   0 samuel    (2020) staff       (20)     3742 2022-04-25 16:20:18.000000 hio-0.6.9/README.md
+-rw-rw-r--   0 samuel    (2020) staff       (20)       38 2022-11-27 03:09:46.360042 hio-0.6.9/setup.cfg
+-rw-rw-r--   0 samuel    (2020) staff       (20)     3420 2022-11-27 01:54:49.000000 hio-0.6.9/setup.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.352633 hio-0.6.9/src/
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.354683 hio-0.6.9/src/hio/
+-rw-rw-r--   0 samuel    (2020) staff       (20)      164 2022-11-27 01:54:56.000000 hio-0.6.9/src/hio/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)      310 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/__main__.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.356169 hio-0.6.9/src/hio/base/
+-rw-rw-r--   0 samuel    (2020) staff       (20)      194 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/base/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)      282 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/base/basing.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    56182 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/base/doing.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    17164 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/base/filing.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)     9022 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/base/tyming.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)      971 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/cli.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.356498 hio-0.6.9/src/hio/core/
+-rw-rw-r--   0 samuel    (2020) staff       (20)      101 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)     4945 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/coring.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.357007 hio-0.6.9/src/hio/core/http/
+-rw-rw-r--   0 samuel    (2020) staff       (20)      217 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/http/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    51553 2022-11-27 01:37:20.000000 hio-0.6.9/src/hio/core/http/clienting.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    32568 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/http/httping.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    48034 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/http/serving.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.357411 hio-0.6.9/src/hio/core/serial/
+-rw-rw-r--   0 samuel    (2020) staff       (20)       89 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/serial/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    20300 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/serial/serialing.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.358190 hio-0.6.9/src/hio/core/tcp/
+-rw-rw-r--   0 samuel    (2020) staff       (20)      209 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/tcp/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    24684 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/tcp/clienting.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    36354 2022-06-17 01:11:17.000000 hio-0.6.9/src/hio/core/tcp/serving.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)      408 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/tcp/tcping.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.358463 hio-0.6.9/src/hio/core/udp/
+-rw-rw-r--   0 samuel    (2020) staff       (20)       57 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/udp/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)     5082 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/udp/udping.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    18975 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/core/wiring.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)      391 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/daemon.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.358596 hio-0.6.9/src/hio/demo/
+-rw-rw-r--   0 samuel    (2020) staff       (20)       85 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/demo/__init__.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.358994 hio-0.6.9/src/hio/demo/web/
+-rw-rw-r--   0 samuel    (2020) staff       (20)       93 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/demo/web/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)     1383 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/demo/web/demo_web.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)      202 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/demo/web/demoing.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.359735 hio-0.6.9/src/hio/help/
+-rw-rw-r--   0 samuel    (2020) staff       (20)      602 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/help/__init__.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)     3216 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/help/decking.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    13292 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/help/helping.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)     6976 2022-05-05 19:38:33.000000 hio-0.6.9/src/hio/help/hicting.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)    13762 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/help/ogling.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)     6777 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/help/timing.py
+-rw-rw-r--   0 samuel    (2020) staff       (20)     1269 2022-04-25 16:20:18.000000 hio-0.6.9/src/hio/hioing.py
+drwxrwxr-x   0 samuel    (2020) staff       (20)        0 2022-11-27 03:09:46.355558 hio-0.6.9/src/hio.egg-info/
+-rw-rw-r--   0 samuel    (2020) staff       (20)     1151 2022-11-27 03:09:46.000000 hio-0.6.9/src/hio.egg-info/PKG-INFO
+-rw-rw-r--   0 samuel    (2020) staff       (20)     1130 2022-11-27 03:09:46.000000 hio-0.6.9/src/hio.egg-info/SOURCES.txt
+-rw-rw-r--   0 samuel    (2020) staff       (20)        1 2022-11-27 03:09:46.000000 hio-0.6.9/src/hio.egg-info/dependency_links.txt
+-rw-rw-r--   0 samuel    (2020) staff       (20)       60 2022-11-27 03:09:46.000000 hio-0.6.9/src/hio.egg-info/entry_points.txt
+-rw-rw-r--   0 samuel    (2020) staff       (20)        1 2022-04-25 16:22:45.000000 hio-0.6.9/src/hio.egg-info/not-zip-safe
+-rw-rw-r--   0 samuel    (2020) staff       (20)      139 2022-11-27 03:09:46.000000 hio-0.6.9/src/hio.egg-info/requires.txt
+-rw-rw-r--   0 samuel    (2020) staff       (20)        4 2022-11-27 03:09:46.000000 hio-0.6.9/src/hio.egg-info/top_level.txt
```

### Comparing `hio-0.6.8/LICENSE` & `hio-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/PKG-INFO` & `hio-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hio
-Version: 0.6.8
+Version: 0.6.9
 Summary: Hierarchical Concurrency with Async IO
 Home-page: https://github.com/ioflo/hio
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://hio.readthedocs.io/
 Project-URL: Changelog, https://hio.readthedocs.io/en/latest/changelog.html
```

### Comparing `hio-0.6.8/README.md` & `hio-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/setup.py` & `hio-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
 
 setup(
     name='hio',
-    version='0.6.8',  #  also change in src/hio/__init__.py
+    version='0.6.9',  #  also change in src/hio/__init__.py
     license='Apache Software License 2.0',
     description='Hierarchical Concurrency with Async IO',
     long_description=("HIO Hierarchical Concurrency and Asynchronous IO Library. "
                       "Rich structured contextual concurrrent coroutines with"
                       " asynchrounous IO modules."),
     author='Samuel M. Smith',
     author_email='smith.samuel.m@gmail.com',
```

### Comparing `hio-0.6.8/src/hio/base/doing.py` & `hio-0.6.9/src/hio/base/doing.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/base/filing.py` & `hio-0.6.9/src/hio/base/filing.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/base/tyming.py` & `hio-0.6.9/src/hio/base/tyming.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/cli.py` & `hio-0.6.9/src/hio/cli.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/core/coring.py` & `hio-0.6.9/src/hio/core/coring.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/core/http/clienting.py` & `hio-0.6.9/src/hio/core/http/clienting.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,43 +45,48 @@
                  method=u'GET',  # unicode
                  path=u'/',  # unicode
                  qargs=None,
                  fragment=u'', #unicode
                  headers=None,
                  body=b'',
                  data=None,
-                 fargs=None):
+                 fargs=None,
+                 portOptional=False):
         """
         Initialize Instance
 
         hostname = remote server hostname (may include port as hostname:port)
         port = remote server port
         scheme = http scheme 'http' or 'https' usually
         method = http request method verb
         path = http url path
         qargs = http query args
         fragment = http fragment
         headers = http request headers
         body = http request body
         data = dict to jsonify as body if provided
         fargs = dict to url form encode as body if provided
+        portOptional = True indicates to leave off port 80 for http or
+                        443 for https in Host header to support
+                        non-compliant server implementations.
         """
         self.hostname, self.port = httping.normalizeHostPort(hostname, port, 80)
         self.scheme = scheme
         self.method = method.upper() if method else u'GET'
         self.path = path or u'/'
         self.qargs = qargs if qargs is not None else dict()
         self.fragment = fragment
         self.headers = help.Hict(headers) if headers else help.Hict()
         if body and isinstance(body, str):  # use default
             # RFC 2616 Section 3.7.1 default charset of iso-8859-1.
             body = body.encode('iso-8859-1')
         self.body = body or b''
         self.data = data
         self.fargs = fargs
+        self.portOptional = True if portOptional else False
 
         self.lines = []  # keep around for testing
         self.head = b""  # keep around for testing
         self.msg = b""
 
     def reinit(self,
                hostname=None,
@@ -90,15 +95,16 @@
                method=None,  # unicode
                path=None,  # unicode
                qargs=None,
                fragment=None,
                headers=None,
                body=None,
                data=None,
-               fargs=None):
+               fargs=None,
+               portOptional=None):
         """
         Reinitialize anything that is not None
         This enables creating another request on a connection to the same host port
         """
         if hostname is not None: # may need to renormalize host port
             self.hostname = hostname
         if port is not None:
@@ -127,35 +133,40 @@
         else:
             self.data = None
         if fargs is not None:
             self.fargs = fargs
         else:
             self.fargs = None
 
+        if portOptional is not None:
+            self.portOptional = True if portOptional else False
+
     def rebuild(self,
                 method=None,
                 path=None,
                 qargs=None,
                 fragment=None,
                 headers=None,
                 body=None,
                 data=None,
-                fargs=None):
+                fargs=None,
+                portOptional=None):
         """
         Reinit then build and return request message
         This allows sending another request to same destination
         """
         self.reinit(method=method,
                     path=path,
                     qargs=qargs,
                     fragment=fragment,
                     headers=headers,
                     body=body,
                     data=data,
-                    fargs=fargs)
+                    fargs=fargs,
+                    portOptional=portOptional)
 
         return self.build()
 
 
     def build(self):
         """
         Build and return request message from attributes
@@ -208,15 +219,18 @@
             port = self.port
 
             # As per RFC 273, IPv6 address should be wrapped with []
             # when used as Host header
             if host.find(u':') >= 0:
                 host = u'[' + host + u']'
 
-            value = "{0}:{1}".format(host, port)
+            if self.portOptional and (self.scheme, port) in (("http", 80), ("https", 443)):
+                value = host # leave port empty when portOptional and one of defaults
+            else:
+                value = "{0}:{1}".format(host, port)
 
             try:
                 value = value.encode("ascii")
             except UnicodeEncodeError:
                 value = value.encode("idna")
 
             self.lines.append(httping.packHeader('Host', value))
@@ -656,14 +670,15 @@
                  requests=None,
                  msg=None,
                  dictable=None,
                  events=None,
                  redirectable=True,
                  redirects=None,
                  responses=None,
+                 portOptional=False,
                  **kwa):
         """
         Initialization method for instance.
         Parameters:
             connector is instance of tcp.Client or tcp.ClientTls or None
             requester is instance of Requester or None
             respondent is instance of Respondent or None
@@ -696,14 +711,16 @@
                 If True attempt to convert body from json
             events is reference to deque of events if any processed by respondent
             redirectable is Boolean to allow redirects to be processed by respondent
             redirects is list of redirects if any processed by respondent
                 each redirect is dict
             responses is deque of responses if any processed by respondent
                  each response is dict
+            portOptional = True indicates to leave off port 80 for http or
+                 443 for https in Host header to support non-compliant server implementations.
 
             **kwa are passed through to init .connector tcp.Client or tcp.ClientTLS
         """
         # .requests is deque of dicts of request data
         self.requests = requests if requests is not None else deque()
         # .responses is deque of dicts of response data
         self.responses = responses if responses is not None else deque()
@@ -794,15 +811,16 @@
                                   method=method,
                                   path=path,  # unicode
                                   headers=headers,
                                   qargs=qargs,
                                   fragment=fragment,
                                   body=body,
                                   data=data,
-                                  fargs=fargs)
+                                  fargs=fargs,
+                                  portOptional=portOptional)
         else:
             requester.reinit(hostname=self.connector.hostname,
                              port=self.connector.port,
                              scheme=scheme,
                              method=method,
                              path=path,
                              qargs=qargs,
```

### Comparing `hio-0.6.8/src/hio/core/http/httping.py` & `hio-0.6.9/src/hio/core/http/httping.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/core/http/serving.py` & `hio-0.6.9/src/hio/core/http/serving.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/core/serial/serialing.py` & `hio-0.6.9/src/hio/core/serial/serialing.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/core/tcp/clienting.py` & `hio-0.6.9/src/hio/core/tcp/clienting.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/core/tcp/serving.py` & `hio-0.6.9/src/hio/core/tcp/serving.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/core/udp/udping.py` & `hio-0.6.9/src/hio/core/udp/udping.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/core/wiring.py` & `hio-0.6.9/src/hio/core/wiring.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/demo/web/demo_web.py` & `hio-0.6.9/src/hio/demo/web/demo_web.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/help/__init__.py` & `hio-0.6.9/src/hio/help/__init__.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/help/decking.py` & `hio-0.6.9/src/hio/help/decking.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/help/helping.py` & `hio-0.6.9/src/hio/help/helping.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/help/hicting.py` & `hio-0.6.9/src/hio/help/hicting.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/help/ogling.py` & `hio-0.6.9/src/hio/help/ogling.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/help/timing.py` & `hio-0.6.9/src/hio/help/timing.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio/hioing.py` & `hio-0.6.9/src/hio/hioing.py`

 * *Files identical despite different names*

### Comparing `hio-0.6.8/src/hio.egg-info/PKG-INFO` & `hio-0.6.9/src/hio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hio
-Version: 0.6.8
+Version: 0.6.9
 Summary: Hierarchical Concurrency with Async IO
 Home-page: https://github.com/ioflo/hio
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://hio.readthedocs.io/
 Project-URL: Changelog, https://hio.readthedocs.io/en/latest/changelog.html
```

### Comparing `hio-0.6.8/src/hio.egg-info/SOURCES.txt` & `hio-0.6.9/src/hio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

