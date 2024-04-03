# Comparing `tmp/smadi-0.2.5.tar.gz` & `tmp/smadi-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smadi-0.2.5.tar", last modified: Tue Apr  2 00:50:29 2024, max compression
+gzip compressed data, was "smadi-0.2.6.tar", last modified: Wed Apr  3 02:38:35 2024, max compression
```

## Comparing `smadi-0.2.5.tar` & `smadi-0.2.6.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.946805 smadi-0.2.5/
--rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.5/.coveragerc
--rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.5/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.5/.readthedocs.yml
--rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.5/AUTHORS.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.5/CHANGELOG.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.5/CONTRIBUTING.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.5/LICENSE.txt
--rw-r--r--   0 m294      (1000) m294      (1000)     2982 2024-04-02 00:50:29.946805 smadi-0.2.5/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)     1591 2024-03-30 14:53:43.000000 smadi-0.2.5/README.rst
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.898804 smadi-0.2.5/docs/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/Makefile
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.898804 smadi-0.2.5/docs/_static/
--rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/_static/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/authors.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/changelog.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     9724 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/conf.py
--rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/contributing.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/index.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/license.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/readme.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      233 2024-03-30 14:53:43.000000 smadi-0.2.5/docs/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.5/pyproject.toml
--rw-rw-r--   0 m294      (1000) m294      (1000)     1479 2024-04-02 00:50:29.950805 smadi-0.2.5/setup.cfg
--rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-02 00:50:00.000000 smadi-0.2.5/setup.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.878804 smadi-0.2.5/src/
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.902804 smadi-0.2.5/src/smadi/
--rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.5/src/smadi/__init__.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    19649 2024-04-01 23:41:33.000000 smadi-0.2.5/src/smadi/anomaly_detectors.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    15269 2024-03-30 15:08:13.000000 smadi-0.2.5/src/smadi/climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-03-29 20:29:27.000000 smadi-0.2.5/src/smadi/data_reader.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8775 2024-03-29 20:29:06.000000 smadi-0.2.5/src/smadi/indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     5258 2024-03-30 14:57:24.000000 smadi-0.2.5/src/smadi/map.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     1813 2024-04-01 23:41:33.000000 smadi-0.2.5/src/smadi/metadata.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     7461 2024-03-30 14:58:05.000000 smadi-0.2.5/src/smadi/plot.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8623 2024-03-29 20:28:21.000000 smadi-0.2.5/src/smadi/preprocess.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     4522 2024-04-01 23:09:32.000000 smadi-0.2.5/src/smadi/utils.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    14711 2024-04-01 23:41:33.000000 smadi-0.2.5/src/smadi/workflow.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.946805 smadi-0.2.5/src/smadi.egg-info/
--rw-r--r--   0 m294      (1000) m294      (1000)     2982 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)      898 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/SOURCES.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/dependency_links.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/entry_points.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-03-30 15:01:49.000000 smadi-0.2.5/src/smadi.egg-info/not-zip-safe
--rw-rw-r--   0 m294      (1000) m294      (1000)      315 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/requires.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-02 00:50:29.000000 smadi-0.2.5/src/smadi.egg-info/top_level.txt
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-02 00:50:29.946805 smadi-0.2.5/tests/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.5/tests/conftest.py
--rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.5/tests/data_sample.csv
--rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.5/tests/test_climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.5/tests/test_indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.5/tox.ini
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.956905 smadi-0.2.6/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.6/.coveragerc
+-rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.6/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.6/.readthedocs.yml
+-rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.6/AUTHORS.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.6/CHANGELOG.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.6/CONTRIBUTING.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.6/LICENSE.txt
+-rw-r--r--   0 m294      (1000) m294      (1000)     3009 2024-04-03 02:38:35.956905 smadi-0.2.6/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1591 2024-03-30 14:53:43.000000 smadi-0.2.6/README.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)  1710114 2024-04-03 02:37:06.000000 smadi-0.2.6/Tutorial.ipynb
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.860905 smadi-0.2.6/docs/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/Makefile
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.860905 smadi-0.2.6/docs/_static/
+-rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/_static/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/authors.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/changelog.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9724 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/conf.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/contributing.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/index.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/license.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/readme.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      233 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.6/pyproject.toml
+-rw-rw-r--   0 m294      (1000) m294      (1000)      301 2024-04-03 02:37:06.000000 smadi-0.2.6/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1492 2024-04-03 02:38:35.956905 smadi-0.2.6/setup.cfg
+-rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-03 02:38:11.000000 smadi-0.2.6/setup.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.760904 smadi-0.2.6/src/
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.864904 smadi-0.2.6/src/smadi/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.6/src/smadi/__init__.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    19649 2024-04-01 23:41:33.000000 smadi-0.2.6/src/smadi/anomaly_detectors.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    15611 2024-04-03 02:37:06.000000 smadi-0.2.6/src/smadi/climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-04-02 14:59:26.000000 smadi-0.2.6/src/smadi/data_reader.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8775 2024-03-29 20:29:06.000000 smadi-0.2.6/src/smadi/indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     5213 2024-04-03 02:37:06.000000 smadi-0.2.6/src/smadi/map.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1813 2024-04-01 23:41:33.000000 smadi-0.2.6/src/smadi/metadata.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     7719 2024-04-03 02:37:06.000000 smadi-0.2.6/src/smadi/plot.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8623 2024-03-29 20:28:21.000000 smadi-0.2.6/src/smadi/preprocess.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     4522 2024-04-01 23:09:32.000000 smadi-0.2.6/src/smadi/utils.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    14908 2024-04-03 02:37:06.000000 smadi-0.2.6/src/smadi/workflow.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.952905 smadi-0.2.6/src/smadi.egg-info/
+-rw-r--r--   0 m294      (1000) m294      (1000)     3009 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)      930 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/entry_points.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-03-30 15:01:49.000000 smadi-0.2.6/src/smadi.egg-info/not-zip-safe
+-rw-rw-r--   0 m294      (1000) m294      (1000)      327 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/requires.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/top_level.txt
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.952905 smadi-0.2.6/tests/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.6/tests/conftest.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.6/tests/data_sample.csv
+-rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.6/tests/test_climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.6/tests/test_indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.6/tox.ini
```

### Comparing `smadi-0.2.5/.coveragerc` & `smadi-0.2.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/.gitignore` & `smadi-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/.readthedocs.yml` & `smadi-0.2.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/CONTRIBUTING.rst` & `smadi-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/LICENSE.txt` & `smadi-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/PKG-INFO` & `smadi-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smadi
-Version: 0.2.5
+Version: 0.2.6
 Summary: Add a short description here!
 Home-page: https://github.com/MuhammedM294/smadi
 Author: MuhammedM294
 Author-email: muhammedaabdelaal@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/MuhammedM294/smadi
