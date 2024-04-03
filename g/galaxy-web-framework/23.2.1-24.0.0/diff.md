# Comparing `tmp/galaxy-web-framework-23.2.1.tar.gz` & `tmp/galaxy-web-framework-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_framework/dist/.tmp-t_oy18t7/galaxy-web-framework-23.2.1.tar", last modified: Thu Feb 22 03:56:06 2024, max compression
+gzip compressed data, was "galaxy-web-framework-24.0.0.tar", last modified: Wed Apr  3 02:46:17 2024, max compression
```

## Comparing `galaxy-web-framework-23.2.1.tar` & `galaxy-web-framework-24.0.0.tar`

### file list

```diff
@@ -1,57 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/form_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21882 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19590 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43001 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/helpers/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/helpers/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17368 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/remoteuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/sqldebug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/translogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/xforwardedhost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/legacy_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/legacy_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38893 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/legacy_framework/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)    13254 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/js/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/js/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/js/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/js/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/js/lib/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/js/lib/mapper.js
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/js/lib/proxy.js
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/proxy/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy/web/short_term_storage/
--rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/short_term_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/galaxy/web/statsd_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy_web_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy_web_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy_web_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy_web_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy_web_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/galaxy_web_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-22 03:56:06.000000 galaxy-web-framework-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-web-framework-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.479979 galaxy-web-framework-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-03 02:46:17.479979 galaxy-web-framework-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.471979 galaxy-web-framework-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.471979 galaxy-web-framework-24.0.0/galaxy/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/form_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21864 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/remoteuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/sqldebug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/translogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/xforwardedhost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/legacy_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/legacy_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38863 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/legacy_framework/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13254 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/mapper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/statsd_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.479979 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-03 02:46:17.479979 galaxy-web-framework-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-web-framework-23.2.1/LICENSE` & `galaxy-web-framework-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/PKG-INFO` & `galaxy-web-framework-24.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-util
+Requires-Dist: babel
+Requires-Dist: MarkupSafe
+Requires-Dist: paste
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: requests
+Requires-Dist: Routes
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: WebOb
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-framework.svg
    :target: https://pypi.org/project/galaxy-web-framework/
 
 
 Overview
