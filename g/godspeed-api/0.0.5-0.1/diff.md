# Comparing `tmp/godspeed_api-0.0.5.tar.gz` & `tmp/godspeed_api-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godspeed_api-0.0.5.tar", last modified: Mon Apr  1 14:23:13 2024, max compression
+gzip compressed data, was "godspeed_api-0.1.tar", last modified: Wed Apr  3 14:41:14 2024, max compression
```

## Comparing `godspeed_api-0.0.5.tar` & `godspeed_api-0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:23:13.550415 godspeed_api-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-01 14:23:07.000000 godspeed_api-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 14:23:13.550415 godspeed_api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 14:23:07.000000 godspeed_api-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:23:13.546415 godspeed_api-0.0.5/godspeed_api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 14:23:07.000000 godspeed_api-0.0.5/godspeed_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 14:23:07.000000 godspeed_api-0.0.5/godspeed_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:23:13.550415 godspeed_api-0.0.5/godspeed_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 14:23:13.000000 godspeed_api-0.0.5/godspeed_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 14:23:13.000000 godspeed_api-0.0.5/godspeed_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:23:13.000000 godspeed_api-0.0.5/godspeed_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 14:23:13.000000 godspeed_api-0.0.5/godspeed_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:23:13.550415 godspeed_api-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-01 14:23:07.000000 godspeed_api-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:41:14.634851 godspeed_api-0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 14:41:08.000000 godspeed_api-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-03 14:41:14.634851 godspeed_api-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 14:41:08.000000 godspeed_api-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:41:14.634851 godspeed_api-0.1/godspeed_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 14:41:08.000000 godspeed_api-0.1/godspeed_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-03 14:41:08.000000 godspeed_api-0.1/godspeed_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:41:14.634851 godspeed_api-0.1/godspeed_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-03 14:41:14.000000 godspeed_api-0.1/godspeed_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 14:41:14.000000 godspeed_api-0.1/godspeed_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:41:14.000000 godspeed_api-0.1/godspeed_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 14:41:14.000000 godspeed_api-0.1/godspeed_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 14:41:14.000000 godspeed_api-0.1/godspeed_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:41:14.634851 godspeed_api-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 14:41:08.000000 godspeed_api-0.1/setup.py
```

### Comparing `godspeed_api-0.0.5/LICENSE` & `godspeed_api-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.0.5/setup.py` & `godspeed_api-0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.5"
+VERSION = "0.1"
 DESCRIPTION = "A Godspeed task manager API wrapper"
 
 setup(
     name="godspeed_api",
     version=VERSION,
     author="Artem Trubacheev",
     author_email="almaz5200@gmail.com",
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=[],
+    install_requires=[
+        "requests",
+    ],
     keywords=["python", "godspeed"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
```

