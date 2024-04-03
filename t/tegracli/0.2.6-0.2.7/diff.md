# Comparing `tmp/tegracli-0.2.6.tar.gz` & `tmp/tegracli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegracli-0.2.6.tar", max compression
+gzip compressed data, was "tegracli-0.2.7.tar", max compression
```

## Comparing `tegracli-0.2.6.tar` & `tegracli-0.2.7.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.6/LICENSE
--rw-r--r--   0        0        0    10186 2023-06-15 14:05:56.208264 tegracli-0.2.6/README.md
--rw-r--r--   0        0        0     1344 2023-06-15 14:05:56.208264 tegracli-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       88 2023-06-15 14:05:56.212264 tegracli-0.2.6/tegracli/__init__.py
--rw-r--r--   0        0        0     5666 2023-04-21 16:50:59.142072 tegracli-0.2.6/tegracli/dispatch.py
--rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.6/tegracli/group.py
--rw-r--r--   0        0        0    13930 2023-06-15 14:05:56.212264 tegracli-0.2.6/tegracli/main.py
--rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.6/tegracli/types.py
--rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.6/tegracli/utilities.py
--rw-r--r--   0        0        0    11211 1970-01-01 00:00:00.000000 tegracli-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.7/LICENSE
+-rw-r--r--   0        0        0    10186 2023-06-15 14:05:56.208264 tegracli-0.2.7/README.md
+-rw-r--r--   0        0        0     1109 2024-04-03 13:42:15.823736 tegracli-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      638 2023-06-22 07:27:50.527928 tegracli-0.2.7/tegracli/Makefile
+-rw-r--r--   0        0        0       88 2024-04-03 13:42:15.823736 tegracli-0.2.7/tegracli/__init__.py
+-rw-r--r--   0        0        0     5666 2023-04-21 16:50:59.142072 tegracli-0.2.7/tegracli/dispatch.py
+-rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.7/tegracli/group.py
+-rw-r--r--   0        0        0    13930 2023-06-15 14:05:56.212264 tegracli-0.2.7/tegracli/main.py
+-rw-r--r--   0        0        0      804 2023-06-22 07:27:50.531928 tegracli-0.2.7/tegracli/make.bat
+-rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.7/tegracli/types.py
+-rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.7/tegracli/utilities.py
+-rw-r--r--   0        0        0    11112 1970-01-01 00:00:00.000000 tegracli-0.2.7/PKG-INFO
```

### Comparing `tegracli-0.2.6/LICENSE` & `tegracli-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.6/README.md` & `tegracli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.6/tegracli/dispatch.py` & `tegracli-0.2.7/tegracli/dispatch.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.6/tegracli/group.py` & `tegracli-0.2.7/tegracli/group.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.6/tegracli/main.py` & `tegracli-0.2.7/tegracli/main.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.6/tegracli/utilities.py` & `tegracli-0.2.7/tegracli/utilities.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.6/PKG-INFO` & `tegracli-0.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tegracli
-Version: 0.2.6
+Version: 0.2.7
 Summary: A research-focused Telegram CLI application
 Home-page: https://pypi.org/project/tegracli/
 License: MIT
 Author: Philipp Kessling
 Author-email: p.kessling@leibniz-hbi.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -12,20 +12,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: Telethon (>=1.24.0,<2.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: ujson (>=5.4.0,<6.0.0)
+Requires-Dist: PyYAML
+Requires-Dist: Telethon
+Requires-Dist: click
+Requires-Dist: loguru
+Requires-Dist: pandas
+Requires-Dist: ujson
 Project-URL: Repository, https://github.com/Leibniz-HBI/tegracli
 Description-Content-Type: text/markdown
 
 # tegracli
 
 ![The TEGRACLI logo](https://github.com/Leibniz-HBI/tegracli/blob/trunk/tegracli.png?raw=true)
```