@@ -42,14 +52,31 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Removes outdated Grid controller and backbone modules by `@guerler <https://github.com/guerler>`_ in `#17434 <https://github.com/galaxyproject/galaxy/pull/17434>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/__init__.py` & `galaxy-web-framework-24.0.0/galaxy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/__init__.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Galaxy web application framework
 """
+
 from . import base
 
 DEPRECATED_URL_ATTRIBUTE_MESSAGE = "*deprecated attribute, URL not filled in by server*"
 
 
 def handle_url_for(*args, **kwargs) -> str:
     """Tries to resolve the URL using the `routes` module.
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/base.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A simple WSGI application/framework.
 """
+
 import io
 import json
 import logging
 import os
 import socket
 import tarfile
 import tempfile
@@ -246,17 +247,17 @@
                 controller_name, controller, action, method = self._resolve_map_match(
                     client_match, path_info, controllers
                 )
             else:
                 raise
         trans.controller = controller_name
         trans.action = action
-        environ[
-            "controller_action_key"
-        ] = f"{'api' if environ['is_api_request'] else 'web'}.{controller_name}.{action or 'default'}"
+        environ["controller_action_key"] = (
+            f"{'api' if environ['is_api_request'] else 'web'}.{controller_name}.{action or 'default'}"
+        )
         # Combine mapper args and query string / form args and call
         kwargs = trans.request.params.mixed()
         kwargs.update(map_match)
         # Special key for AJAX debugging, remove to avoid confusing methods
         kwargs.pop("_", None)
         try:
             body = method(trans, **kwargs)
@@ -422,16 +423,15 @@
             return socket.gethostbyaddr(self.remote_addr)[0]
         except OSError:
             return self.remote_addr
 
     @lazy_property
     def cookies(self):
         cookies = SimpleCookie()
-        cookie_header = self.environ.get("HTTP_COOKIE")
-        if cookie_header:
+        if cookie_header := self.environ.get("HTTP_COOKIE"):
             all_cookies = webob.cookies.parse_cookie(cookie_header)
             galaxy_cookies = {k.decode(): v.decode() for k, v in all_cookies if k.startswith(b"galaxy")}
             if galaxy_cookies:
                 try:
                     cookies.load(galaxy_cookies)
                 except CookieError:
                     pass
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/decorators.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import logging
 from functools import wraps
 from inspect import getfullargspec
 from json import loads
 from traceback import format_exc
+from typing import (
+    TYPE_CHECKING,
+    Union,
+)
 
 import paste.httpexceptions
-from pydantic import BaseModel
-from pydantic.error_wrappers import ValidationError
+from pydantic import (
+    BaseModel,
+    ValidationError,
+)
 
 from galaxy.exceptions import (
     error_codes,
     MessageException,
     RequestParameterInvalidException,
     RequestParameterMissingException,
 )
+from galaxy.exceptions.utils import api_error_to_dict
 from galaxy.util import (
     parse_non_hex_float,
     unicodify,
 )
 from galaxy.util.json import safe_dumps
 from galaxy.web.framework import url_for
 
+if TYPE_CHECKING:
+    from fastapi.exceptions import RequestValidationError
+
 log = logging.getLogger(__name__)
 
 JSON_CONTENT_TYPE = "application/json; charset=UTF-8"
 JSONP_CONTENT_TYPE = "application/javascript"
 JSONP_CALLBACK_KEY = "callback"
 
 
@@ -232,16 +242,15 @@
     elif content_type == "application/offset+octet-stream":
         return unicodify(trans.request.body)
     else:
         # Assume application/json content type and parse request body manually, since wsgi won't do it. However, the order of this check
         # should ideally be in reverse, with the if clause being a check for application/json and the else clause assuming a standard encoding
         # such as multipart/form-data. Leaving it as is for backward compatibility, just in case.
         payload = loads(unicodify(trans.request.body))
-    run_as = trans.request.headers.get("run-as")
-    if run_as:
+    if run_as := trans.request.headers.get("run-as"):
         payload["run_as"] = run_as
     return payload
 
 
 def legacy_expose_api_raw(func):
     """
     Expose this function via the API but don't dump the results
@@ -369,69 +378,47 @@
     """
     Formats a return value as JSON or JSONP if `jsonp_callback` is present.
 
     Use `pretty=True` to return pretty printed json.
     """
     dumps_kwargs = dict(indent=4, sort_keys=True) if pretty else {}
     if isinstance(rval, BaseModel):
-        json = rval.json(**dumps_kwargs)
+        json = rval.model_dump_json(indent=4)
     else:
         json = safe_dumps(rval, **dumps_kwargs)
     if jsonp_callback:
         json = f"{jsonp_callback}({json});"
     return json
 
 
-def validation_error_to_message_exception(e: ValidationError) -> MessageException:
+def validation_error_to_message_exception(e: Union[ValidationError, "RequestValidationError"]) -> MessageException:
     invalid_found = False
     missing_found = False
+    messages = []
+    clean_validation_errors = []
     for error in e.errors():
-        if error["type"] == "value_error.missing" or error["type"] == "type_error.none.not_allowed":
+        messages.append(f"{error['msg']} in {error['loc']}")
+        if error["type"] == "missing" or error["type"] == "type_error.none.not_allowed":
             missing_found = True
         elif error["type"].startswith("type_error"):
             invalid_found = True
+        # ctx contains data that can't be serialized, like exception instances
+        error.pop("ctx", None)
+        try:
+            clean_validation_errors.append(safe_dumps(error))
+        except TypeError:
+            pass
     if missing_found and not invalid_found:
-        return RequestParameterMissingException(str(e), validation_errors=loads(e.json()))
-    else:
-        return RequestParameterInvalidException(str(e), validation_errors=loads(e.json()))
-
-
-def api_error_message(trans, **kwds):
-    exception = kwds.get("exception", None)
-    if exception:
-        # If we are passed a MessageException use err_msg.
-        default_error_code = getattr(exception, "err_code", error_codes.UNKNOWN)
-        default_error_message = getattr(exception, "err_msg", default_error_code.default_error_message)
-        extra_error_info = getattr(exception, "extra_error_info", {})
-        if not isinstance(extra_error_info, dict):
-            extra_error_info = {}
+        return RequestParameterMissingException("\n".join(messages), validation_errors=clean_validation_errors)
     else:
-        default_error_message = "Error processing API request."
-        default_error_code = error_codes.UNKNOWN
-        extra_error_info = {}
-    traceback_string = kwds.get("traceback", "No traceback available.")
-    err_msg = kwds.get("err_msg", default_error_message)
-    error_code_object = kwds.get("err_code", default_error_code)
-    try:
-        error_code = error_code_object.code
-    except AttributeError:
-        # Some sort of bad error code sent in, logic failure on part of
-        # Galaxy developer.
-        error_code = error_codes.UNKNOWN.code
-    # Would prefer the terminology of error_code and error_message, but
-    # err_msg used a good number of places already. Might as well not change
-    # it?
-    error_response = dict(err_msg=err_msg, err_code=error_code, **extra_error_info)
-    if trans and trans.debug:  # TODO: Should admins get to see traceback as well?
-        error_response["traceback"] = traceback_string
-    return error_response
+        return RequestParameterInvalidException("\n".join(messages), validation_errors=clean_validation_errors)
 
 
 def __api_error_dict(trans, **kwds):
-    error_dict = api_error_message(trans, **kwds)
+    error_dict = api_error_to_dict(debug=trans.debug, **kwds)
     exception = kwds.get("exception", None)
     # If we are given an status code directly - use it - otherwise check
     # the exception for a status_code attribute.
     if "status_code" in kwds:
         status_code = int(kwds.get("status_code"))
     elif hasattr(exception, "status_code"):
         status_code = int(exception.status_code)
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/helpers/__init__.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Galaxy web framework helpers
 
 The functions in this module should be considered part of the API used by
 visualizations in their mako files through the `$h` object, see
 GalaxyWebTransaction in galaxy/webapps/base/webapp.py
 """
+
 from datetime import (
     datetime,
     timedelta,
 )
 
 from babel import default_locale
 from babel.dates import format_timedelta
 from routes import url_for
 
-from galaxy.util import unicodify
 from galaxy.util.json import safe_dumps as dumps  # noqa: F401
 from .tags import (
     javascript_link,
     stylesheet_link,
 )
 from ..base import server_starttime
 
@@ -94,23 +94,14 @@
     """
     Take a prefix and list of javascript names and return appropriate
     string of script tags.
     """
     return js_helper("static/dist/", *args)
 
 
-# Unicode help
-def to_unicode(a_string):
-    """
-    Convert a string to unicode in utf-8 format; if string is already unicode,
-    does nothing because string's encoding cannot be determined by introspection.
-    """
-    return unicodify(a_string, "utf-8")
-
-
 def is_true(val):
     """
     Returns true if input is a boolean and true or is a string and looks like a true value.
     """
     return val is True or val in ["True", "true", "T", "t"]
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/helpers/grids.py` & `galaxy-web-framework-24.0.0/galaxy/web/legacy_framework/grids.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 
 from galaxy.model.item_attrs import (
     get_foreign_key,
     UsesAnnotations,
     UsesItemRatings,
 )
 from galaxy.util import (
-    restore_text,
     sanitize_text,
     unicodify,
 )
 from galaxy.web.framework import (
     decorators,
     url_for,
 )
+from galaxy.web.framework.helpers import iff
 
 log = logging.getLogger(__name__)
 
 
 class GridColumn:
     def __init__(
         self,
@@ -51,37 +51,35 @@
         visible=True,
         nowrap=False,
         # Valid values for filterable are ['standard', 'advanced', None]
         filterable=None,
         sortable=True,
         label_id_prefix=None,
         target=None,
-        delayed=False,
     ):
         """Create a grid column."""
         self.label = label
         self.key = key
         self.model_class = model_class
         self.method = method
         self.format = format
         self.link = link
         self.target = target
         self.nowrap = nowrap
         self.attach_popup = attach_popup
         self.visible = visible
         self.filterable = filterable
-        self.delayed = delayed
         # Column must have a key to be sortable.
         self.sortable = self.key is not None and sortable
         self.label_id_prefix = label_id_prefix or ""
 
     def get_value(self, trans, grid, item):
         if self.method:
             value = getattr(grid, self.method)(trans, item)
-        elif self.key and hasattr(item, self.key):
+        elif self.key:
             value = getattr(item, self.key)
         else:
             value = None
         if self.format:
             value = self.format(value)
         return escape(unicodify(value))
 
@@ -109,21 +107,18 @@
             accepted_filters.append(GridColumnFilter(val, args))
         return accepted_filters
 
     def sort(self, trans, query, ascending, column_name=None):
         """Sort query using this column."""
         if column_name is None:
             column_name = self.key
-        column = getattr(self.model_class, column_name)
-        if column is None:
-            column = self.model_class.table.c.get(column_name)
         if ascending:
-            query = query.order_by(column.asc())
+            query = query.order_by(self.model_class.table.c.get(column_name).asc())
         else:
-            query = query.order_by(column.desc())
+            query = query.order_by(self.model_class.table.c.get(column_name).desc())
         return query
 
 
 class ReverseSortColumn(GridColumn):
     """Column that reverses sorting; this is useful when the natural sort is descending."""
 
     def sort(self, trans, query, ascending, column_name=None):
@@ -224,24 +219,15 @@
         return GridColumn.sort(self, trans, query, ascending, column_name=column_name)
 
 
 class CommunityRatingColumn(GridColumn, UsesItemRatings):
     """Column that displays community ratings for an item."""
 
     def get_value(self, trans, grid, item):
-        if not hasattr(item, "average_rating"):
-            # No prefetched column property, generate it on the fly.
-            ave_item_rating, num_ratings = self.get_ave_item_rating_data(
-                trans.sa_session, item, webapp_model=trans.model
-            )
-        else:
-            ave_item_rating = item.average_rating
-            num_ratings = 2  # just used for pluralization
-        if not ave_item_rating:
-            ave_item_rating = 0
+        ave_item_rating, num_ratings = self.get_ave_item_rating_data(trans.sa_session, item, webapp_model=trans.model)
         return trans.fill_template(
             "tool_shed_rating.mako",
             ave_item_rating=ave_item_rating,
             num_ratings=num_ratings,
             item_id=trans.security.encode_id(item.id),
         )
 
@@ -336,15 +322,15 @@
         return query
 
     def get_filter(self, trans, user, column_filter):
         # Parse filter to extract multiple tags.
         if isinstance(column_filter, list):
             # Collapse list of tags into a single string; this is redundant but effective. TODO: fix this by iterating over tags.
             column_filter = ",".join(column_filter)
-        raw_tags = trans.app.tag_handler.parse_tags(column_filter)
+        raw_tags = trans.app.tag_handler.parse_tags(column_filter.encode("utf-8"))
         clause_list = []
         for name, value in raw_tags:
             if name:
                 # Filter by all tags.
                 clause_list.append(
                     self.model_class.tags.any(
                         func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%")
@@ -375,15 +361,15 @@
         )
 
     def get_filter(self, trans, user, column_filter):
         # Parse filter to extract multiple tags.
         if isinstance(column_filter, list):
             # Collapse list of tags into a single string; this is redundant but effective. TODO: fix this by iterating over tags.
             column_filter = ",".join(column_filter)
-        raw_tags = trans.app.tag_handler.parse_tags(column_filter)
+        raw_tags = trans.app.tag_handler.parse_tags(column_filter.encode("utf-8"))
         clause_list = []
         for name, value in raw_tags:
             if name:
                 # Filter by individual's tag names.
                 clause_list.append(
                     self.model_class.tags.any(
                         and_(
@@ -478,91 +464,61 @@
         if column_filter == "All":
             pass
         elif column_filter in ["True", "False"]:
             query = query.filter(self.model_class.deleted == (column_filter == "True"))
         return query
 
 
-class PurgedColumn(GridColumn):
-    """Column that tracks and filters for items with purged attribute."""
-
-    def get_accepted_filters(self):
-        """Returns a list of accepted filters for this column."""
-        accepted_filter_labels_and_vals = {"nonpurged": "False", "purged": "True", "all": "All"}
-        accepted_filters = []
-        for label, val in accepted_filter_labels_and_vals.items():
-            args = {self.key: val}
-            accepted_filters.append(GridColumnFilter(label, args))
-        return accepted_filters
-
-    def filter(self, trans, user, query, column_filter):
-        """Modify query to filter self.model_class by state."""
-        if column_filter == "All":
-            pass
-        elif column_filter in ["True", "False"]:
-            query = query.filter(self.model_class.purged == (column_filter == "True"))
-        return query
-
-
 class StateColumn(GridColumn):
     """
     Column that tracks and filters for items with state attribute.
-
-    IMPORTANT NOTE: self.model_class must have a states Bunch or dict if
-    this column type is used in the grid.
     """
 
     def get_value(self, trans, grid, item):
         return item.state
 
     def filter(self, trans, user, query, column_filter):
         """Modify query to filter self.model_class by state."""
         if column_filter == "All":
             pass
-        elif column_filter in [v for k, v in self.model_class.states.items()]:
+        elif column_filter in list(self.model_class.states):
             query = query.filter(self.model_class.state == column_filter)
         return query
 
     def get_accepted_filters(self):
         """Returns a list of accepted filters for this column."""
         all = GridColumnFilter("all", {self.key: "All"})
         accepted_filters = [all]
-        for v in self.model_class.states.values():
-            args = {self.key: v}
-            accepted_filters.append(GridColumnFilter(v, args))
+        for state in self.model_class.states:
+            args = {self.key: state.value}
+            accepted_filters.append(GridColumnFilter(state.value, args))
         return accepted_filters
 
 
 class SharingStatusColumn(GridColumn):
     """Grid column to indicate sharing status."""
 
-    def __init__(self, *args, **kwargs):
-        self.use_shared_with_count = kwargs.pop("use_shared_with_count", False)
-        super().__init__(*args, **kwargs)
-
     def get_value(self, trans, grid, item):
         # Delete items cannot be shared.
         if item.deleted:
             return ""
         # Build a list of sharing for this item.
         sharing_statuses = []
-        if self._is_shared(item):
+        if item.users_shared_with:
             sharing_statuses.append("Shared")
         if item.importable:
             sharing_statuses.append("Accessible")
         if item.published:
             sharing_statuses.append("Published")
         return ", ".join(sharing_statuses)
 
-    def _is_shared(self, item):
-        if self.use_shared_with_count:
-            # optimization to skip join for users_shared_with and loading in that data.
-            return item.users_shared_with_count > 0
-
-        return item.users_shared_with
+    def get_link(self, trans, grid, item):
+        if not item.deleted and (item.users_shared_with or item.importable or item.published):
+            return dict(operation="share or publish", id=item.id)
+        return None
 
     def filter(self, trans, user, query, column_filter):
         """Modify query to filter histories by sharing status."""
         if column_filter == "All":
             pass
         elif column_filter:
             if column_filter == "private":
@@ -669,30 +625,34 @@
     """
     Specifies the content and format of a grid (data table).
     """
 
     title = ""
     model_class: Optional[type] = None
     show_item_checkboxes = False
+    template = "legacy/grid_base.mako"
+    async_template = "legacy/grid_base_async.mako"
+    use_async = False
     use_hide_message = True
     global_actions: List[GridAction] = []
     columns: List[GridColumn] = []
     operations: List[GridOperation] = []
     standard_filters: List[GridColumnFilter] = []
     # Any columns that are filterable (either standard or advanced) should have a default value set in the default filter.
     default_filter: Dict[str, str] = {}
     default_sort_key: Optional[str] = None
     use_paging = False
     num_rows_per_page = 25
     num_page_links = 10
+    allow_fetching_all_results = True
     # Set preference names.
     cur_filter_pref_name = ".filter"
     cur_sort_key_pref_name = ".sort_key"
     legend = None
-    info_text: Optional[str] = None
+    info_text = None
 
     def __init__(self):
         # Determine if any multiple row operations are defined
         self.has_multiple_item_operations = False
         for operation in self.operations:
             if operation.allow_multiple:
                 self.has_multiple_item_operations = True
@@ -718,17 +678,16 @@
         base_sort_key = self.default_sort_key
         # Build initial query
         query = self.build_initial_query(trans, **kwargs)
         query = self.apply_query_filter(trans, query, **kwargs)
         # Maintain sort state in generated urls
         extra_url_args = {}
         # Determine whether use_default_filter flag is set.
-        use_default_filter_str = kwargs.get("use_default_filter")
         use_default_filter = False
-        if use_default_filter_str:
+        if use_default_filter_str := kwargs.get("use_default_filter"):
             use_default_filter = use_default_filter_str.lower() == "true"
         # Process filtering arguments to (a) build a query that represents the filter and (b) build a
         # dictionary that denotes the current filter.
         cur_filter_dict = {}
         for column in self.columns:
             if column.key:
                 # Get the filter criterion for the column. Precedence is (a) if using default filter, only look there; otherwise,
@@ -792,18 +751,21 @@
                     # Upate current filter dict.
                     # Column filters are rendered in various places, sanitize them all here.
                     cur_filter_dict[column.key] = sanitize_text(column_filter)
                     # Carry filter along to newly generated urls; make sure filter is a string so
                     # that we can encode to UTF-8 and thus handle user input to filters.
                     if isinstance(column_filter, list):
                         # Filter is a list; process each item.
+                        column_filter = [str(_).encode("utf-8") if not isinstance(_, str) else _ for _ in column_filter]
                         extra_url_args[f"f-{column.key}"] = dumps(column_filter)
                     else:
                         # Process singleton filter.
-                        extra_url_args[f"f-{column.key}"] = column_filter
+                        if not isinstance(column_filter, str):
+                            column_filter = str(column_filter)
+                        extra_url_args[f"f-{column.key}"] = column_filter.encode("utf-8")
         # Process sort arguments.
         sort_key = None
         if "sort" in kwargs:
             sort_key = kwargs["sort"]
         elif base_sort_key:
             sort_key = base_sort_key
         if sort_key:
@@ -831,40 +793,58 @@
                 if (table_name is None or table_name == column.model_class.__name__) and column_key == column_name:
                     query = column.sort(trans, query, ascending, column_name=column_name)
                     break
             extra_url_args["sort"] = sort_key
         # There might be a current row
         current_item = self.get_current_item(trans, **kwargs)
         # Process page number.
-        num_pages = None
-        total_row_count_query = query  # query without limit applied to get total number of rows.
         if self.use_paging:
             if "page" in kwargs:
                 if kwargs["page"] == "all":
                     page_num = 0
+                    if self.allow_fetching_all_results:
+                        page_num = 0
+                    else:
+                        # Should make it harder to return all results at once
+                        page_num = 1
                 else:
                     page_num = int(kwargs["page"])
             else:
                 page_num = 1
             if page_num == 0:
-                num_pages = 1
+                # Show all rows in page.
+                total_num_rows = query.count()
                 page_num = 1
+                num_pages = 1
             else:
+                # Show a limited number of rows. Before modifying query, get the total number of rows that query
+                # returns so that the total number of pages can be computed.
+                total_num_rows = query.count()
                 query = query.limit(self.num_rows_per_page).offset((page_num - 1) * self.num_rows_per_page)
+                num_pages = int(math.ceil(float(total_num_rows) / self.num_rows_per_page))
         else:
             # Defaults.
             page_num = 1
+            num_pages = 1
         # There are some places in grid templates where it's useful for a grid
         # to have its current filter.
         self.cur_filter_dict = cur_filter_dict
 
         # Log grid view.
         context = str(self.__class__.__name__)
         params = cur_filter_dict.copy()
         params["sort"] = sort_key
+        params["async"] = "async" in kwargs
+
+        # TODO:??
+        # commenting this out; when this fn calls session.add( action ) and session.flush the query from this fn
+        # is effectively 'wiped' out. Nate believes it has something to do with our use of session( autocommit=True )
+        # in mapping.py. If you change that to False, the log_action doesn't affect the query
+        # Below, I'm rendering the template first (that uses query), then calling log_action, then returning the page
+        # trans.log_action( trans.get_user(), text_type( "grid.view" ), context, params )
 
         # Render grid.
         def url(*args, **kwargs):
             route_name = kwargs.pop("__route_name__", None)
             # Only include sort/filter arguments if not linking to another
             # page. This is a bit of a hack.
             if "action" in kwargs:
@@ -889,138 +869,49 @@
                 new_kwargs["action"] = trans.action
             if route_name:
                 return url_for(route_name, **new_kwargs)
             return url_for(**new_kwargs)
 
         self.use_panels = kwargs.get("use_panels", False) in [True, "True", "true"]
         self.advanced_search = kwargs.get("advanced_search", False) in [True, "True", "true"]
+        async_request = (self.use_async) and (kwargs.get("async", False) in [True, "True", "true"])
         # Currently, filling the template returns a str object; this requires decoding the string into a
         # unicode object within mako templates. What probably should be done is to return the template as
         # utf-8 unicode; however, this would require encoding the object as utf-8 before returning the grid
         # results via a controller method, which is require substantial changes. Hence, for now, return grid
         # as str.
-        grid_config = {
-            "title": self.title,
-            "title_id": getattr(self, "title_id", None),
-            "url_base": trans.request.path_url,
-            "async_ops": [],
-            "categorical_filters": {},
-            "filters": cur_filter_dict,
-            "sort_key": sort_key,
-            "show_item_checkboxes": self.show_item_checkboxes
-            or kwargs.get("show_item_checkboxes", "") in ["True", "true"],
-            "cur_page_num": page_num,
-            "num_page_links": self.num_page_links,
-            "status": status,
-            "message": restore_text(message),
-            "global_actions": [],
-            "operations": [],
-            "items": [],
-            "columns": [],
-            "model_class": str(self.model_class),
-            "use_paging": self.use_paging,
-            "legend": self.legend,
-            "current_item_id": False,
-            "use_hide_message": self.use_hide_message,
-            "default_filter_dict": self.default_filter,
-            "advanced_search": self.advanced_search,
-            "info_text": self.info_text,
-            "url": url(dict()),
-            "refresh_frames": kwargs.get("refresh_frames", []),
-        }
-        if current_item:
-            grid_config["current_item_id"] = current_item.id
-        for column in self.columns:
-            extra = ""
-            if column.sortable:
-                if sort_key.endswith(column.key):
-                    if not sort_key.startswith("-"):
-                        extra = "&darr;"
-                    else:
-                        extra = "&uarr;"
-            grid_config["columns"].append(
-                {
-                    "key": column.key,
-                    "visible": column.visible,
-                    "nowrap": column.nowrap,
-                    "attach_popup": column.attach_popup,
-                    "label_id_prefix": column.label_id_prefix,
-                    "sortable": column.sortable,
-                    "label": column.label,
-                    "filterable": column.filterable,
-                    "delayed": column.delayed,
-                    "is_text": isinstance(column, TextColumn),
-                    "extra": extra,
-                }
-            )
-        for operation in self.operations:
-            grid_config["operations"].append(
-                {
-                    "allow_multiple": operation.allow_multiple,
-                    "allow_popup": operation.allow_popup,
-                    "target": operation.target,
-                    "label": operation.label,
-                    "confirm": operation.confirm,
-                    "href": url(**operation.url_args) if isinstance(operation.url_args, dict) else None,
-                    "global_operation": False,
-                }
-            )
-            if operation.allow_multiple:
-                grid_config["show_item_checkboxes"] = True
-            if operation.global_operation:
-                grid_config["global_operation"] = url(**(operation.global_operation()))
-        for action in self.global_actions:
-            grid_config["global_actions"].append(
-                {"url_args": url(**action.url_args), "label": action.label, "target": action.target}
-            )
-        for operation in [op for op in self.operations if op.async_compatible]:
-            grid_config["async_ops"].append(operation.label.lower())
-        for column in self.columns:
-            if column.filterable is not None and not isinstance(column, TextColumn):
-                grid_config["categorical_filters"][column.key] = {
-                    filter.label: filter.args for filter in column.get_accepted_filters()
-                }
-        for item in query:
-            item_dict = {
-                "id": item.id,
-                "encode_id": trans.security.encode_id(item.id),
-                "link": [],
-                "operation_config": {},
-                "column_config": {},
-            }
-            for column in self.columns:
-                if column.visible:
-                    link = column.get_link(trans, self, item)
-                    if link:
-                        link = url(**link)
-                    else:
-                        link = None
-                    target = column.target
-                    value = unicodify(column.get_value(trans, self, item))
-                    if value:
-                        value = value.replace("/", "//")
-                    item_dict["column_config"][column.label] = {"link": link, "value": value, "target": target}
-            for operation in self.operations:
-                item_dict["operation_config"][operation.label] = {
-                    "allowed": operation.allowed(item),
-                    "url_args": url(**operation.get_url_args(item)),
-                    "target": operation.target,
-                }
-            grid_config["items"].append(item_dict)
-
-        if self.use_paging and num_pages is None:
-            # TODO: it would be better to just return this as None, render, and fire
-            # off a second request for this count I think.
-            total_num_rows = total_row_count_query.count()
-            num_pages = int(math.ceil(float(total_num_rows) / self.num_rows_per_page))
-
-        grid_config["num_pages"] = num_pages
-
+        page = trans.fill_template(
+            iff(async_request, self.async_template, self.template),
+            grid=self,
+            query=query,
+            cur_page_num=page_num,
+            num_pages=num_pages,
+            num_page_links=self.num_page_links,
+            allow_fetching_all_results=self.allow_fetching_all_results,
+            default_filter_dict=self.default_filter,
+            cur_filter_dict=cur_filter_dict,
+            sort_key=sort_key,
+            current_item=current_item,
+            ids=kwargs.get("id", []),
+            url=url,
+            status=status,
+            message=message,
+            info_text=self.info_text,
+            use_panels=self.use_panels,
+            use_hide_message=self.use_hide_message,
+            advanced_search=self.advanced_search,
+            show_item_checkboxes=(
+                self.show_item_checkboxes or kwargs.get("show_item_checkboxes", "") in ["True", "true"]
+            ),
+            # Pass back kwargs so that grid template can set and use args without
+            # grid explicitly having to pass them.
+            kwargs=kwargs,
+        )
         trans.log_action(trans.get_user(), "grid.view", context, params)
-        return grid_config
+        return page
 
     def get_ids(self, **kwargs):
         id = []
         if "id" in kwargs:
             id = kwargs["id"]
             # Coerce ids to list
             if not isinstance(id, list):
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/helpers/tags.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/error.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         return "<NoDefault>"
 
 
 NoDefault = _NoDefault()
 
 
 class ErrorMiddleware:
-
     """
     Error handling middleware
 
     Usage::
 
         error_catching_wsgi_app = ErrorMiddleware(wsgi_app)
 
@@ -219,15 +218,14 @@
         self.response_started = True
         # Return whatever the wrapped start_response would have
         # returned
         return self.start_response(*args)
 
 
 class CatchingIter:
-
     """
     A wrapper around the application iterator that will catch
     exceptions raised by the a generator, or by the close method, and
     display or report as necessary.
     """
 
     def __init__(self, app_iter, environ, start_checker, error_middleware):
@@ -282,15 +280,14 @@
             return None
         except Exception:
             close_response = self.error_middleware.exception_handler(sys.exc_info(), self.environ)
             return close_response
 
 
 class Supplement:
-
     """
     This is a supplement used to display standard WSGI information in
     the traceback.
     """
 
     def __init__(self, middleware, environ):
         self.middleware = middleware
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/profile.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/profile.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Middleware that profiles the request with cProfile and displays profiling
 information at the bottom of each page.
 """
+
 import cProfile
 import pstats
 import threading
 
 import markupsafe
 from paste import response
 
@@ -33,15 +34,14 @@
 %s
 </div>
 </div>
 """
 
 
 class ProfileMiddleware:
-
     """
     Middleware that profiles all requests.
 
     All HTML pages will have profiling information appended to them.
     The data is isolated to that single request, and does not include
     data from previous requests.
     """
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/remoteuser.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/remoteuser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Middleware for handling $REMOTE_USER if use_remote_user is enabled.
 """
+
 import logging
 import socket
 
 from galaxy.util import safe_str_cmp
 
 log = logging.getLogger(__name__)
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/sqldebug.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/sqldebug.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Per-request SQL debugging middleware.
 """
+
 import logging
 
 from galaxy.model.orm.engine_factory import (
     log_request_query_counts,
     reset_request_query_counts,
 )
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/static.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,15 @@
         if not os.path.exists(full):
             return self.not_found(environ, start_response)
         if os.path.isdir(full):
             # @@: Cache?
             return self.__class__(full)(environ, start_response)
         if environ.get("PATH_INFO") and environ.get("PATH_INFO") != "/":
             return self.error_extra_path(environ, start_response)
-        if_none_match = environ.get("HTTP_IF_NONE_MATCH")
-        if if_none_match:
+        if if_none_match := environ.get("HTTP_IF_NONE_MATCH"):
             mytime = os.stat(full).st_mtime
             if str(mytime) == if_none_match:
                 headers: List[Tuple[str, str]] = []
                 ETAG.update(headers, mytime)
                 start_response("304 Not Modified", headers)
                 return [""]  # empty body
         app = FileApp(full)
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/statsd.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/statsd.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/translogger.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/translogger.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/framework/middleware/xforwardedhost.py` & `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/xforwardedhost.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,20 @@
     based on the X-Forwarded-Host header IF found
     """
 
     def __init__(self, app, global_conf=None):
         self.app = app
 
     def __call__(self, environ, start_response):
-        x_forwarded_host = environ.get("HTTP_X_FORWARDED_HOST", None)
-        if x_forwarded_host:
+        if x_forwarded_host := environ.get("HTTP_X_FORWARDED_HOST", None):
             environ["ORGINAL_HTTP_HOST"] = environ["HTTP_HOST"]
             environ["HTTP_HOST"] = x_forwarded_host.split(", ", 1)[0]
-        x_forwarded_for = environ.get("HTTP_X_FORWARDED_FOR", None)
-        if x_forwarded_for:
+        if x_forwarded_for := environ.get("HTTP_X_FORWARDED_FOR", None):
             environ["ORGINAL_REMOTE_ADDR"] = environ["REMOTE_ADDR"]
             environ["REMOTE_ADDR"] = x_forwarded_for.split(",", 1)[0].strip()
         x_forwarded_proto = environ.get("HTTP_X_FORWARDED_PROTO", None)
         if x_forwarded_proto:
             x_forwarded_proto = x_forwarded_proto.split(",", 1)[0].strip()
-        x_url_scheme = environ.get("HTTP_X_URL_SCHEME", x_forwarded_proto)
-        if x_url_scheme:
+        if x_url_scheme := environ.get("HTTP_X_URL_SCHEME", x_forwarded_proto):
             environ["original_wsgi.url_scheme"] = environ["wsgi.url_scheme"]
             environ["wsgi.url_scheme"] = x_url_scheme
         return self.app(environ, start_response)
```

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/proxy/__init__.py` & `galaxy-web-framework-24.0.0/galaxy/web/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/proxy/js/Dockerfile` & `galaxy-web-framework-24.0.0/galaxy/web/proxy/js/Dockerfile`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/proxy/js/lib/main.js` & `galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/main.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/proxy/js/lib/mapper.js` & `galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/mapper.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/proxy/js/lib/proxy.js` & `galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/proxy.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.2.1/galaxy/web/statsd_client.py` & `galaxy-web-framework-24.0.0/galaxy/web/statsd_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,34 +50,31 @@
 
 CURRENT_TEST: Optional[str] = None
 CURRENT_TEST_METRICS: Optional[Dict[str, Dict]] = None
 
 
 class PyTestGalaxyStatsdClient(VanillaGalaxyStatsdClient):
     def timing(self, path, time, tags=None):
-        metrics = CURRENT_TEST_METRICS
-        if metrics is not None:
+        if (metrics := CURRENT_TEST_METRICS) is not None:
             timing = metrics["timing"]
             if path not in timing:
                 timing[path] = []
             timing[path].append({"time": time, "tags": tags})
         super().timing(path, time, tags=tags)
 
     def incr(self, path, n=1, tags=None):
-        metrics = CURRENT_TEST_METRICS
-        if metrics is not None:
+        if (metrics := CURRENT_TEST_METRICS) is not None:
             counter = metrics["counter"]
             if path not in counter:
                 counter[path] = []
             counter[path].append({"n": n, "tags": tags})
         super().incr(path, n=n, tags=tags)
 
     def _effective_infix(self, path, tags):
-        current_test = CURRENT_TEST
-        if current_test is not None:
+        if (current_test := CURRENT_TEST) is not None:
             tags = tags or {}
             tags["test"] = current_test
         return super()._effective_infix(path, tags)
 
 
 class MockStatsClient:
     def timing(self, path, time, tags=None):
```

