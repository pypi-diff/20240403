# Comparing `tmp/PyFaceCrop-0.0.1.tar.gz` & `tmp/PyFaceCrop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFaceCrop-0.0.1.tar", last modified: Wed Apr  3 09:31:28 2024, max compression
+gzip compressed data, was "PyFaceCrop-0.0.2.tar", last modified: Wed Apr  3 10:21:03 2024, max compression
```

## Comparing `PyFaceCrop-0.0.1.tar` & `PyFaceCrop-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 09:31:28.467870 PyFaceCrop-0.0.1/
--rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.1/LICENSE
--rw-r--r--   0 cdp        (501) staff       (20)       76 2024-04-03 09:31:28.467560 PyFaceCrop-0.0.1/PKG-INFO
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 09:31:28.465894 PyFaceCrop-0.0.1/PyFaceCrop/
--rw-r--r--   0 cdp        (501) staff       (20)     4414 2024-04-03 06:52:33.000000 PyFaceCrop-0.0.1/PyFaceCrop/FaceCrop.py
--rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.1/PyFaceCrop/__init__.py
--rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.1/PyFaceCrop/main.py
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 09:31:28.466952 PyFaceCrop-0.0.1/PyFaceCrop.egg-info/
--rw-r--r--   0 cdp        (501) staff       (20)       76 2024-04-03 09:31:28.000000 PyFaceCrop-0.0.1/PyFaceCrop.egg-info/PKG-INFO
--rw-r--r--   0 cdp        (501) staff       (20)      227 2024-04-03 09:31:28.000000 PyFaceCrop-0.0.1/PyFaceCrop.egg-info/SOURCES.txt
--rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-03 09:31:28.000000 PyFaceCrop-0.0.1/PyFaceCrop.egg-info/dependency_links.txt
--rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-03 09:31:28.000000 PyFaceCrop-0.0.1/PyFaceCrop.egg-info/top_level.txt
--rw-r--r--   0 cdp        (501) staff       (20)       33 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.1/README.md
--rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-03 09:31:28.467940 PyFaceCrop-0.0.1/setup.cfg
--rw-r--r--   0 cdp        (501) staff       (20)      152 2024-04-03 09:30:49.000000 PyFaceCrop-0.0.1/setup.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 10:21:03.155194 PyFaceCrop-0.0.2/
+-rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.2/LICENSE
+-rw-r--r--   0 cdp        (501) staff       (20)      179 2024-04-03 10:21:03.154905 PyFaceCrop-0.0.2/PKG-INFO
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 10:21:03.153497 PyFaceCrop-0.0.2/PyFaceCrop/
+-rw-r--r--   0 cdp        (501) staff       (20)     4414 2024-04-03 06:52:33.000000 PyFaceCrop-0.0.2/PyFaceCrop/FaceCrop.py
+-rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.2/PyFaceCrop/__init__.py
+-rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.2/PyFaceCrop/main.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 10:21:03.154498 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/
+-rw-r--r--   0 cdp        (501) staff       (20)      179 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/PKG-INFO
+-rw-r--r--   0 cdp        (501) staff       (20)      260 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/SOURCES.txt
+-rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/dependency_links.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/requires.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/top_level.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       33 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.2/README.md
+-rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-03 10:21:03.155257 PyFaceCrop-0.0.2/setup.cfg
+-rw-r--r--   0 cdp        (501) staff       (20)      320 2024-04-03 10:19:54.000000 PyFaceCrop-0.0.2/setup.py
```

### Comparing `PyFaceCrop-0.0.1/LICENSE` & `PyFaceCrop-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFaceCrop-0.0.1/PyFaceCrop/FaceCrop.py` & `PyFaceCrop-0.0.2/PyFaceCrop/FaceCrop.py`

 * *Files identical despite different names*