@@ -38,14 +38,15 @@
 Requires-Dist: pynetcf
 Requires-Dist: cmcrameri
 Requires-Dist: fibgrid
 Requires-Dist: datashader
 Requires-Dist: pycountry
 Requires-Dist: PyQt5
 Requires-Dist: PySide2
+Requires-Dist: mapclassify
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
```

### Comparing `smadi-0.2.5/README.rst` & `smadi-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/docs/Makefile` & `smadi-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/docs/conf.py` & `smadi-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/docs/index.rst` & `smadi-0.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/setup.cfg` & `smadi-0.2.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 	pynetcf
 	cmcrameri
 	fibgrid
 	datashader
 	pycountry
 	PyQt5
 	PySide2
+	mapclassify
 	importlib-metadata; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `smadi-0.2.5/setup.py` & `smadi-0.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(
-            version="0.2.5",
+            version="0.2.6",
             entry_points={
                 "console_scripts": [
                     "run = smadi.workflow:main",
                 ]
             },
         )
```

### Comparing `smadi-0.2.5/src/smadi/__init__.py` & `smadi-0.2.6/src/smadi/__init__.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/src/smadi/anomaly_detectors.py` & `smadi-0.2.6/src/smadi/anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/src/smadi/climatology.py` & `smadi-0.2.6/src/smadi/climatology.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,48 +90,65 @@
         smooth_window_size=None,
         timespan: List[str] = None,
     ):
         """
         Initializes the Aggregation class.
 
         """
-
         self.original_df = df
         self.var = variable
         self.fillna = fillna
         self.fillna_window_size = fillna_window_size
         self.smoothing = smoothing
         self.smooth_window_size = smooth_window_size
         self.timespan = timespan
-
         self._validate_input()