### Comparing `galaxy-web-framework-23.2.1/galaxy_web_framework.egg-info/PKG-INFO` & `galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-util
+Requires-Dist: babel
+Requires-Dist: MarkupSafe
+Requires-Dist: paste
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: requests
+Requires-Dist: Routes
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: WebOb
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-framework.svg
    :target: https://pypi.org/project/galaxy-web-framework/
 
 
 Overview
@@ -42,14 +52,31 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Removes outdated Grid controller and backbone modules by `@guerler <https://github.com/guerler>`_ in `#17434 <https://github.com/galaxyproject/galaxy/pull/17434>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-web-framework-23.2.1/galaxy_web_framework.egg-info/SOURCES.txt` & `galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,13 +32,12 @@
 galaxy/web/proxy/__init__.py
 galaxy/web/proxy/js/Dockerfile
 galaxy/web/proxy/js/README.md
 galaxy/web/proxy/js/package.json
 galaxy/web/proxy/js/lib/main.js
 galaxy/web/proxy/js/lib/mapper.js
 galaxy/web/proxy/js/lib/proxy.js
-galaxy/web/short_term_storage/__init__.py
 galaxy_web_framework.egg-info/PKG-INFO
 galaxy_web_framework.egg-info/SOURCES.txt
 galaxy_web_framework.egg-info/dependency_links.txt
 galaxy_web_framework.egg-info/requires.txt
 galaxy_web_framework.egg-info/top_level.txt
```

### Comparing `galaxy-web-framework-23.2.1/setup.cfg` & `galaxy-web-framework-24.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -5,49 +5,49 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy web framework
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-framework
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 	babel
 	MarkupSafe
 	paste
-	pydantic<2
+	pydantic>=2,!=2.6.0,!=2.6.1
 	requests
 	Routes
 	SQLAlchemy>=1.4.25,<2
 	WebOb
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

