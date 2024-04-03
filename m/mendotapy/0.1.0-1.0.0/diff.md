# Comparing `tmp/mendotapy-0.1.0.tar.gz` & `tmp/mendotapy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mendotapy-0.1.0.tar", last modified: Thu Jun 30 01:56:45 2022, max compression
+gzip compressed data, was "mendotapy-1.0.0.tar", last modified: Wed Apr  3 03:12:16 2024, max compression
```

## Comparing `mendotapy-0.1.0.tar` & `mendotapy-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,33 @@
-drwxr-xr-x   0 gloege     (501) staff       (20)        0 2022-06-30 01:56:45.394075 mendotapy-0.1.0/
--rw-r--r--   0 gloege     (501) staff       (20)     1068 2022-03-20 22:48:56.000000 mendotapy-0.1.0/LICENSE
--rw-r--r--   0 gloege     (501) staff       (20)     1420 2022-06-30 01:56:45.394149 mendotapy-0.1.0/PKG-INFO
--rw-r--r--   0 gloege     (501) staff       (20)      502 2022-03-21 14:30:48.000000 mendotapy-0.1.0/README.md
--rw-r--r--   0 gloege     (501) staff       (20)      500 2022-03-20 23:08:27.000000 mendotapy-0.1.0/pyproject.toml
--rw-r--r--   0 gloege     (501) staff       (20)     1222 2022-06-30 01:56:45.394487 mendotapy-0.1.0/setup.cfg
--rw-r--r--   0 gloege     (501) staff       (20)       69 2022-03-20 22:48:56.000000 mendotapy-0.1.0/setup.py
-drwxr-xr-x   0 gloege     (501) staff       (20)        0 2022-06-30 01:56:45.391595 mendotapy-0.1.0/src/
-drwxr-xr-x   0 gloege     (501) staff       (20)        0 2022-06-30 01:56:45.393186 mendotapy-0.1.0/src/mendotapy/
--rw-r--r--   0 gloege     (501) staff       (20)      112 2022-03-20 23:29:19.000000 mendotapy-0.1.0/src/mendotapy/__init__.py
--rw-r--r--   0 gloege     (501) staff       (20)    15445 2022-03-21 22:14:59.000000 mendotapy-0.1.0/src/mendotapy/mendotapy.py
--rw-r--r--   0 gloege     (501) staff       (20)        0 2022-03-20 22:48:56.000000 mendotapy-0.1.0/src/mendotapy/py.typed
-drwxr-xr-x   0 gloege     (501) staff       (20)        0 2022-06-30 01:56:45.393960 mendotapy-0.1.0/src/mendotapy.egg-info/
--rw-r--r--   0 gloege     (501) staff       (20)     1420 2022-06-30 01:56:45.000000 mendotapy-0.1.0/src/mendotapy.egg-info/PKG-INFO
--rw-r--r--   0 gloege     (501) staff       (20)      347 2022-06-30 01:56:45.000000 mendotapy-0.1.0/src/mendotapy.egg-info/SOURCES.txt
--rw-r--r--   0 gloege     (501) staff       (20)        1 2022-06-30 01:56:45.000000 mendotapy-0.1.0/src/mendotapy.egg-info/dependency_links.txt
--rw-r--r--   0 gloege     (501) staff       (20)        1 2022-03-20 23:11:36.000000 mendotapy-0.1.0/src/mendotapy.egg-info/not-zip-safe
--rw-r--r--   0 gloege     (501) staff       (20)      179 2022-06-30 01:56:45.000000 mendotapy-0.1.0/src/mendotapy.egg-info/requires.txt
--rw-r--r--   0 gloege     (501) staff       (20)       10 2022-06-30 01:56:45.000000 mendotapy-0.1.0/src/mendotapy.egg-info/top_level.txt
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-03 03:12:16.318906 mendotapy-1.0.0/
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-03 03:12:16.314665 mendotapy-1.0.0/.github/
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-03 03:12:16.316390 mendotapy-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 luke       (501) staff       (20)      834 2024-04-03 02:19:48.000000 mendotapy-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 luke       (501) staff       (20)      596 2024-04-03 02:19:48.000000 mendotapy-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-03 03:12:16.316824 mendotapy-1.0.0/.github/workflows/
+-rw-r--r--   0 luke       (501) staff       (20)      819 2024-04-03 02:19:48.000000 mendotapy-1.0.0/.github/workflows/coverage.yaml
+-rw-r--r--   0 luke       (501) staff       (20)      714 2024-04-03 02:19:48.000000 mendotapy-1.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0 luke       (501) staff       (20)     1798 2024-04-03 02:19:48.000000 mendotapy-1.0.0/.gitignore
+-rw-r--r--   0 luke       (501) staff       (20)     1068 2024-04-03 02:19:48.000000 mendotapy-1.0.0/LICENSE
+-rw-r--r--   0 luke       (501) staff       (20)     1791 2024-04-03 03:12:16.318841 mendotapy-1.0.0/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)      517 2024-04-03 02:57:38.000000 mendotapy-1.0.0/README.md
+-rw-r--r--   0 luke       (501) staff       (20)      500 2024-04-03 02:19:48.000000 mendotapy-1.0.0/pyproject.toml
+-rw-r--r--   0 luke       (501) staff       (20)       64 2024-04-03 02:46:23.000000 mendotapy-1.0.0/requirements.txt
+-rw-r--r--   0 luke       (501) staff       (20)      135 2024-04-03 02:46:41.000000 mendotapy-1.0.0/requirements_dev.txt
+-rw-r--r--   0 luke       (501) staff       (20)     1173 2024-04-03 03:12:16.319240 mendotapy-1.0.0/setup.cfg
+-rw-r--r--   0 luke       (501) staff       (20)       69 2024-04-03 02:19:48.000000 mendotapy-1.0.0/setup.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-03 03:12:16.314863 mendotapy-1.0.0/src/
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-03 03:12:16.317249 mendotapy-1.0.0/src/mendotapy/
+-rw-r--r--   0 luke       (501) staff       (20)       98 2024-04-03 02:44:05.000000 mendotapy-1.0.0/src/mendotapy/__init__.py
+-rw-r--r--   0 luke       (501) staff       (20)     8109 2024-04-03 02:41:23.000000 mendotapy-1.0.0/src/mendotapy/mendotapy.py
+-rw-r--r--   0 luke       (501) staff       (20)        0 2024-04-03 02:19:48.000000 mendotapy-1.0.0/src/mendotapy/py.typed
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-03 03:12:16.317905 mendotapy-1.0.0/src/mendotapy.egg-info/
+-rw-r--r--   0 luke       (501) staff       (20)     1791 2024-04-03 03:12:16.000000 mendotapy-1.0.0/src/mendotapy.egg-info/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)      586 2024-04-03 03:12:16.000000 mendotapy-1.0.0/src/mendotapy.egg-info/SOURCES.txt
+-rw-r--r--   0 luke       (501) staff       (20)        1 2024-04-03 03:12:16.000000 mendotapy-1.0.0/src/mendotapy.egg-info/dependency_links.txt
+-rw-r--r--   0 luke       (501) staff       (20)        1 2024-04-03 02:43:01.000000 mendotapy-1.0.0/src/mendotapy.egg-info/not-zip-safe
+-rw-r--r--   0 luke       (501) staff       (20)      132 2024-04-03 03:12:16.000000 mendotapy-1.0.0/src/mendotapy.egg-info/requires.txt
+-rw-r--r--   0 luke       (501) staff       (20)       10 2024-04-03 03:12:16.000000 mendotapy-1.0.0/src/mendotapy.egg-info/top_level.txt
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-03 03:12:16.318132 mendotapy-1.0.0/tests/
+-rw-r--r--   0 luke       (501) staff       (20)        0 2024-04-03 02:19:48.000000 mendotapy-1.0.0/tests/__init__.py
+-rw-r--r--   0 luke       (501) staff       (20)       76 2024-04-03 02:32:08.000000 mendotapy-1.0.0/tests/test_mendotapy.py
+-rw-r--r--   0 luke       (501) staff       (20)      598 2024-04-03 02:19:48.000000 mendotapy-1.0.0/tox.ini
```

### Comparing `mendotapy-0.1.0/LICENSE` & `mendotapy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mendotapy-0.1.0/setup.cfg` & `mendotapy-1.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = mendotapy
 description = load Lake Mendota ice phenology
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.1.0
+version = 1.0.0
 author = Luke Gloege
-author_email = ljg2157@columbia.edu
+author_email = lucas.gloege@yale.edu
 url = https://github.com/lgloege/mendotapy
 keywords = mendota
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Development Status :: 3 - Alpha
@@ -24,20 +24,17 @@
 	Programming Language :: Python :: 3.9
 
 [options]
 packages = 
 	mendotapy
 install_requires = 
 	pandas>=1.3
-	numpy>=1.21
 	requests>=2.26
 	types-requests>=2.27
 	bs4==0.0.1
-	scikit-learn>=0.23
-	matplotlib>=3.3
 python_requires = >=3.6
 package_dir = 
 	=src
 zip_safe = no
 
 [options.extras_require]
 testing =
```