-        self.df = pd.DataFrame(self.original_df[self.var]).resample("D").mean()
-        self.df = (
-            self.df.truncate(before=timespan[0], after=timespan[1])
-            if timespan
-            else self.df
-        )
-        self._fillna()
-        self._smooth()
-        self.df.dropna(inplace=True)
         self.resulted_df = pd.DataFrame()
 
-    def _fillna(self):
+    @property
+    def df(self):
+        """
+        Prepares the DataFrame for aggregation.
+        """
+
+        # Resample the data to daily frequency
+        _df = pd.DataFrame(self.original_df[self.var]).resample("D").mean()
+
+        # Truncate the data based on the timespan provided
+        _df = (
+            _df.truncate(before=self.timespan[0], after=self.timespan[1])
+            if self.timespan
+            else _df
+        )
+
+        # Validate the input parameters
+        self._validate_input()
+        _df = self._fillna(_df)
+        _df = self._smooth(_df)
+        _df.dropna(inplace=True)
+
+        return _df
+
+    def _fillna(self, df):
         """
         Fills NaN values in the time series data using a moving window average.
         """
         if self.fillna:
-            self.df[self.var] = fillna(self.df, self.var, self.fillna_window_size)
+            df[self.var] = fillna(df, self.var, self.fillna_window_size)
+
+        return df
 
-    def _smooth(self):
+    def _smooth(self, df):
         """
         Smooths the time series data using a moving window average.
         """
         if self.smoothing:
-            self.df[self.var] = smooth(self.df, self.var, self.smooth_window_size)
+            df[self.var] = smooth(df, self.var, self.smooth_window_size)
+
+        return df
 
     def _validate_df_index(self):
         """
         Validates the input DataFrame type and index.
 
         Raises:
         -------
```

### Comparing `smadi-0.2.5/src/smadi/data_reader.py` & `smadi-0.2.6/src/smadi/data_reader.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/src/smadi/indicators.py` & `smadi-0.2.6/src/smadi/indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/src/smadi/map.py` & `smadi-0.2.6/src/smadi/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-import matplotlib
 import eomaps
-
 from smadi.metadata import indicators_thresholds
 
-matplotlib.use("Qt5Agg")
-
 
 def set_thresholds(method):
     """
     Set the thresholds for the specified method based on the method name.
 
     parameters:
     -----------
```

### Comparing `smadi-0.2.5/src/smadi/metadata.py` & `smadi-0.2.6/src/smadi/metadata.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/src/smadi/plot.py` & `smadi-0.2.6/src/smadi/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import matplotlib
 import matplotlib.pyplot as plt
 
 
 from smadi.anomaly_detectors import *
 from smadi.metadata import indicators_thresholds
 
-matplotlib.use("Qt5Agg")
-
 
 def get_plot_options(**kwargs):
     """
     Set the basic plot options based on the provided kwargs for the plot.
 
     parameters:
     -----------
@@ -29,15 +27,17 @@
         "title": kwargs.get("title", None),
         "xlabel": kwargs.get("xlabel", None),
         "ylabel": kwargs.get("ylabel", None),
         "legend": kwargs.get("legend", None),
         "legend_labels": kwargs.get("legend_labels", None),
         "figsize": kwargs.get("figsize", None),
         "grid": kwargs.get("grid", None),
+        "savefig": kwargs.get("savefig", None),
     }
+
     return plot_options
 
 
 def plot_figure(plot_params):
     """
     Plot the figure based on the provided plot parameters.
 
@@ -60,14 +60,16 @@
             plt.legend(plot_params["legend_labels"])
         else:
             plt.legend()
 
     # Show plot
     plt.grid(plot_params["grid"])
     plt.tight_layout()
+    if plot_params["savefig"] is not None:
+        plt.savefig(plot_params["savefig"])
     plt.show()
 
 
 def plot_colmns(df, x_axis, colmns_kwargs):
     """
     Plot the data in each column of the dataframe with the provided x_axis.
 
@@ -128,19 +130,22 @@
     columns: dict
         The dictionary containing the column names and their respective matplotlib plot options.
 
     thresholds: str
         The name of the anomaly method to use its thresholds.
     """
 
-    category_counter = {}
     results = []
     anomaly_thresholds = indicators_thresholds[thresholds]
 
+    if len(columns) > 2:
+        raise ValueError("The number of columns should not exceed 2.")
+
     for colm, _ in columns.items():
+        category_counter = {}
         for key, value in anomaly_thresholds.items():
             category_counter[key] = df[colm].between(value[0], value[1]).sum()
 
         results.append(category_counter)
 
     return results
 
