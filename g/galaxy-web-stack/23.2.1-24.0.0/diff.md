# Comparing `tmp/galaxy-web-stack-23.2.1.tar.gz` & `tmp/galaxy-web-stack-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_stack/dist/.tmp-yrqypwac/galaxy-web-stack-23.2.1.tar", last modified: Thu Feb 22 03:56:25 2024, max compression
+gzip compressed data, was "galaxy-web-stack-24.0.0.tar", last modified: Wed Apr  3 02:46:26 2024, max compression
```

## Comparing `galaxy-web-stack-23.2.1.tar` & `galaxy-web-stack-24.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/galaxy/web_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/galaxy/web_stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/galaxy/web_stack/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/galaxy/web_stack/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/galaxy/web_stack/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/galaxy/web_stack/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/galaxy_web_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/galaxy_web_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/galaxy_web_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/galaxy_web_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/galaxy_web_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/galaxy_web_stack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-22 03:56:25.000000 galaxy-web-stack-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-22 03:50:43.000000 galaxy-web-stack-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:26.532101 galaxy-web-stack-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-03 02:46:26.532101 galaxy-web-stack-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:26.528101 galaxy-web-stack-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:26.528101 galaxy-web-stack-24.0.0/galaxy/web_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/galaxy/web_stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/galaxy/web_stack/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/galaxy/web_stack/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/galaxy/web_stack/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/galaxy/web_stack/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:26.532101 galaxy-web-stack-24.0.0/galaxy_web_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-03 02:46:26.000000 galaxy-web-stack-24.0.0/galaxy_web_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-03 02:46:26.000000 galaxy-web-stack-24.0.0/galaxy_web_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:26.000000 galaxy-web-stack-24.0.0/galaxy_web_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 02:46:26.000000 galaxy-web-stack-24.0.0/galaxy_web_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:46:26.000000 galaxy-web-stack-24.0.0/galaxy_web_stack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-03 02:46:26.532101 galaxy-web-stack-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 02:43:42.000000 galaxy-web-stack-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-web-stack-23.2.1/HISTORY.rst` & `galaxy-web-stack-24.0.0/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,24 @@
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
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-web-stack-23.2.1/LICENSE` & `galaxy-web-stack-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.2.1/PKG-INFO` & `galaxy-web-stack-24.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy web stack abstraction
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
+Requires-Dist: SQLAlchemy<2,>=1.4.25
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-stack.svg
    :target: https://pypi.python.org/pypi/galaxy-web-stack/
 
 
 Overview
@@ -42,14 +45,25 @@
 
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
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-web-stack-23.2.1/galaxy/web_stack/__init__.py` & `galaxy-web-stack-24.0.0/galaxy/web_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.2.1/galaxy/web_stack/gunicorn_config.py` & `galaxy-web-stack-24.0.0/galaxy/web_stack/gunicorn_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Gunicorn config file based on https://gist.github.com/hynek/ba655c8756924a5febc5285c712a7946
 """
+
 import gc
 import os
 import sys
 
 
 def is_preload_app():
     return "--preload" in os.environ.get("GUNICORN_CMD_ARGS", "") or "--preload" in sys.argv
```

### Comparing `galaxy-web-stack-23.2.1/galaxy/web_stack/handlers.py` & `galaxy-web-stack-24.0.0/galaxy/web_stack/handlers.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.2.1/galaxy/web_stack/message.py` & `galaxy-web-stack-24.0.0/galaxy/web_stack/message.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.2.1/galaxy/web_stack/transport.py` & `galaxy-web-stack-24.0.0/galaxy/web_stack/transport.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.2.1/galaxy_web_stack.egg-info/PKG-INFO` & `galaxy-web-stack-24.0.0/galaxy_web_stack.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy web stack abstraction
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
+Requires-Dist: SQLAlchemy<2,>=1.4.25
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-stack.svg
    :target: https://pypi.python.org/pypi/galaxy-web-stack/
 
 
 Overview
@@ -42,14 +45,25 @@
 
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
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-web-stack-23.2.1/setup.cfg` & `galaxy-web-stack-24.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,42 +5,42 @@
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
 description = Galaxy web stack abstraction
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-stack
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 	SQLAlchemy>=1.4.25,<2
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

