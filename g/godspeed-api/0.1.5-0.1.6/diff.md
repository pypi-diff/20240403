# Comparing `tmp/godspeed_api-0.1.5.tar.gz` & `tmp/godspeed_api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godspeed_api-0.1.5.tar", last modified: Wed Apr  3 15:25:40 2024, max compression
+gzip compressed data, was "godspeed_api-0.1.6.tar", last modified: Wed Apr  3 15:31:06 2024, max compression
```

## Comparing `godspeed_api-0.1.5.tar` & `godspeed_api-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:40.319197 godspeed_api-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 15:25:30.000000 godspeed_api-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 15:25:40.319197 godspeed_api-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 15:25:30.000000 godspeed_api-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:40.315197 godspeed_api-0.1.5/godspeed_api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 15:25:30.000000 godspeed_api-0.1.5/godspeed_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 15:25:30.000000 godspeed_api-0.1.5/godspeed_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:40.319197 godspeed_api-0.1.5/godspeed_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 15:25:40.000000 godspeed_api-0.1.5/godspeed_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 15:25:40.000000 godspeed_api-0.1.5/godspeed_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:25:40.000000 godspeed_api-0.1.5/godspeed_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 15:25:40.000000 godspeed_api-0.1.5/godspeed_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 15:25:40.000000 godspeed_api-0.1.5/godspeed_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:25:40.319197 godspeed_api-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 15:25:30.000000 godspeed_api-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/godspeed_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/godspeed_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/godspeed_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/godspeed_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/setup.py
```

### Comparing `godspeed_api-0.1.5/LICENSE` & `godspeed_api-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.1.5/godspeed_api/api.py` & `godspeed_api-0.1.6/godspeed_api/api.py`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.1.5/setup.py` & `godspeed_api-0.1.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 DESCRIPTION = "A Godspeed task manager API wrapper"
 
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
     name="godspeed_api",
     version=VERSION,
     author="Artem Trubacheev",
     author_email="almaz5200@gmail.com",
     description=DESCRIPTION,
-    long_description=DESCRIPTION,
+    long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     keywords=["python", "godspeed"],
     classifiers=[
```