@@ -265,15 +270,16 @@
 
     **kwargs: dict
         The keyword arguments for the matplotlib plot for the figure such as title, xlabel, ylabel, legend, figsize, and grid.
 
     """
     # Set values for kwargs based on provided values
     plot_params = get_plot_options(**kwargs)
-    plt.figure(figsize=plot_params["figsize"])
+    if plot_params["figsize"] is not None:
+        plt.figure(figsize=plot_params["figsize"])
 
     if plot_raw:
         plt.plot(
             clim_obj.original_df.index,
             clim_obj.original_df[raw_var],
             **raw_kwargs if raw_kwargs else {},
         )
```

### Comparing `smadi-0.2.5/src/smadi/preprocess.py` & `smadi-0.2.6/src/smadi/preprocess.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/src/smadi/utils.py` & `smadi-0.2.6/src/smadi/utils.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/src/smadi/workflow.py` & `smadi-0.2.6/src/smadi/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,20 @@
         default="month",
         choices=["month", "dekad", "week", "bimonth", "day"],
         help="The time step for the climatology calculation. Supported values: month, dekad, week, bimonth, day",
     )
 
     # Optional arguments
     parser.add_argument(
+        "--data_read_bulk",
+        type=bool,
+        default=False,
+        help="Read data in bulk mode. If 'True' all data will be read in memory",
+    )
+    parser.add_argument(
         "--variable",
         metavar="variable",
         type=str,
         default="sm",
         help="The variable to be used for the anomaly detection.",
     )
     parser.add_argument(
@@ -166,14 +172,15 @@
 aoi = args.aoi
 if "," in aoi:
     aoi = tuple(map(float, aoi.split(",")))
 variable = args.variable
 time_step = args.time_step
 
 # Optional parameters
+data_read_bulk = args.data_read_bulk
 methods = args.methods
 workers = args.workers
 fillna = args.fillna
 fillna_window_size = args.fillna_size
 smoothing = args.smoothing
 smooth_window_size = args.smooth_size
 timespan = args.timespan
@@ -182,15 +189,15 @@
 dekad = args.dekad
 week = args.week
 bimonth = args.bimonth
 day = args.day
 save_to = args.save_to
 
 # Create an instance of the AscatData class
-ascat_obj = AscatData(data_path, False)
+ascat_obj = AscatData(data_path, data_read_bulk)
 
 # Create a logger
 logger = create_logger("run_logger")
 
 
 @log_exception(logger)
 def load_ts(gpi, variable="sm"):
@@ -424,15 +431,14 @@
         pointlist = load_gpis_by_country(aoi)
     else:
         pointlist = get_gpis_from_bbox(aoi)
 
     print(f"Grid points loaded successfully for {aoi}\n")
     print(pointlist.head())
     print("\n")
-    pointlist = pointlist[:100]
     pre_compute = partial(
         single_po_run,
         methods=methods,
         variable=variable,
         time_step=time_step,
         fillna=fillna,
         fillna_window_size=fillna_window_size,
```

### Comparing `smadi-0.2.5/src/smadi.egg-info/PKG-INFO` & `smadi-0.2.6/src/smadi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smadi
-Version: 0.2.5
+Version: 0.2.6
 Summary: Add a short description here!
 Home-page: https://github.com/MuhammedM294/smadi
 Author: MuhammedM294
 Author-email: muhammedaabdelaal@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/MuhammedM294/smadi
@@ -38,14 +38,15 @@
 Requires-Dist: pynetcf
 Requires-Dist: cmcrameri
 Requires-Dist: fibgrid
 Requires-Dist: datashader
 Requires-Dist: pycountry
 Requires-Dist: PyQt5
 Requires-Dist: PySide2
+Requires-Dist: mapclassify
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
```

### Comparing `smadi-0.2.5/src/smadi.egg-info/SOURCES.txt` & `smadi-0.2.6/src/smadi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 .gitignore
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
+Tutorial.ipynb
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
```

### Comparing `smadi-0.2.5/tests/conftest.py` & `smadi-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/tests/data_sample.csv` & `smadi-0.2.6/tests/data_sample.csv`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/tests/test_climatology.py` & `smadi-0.2.6/tests/test_climatology.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/tests/test_indicators.py` & `smadi-0.2.6/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.5/tox.ini` & `smadi-0.2.6/tox.ini`

 * *Files identical despite different names*

