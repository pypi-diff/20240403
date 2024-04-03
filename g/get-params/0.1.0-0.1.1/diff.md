# Comparing `tmp/get-params-0.1.0.tar.gz` & `tmp/get-params-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-params-0.1.0.tar", last modified: Wed Apr  3 21:23:35 2024, max compression
+gzip compressed data, was "get-params-0.1.1.tar", last modified: Wed Apr  3 21:30:44 2024, max compression
```

## Comparing `get-params-0.1.0.tar` & `get-params-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tollef    (1000) tollef    (1000)        0 2024-04-03 21:23:35.818786 get-params-0.1.0/
--rw-rw-r--   0 tollef    (1000) tollef    (1000)     1063 2024-04-03 21:15:08.000000 get-params-0.1.0/LICENSE
--rw-r--r--   0 tollef    (1000) tollef    (1000)      207 2024-04-03 21:23:35.818786 get-params-0.1.0/PKG-INFO
--rw-rw-r--   0 tollef    (1000) tollef    (1000)      889 2024-04-03 21:23:23.000000 get-params-0.1.0/README.md
-drwxrwxr-x   0 tollef    (1000) tollef    (1000)        0 2024-04-03 21:23:35.818786 get-params-0.1.0/get_params/
--rw-rw-r--   0 tollef    (1000) tollef    (1000)       41 2024-04-03 21:14:00.000000 get-params-0.1.0/get_params/__init__.py
--rw-rw-r--   0 tollef    (1000) tollef    (1000)      837 2024-04-03 21:21:27.000000 get-params-0.1.0/get_params/utils.py
-drwxrwxr-x   0 tollef    (1000) tollef    (1000)        0 2024-04-03 21:23:35.818786 get-params-0.1.0/get_params.egg-info/
--rw-r--r--   0 tollef    (1000) tollef    (1000)      207 2024-04-03 21:23:35.000000 get-params-0.1.0/get_params.egg-info/PKG-INFO
--rw-rw-r--   0 tollef    (1000) tollef    (1000)      205 2024-04-03 21:23:35.000000 get-params-0.1.0/get_params.egg-info/SOURCES.txt
--rw-rw-r--   0 tollef    (1000) tollef    (1000)        1 2024-04-03 21:23:35.000000 get-params-0.1.0/get_params.egg-info/dependency_links.txt
--rw-rw-r--   0 tollef    (1000) tollef    (1000)       11 2024-04-03 21:23:35.000000 get-params-0.1.0/get_params.egg-info/top_level.txt
--rw-rw-r--   0 tollef    (1000) tollef    (1000)       38 2024-04-03 21:23:35.818786 get-params-0.1.0/setup.cfg
--rw-rw-r--   0 tollef    (1000) tollef    (1000)      305 2024-04-03 21:23:25.000000 get-params-0.1.0/setup.py
+drwxrwxr-x   0 tollef    (1000) tollef    (1000)        0 2024-04-03 21:30:44.338780 get-params-0.1.1/
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)     1063 2024-04-03 21:15:08.000000 get-params-0.1.1/LICENSE
+-rw-r--r--   0 tollef    (1000) tollef    (1000)     1307 2024-04-03 21:30:44.338780 get-params-0.1.1/PKG-INFO
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)      889 2024-04-03 21:23:23.000000 get-params-0.1.1/README.md
+drwxrwxr-x   0 tollef    (1000) tollef    (1000)        0 2024-04-03 21:30:44.338780 get-params-0.1.1/get_params/
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)       41 2024-04-03 21:14:00.000000 get-params-0.1.1/get_params/__init__.py
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)      837 2024-04-03 21:21:27.000000 get-params-0.1.1/get_params/utils.py
+drwxrwxr-x   0 tollef    (1000) tollef    (1000)        0 2024-04-03 21:30:44.338780 get-params-0.1.1/get_params.egg-info/
+-rw-r--r--   0 tollef    (1000) tollef    (1000)     1307 2024-04-03 21:30:44.000000 get-params-0.1.1/get_params.egg-info/PKG-INFO
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)      205 2024-04-03 21:30:44.000000 get-params-0.1.1/get_params.egg-info/SOURCES.txt
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)        1 2024-04-03 21:30:44.000000 get-params-0.1.1/get_params.egg-info/dependency_links.txt
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)       11 2024-04-03 21:30:44.000000 get-params-0.1.1/get_params.egg-info/top_level.txt
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)       38 2024-04-03 21:30:44.338780 get-params-0.1.1/setup.cfg
+-rw-rw-r--   0 tollef    (1000) tollef    (1000)      661 2024-04-03 21:30:42.000000 get-params-0.1.1/setup.py
```

### Comparing `get-params-0.1.0/LICENSE` & `get-params-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `get-params-0.1.0/README.md` & `get-params-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `get-params-0.1.0/get_params/utils.py` & `get-params-0.1.1/get_params/utils.py`

 * *Files identical despite different names*

