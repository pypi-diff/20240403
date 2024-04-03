# Comparing `tmp/clap-detector-2.0.2.tar.gz` & `tmp/clap-detector-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clap-detector-2.0.2.tar", last modified: Wed Apr  3 04:23:23 2024, max compression
+gzip compressed data, was "clap-detector-2.0.3.tar", last modified: Wed Apr  3 04:38:16 2024, max compression
```

## Comparing `clap-detector-2.0.2.tar` & `clap-detector-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:23:23.977150 clap-detector-2.0.2/
--rw-rw-rw-   0        0        0     1090 2024-04-03 02:43:53.000000 clap-detector-2.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3327 2024-04-03 04:23:23.975236 clap-detector-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2850 2024-04-03 04:06:50.000000 clap-detector-2.0.2/README.md
--rw-rw-rw-   0        0        0      138 2024-04-03 03:43:06.000000 clap-detector-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 04:23:23.977666 clap-detector-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      771 2024-04-03 03:56:37.000000 clap-detector-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:23:23.935430 clap-detector-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 04:23:23.951837 clap-detector-2.0.2/src/clapDetector/
--rw-rw-rw-   0        0        0        0 2024-04-03 03:12:20.000000 clap-detector-2.0.2/src/clapDetector/__init__.py
--rw-rw-rw-   0        0        0    17669 2024-04-03 03:05:31.000000 clap-detector-2.0.2/src/clapDetector/clapDetector.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:23:23.973806 clap-detector-2.0.2/src/clap_detector.egg-info/
--rw-rw-rw-   0        0        0     3327 2024-04-03 04:23:23.000000 clap-detector-2.0.2/src/clap_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-03 04:23:23.000000 clap-detector-2.0.2/src/clap_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:23:23.000000 clap-detector-2.0.2/src/clap_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-03 04:23:23.000000 clap-detector-2.0.2/src/clap_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 04:38:16.044336 clap-detector-2.0.3/
+-rw-rw-rw-   0        0        0     1090 2024-04-03 02:43:53.000000 clap-detector-2.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3327 2024-04-03 04:38:16.041357 clap-detector-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2850 2024-04-03 04:06:50.000000 clap-detector-2.0.3/README.md
+-rw-rw-rw-   0        0        0      138 2024-04-03 03:43:06.000000 clap-detector-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 04:38:16.044336 clap-detector-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      771 2024-04-03 04:37:54.000000 clap-detector-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:38:15.994794 clap-detector-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 04:38:16.011785 clap-detector-2.0.3/src/clapDetector/
+-rw-rw-rw-   0        0        0       38 2024-04-03 04:29:52.000000 clap-detector-2.0.3/src/clapDetector/__init__.py
+-rw-rw-rw-   0        0        0    17669 2024-04-03 03:05:31.000000 clap-detector-2.0.3/src/clapDetector/clapDetector.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:38:16.038361 clap-detector-2.0.3/src/clap_detector.egg-info/
+-rw-rw-rw-   0        0        0     3327 2024-04-03 04:38:15.000000 clap-detector-2.0.3/src/clap_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-03 04:38:15.000000 clap-detector-2.0.3/src/clap_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 04:38:15.000000 clap-detector-2.0.3/src/clap_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-03 04:38:15.000000 clap-detector-2.0.3/src/clap_detector.egg-info/top_level.txt
```

### Comparing `clap-detector-2.0.2/LICENSE.txt` & `clap-detector-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clap-detector-2.0.2/PKG-INFO` & `clap-detector-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clap-detector
-Version: 2.0.2
+Version: 2.0.3
 Summary: A clap detector that can detect claps in patterns of single, double, etc.
 Home-page: https://github.com/TzurSoffer/clapDetection
 Author: Tzur Soffer
 Author-email: tzur.soffer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clap-detector-2.0.2/README.md` & `clap-detector-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `clap-detector-2.0.2/setup.py` & `clap-detector-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "clap-detector",
-    version = "2.0.2",
+    version = "2.0.3",
     author = "Tzur Soffer",
     author_email = "tzur.soffer@gmail.com",
     description = "A clap detector that can detect claps in patterns of single, double, etc.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/TzurSoffer/clapDetection",
     classifiers = [
```

### Comparing `clap-detector-2.0.2/src/clapDetector/clapDetector.py` & `clap-detector-2.0.3/src/clapDetector/clapDetector.py`

 * *Files identical despite different names*

### Comparing `clap-detector-2.0.2/src/clap_detector.egg-info/PKG-INFO` & `clap-detector-2.0.3/src/clap_detector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clap-detector
-Version: 2.0.2
+Version: 2.0.3
 Summary: A clap detector that can detect claps in patterns of single, double, etc.
 Home-page: https://github.com/TzurSoffer/clapDetection
 Author: Tzur Soffer
 Author-email: tzur.soffer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

