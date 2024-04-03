# Comparing `tmp/galaxy-files-23.2.1.tar.gz` & `tmp/galaxy-files-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/files/dist/.tmp-_0l8203m/galaxy-files-23.2.1.tar", last modified: Thu Feb 22 03:51:48 2024, max compression
+gzip compressed data, was "galaxy-files-24.0.0.tar", last modified: Wed Apr  3 02:44:16 2024, max compression
```

## Comparing `galaxy-files-23.2.1.tar` & `galaxy-files-24.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy/files/
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy/files/sources/
--rw-r--r--   0 runner    (1001) docker     (127)    18971 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/_pyfilesystem2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/_rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/anvil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/basespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/drs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/googlecloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/invenio.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/onedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/posix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/sources/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy/files/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/files/uris.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/galaxy_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-22 03:51:48.000000 galaxy-files-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-22 03:50:43.000000 galaxy-files-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.762559 galaxy-files-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-03 02:44:16.762559 galaxy-files-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.754559 galaxy-files-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.754559 galaxy-files-24.0.0/galaxy/files/
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.758559 galaxy-files-24.0.0/galaxy/files/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    18971 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/_pyfilesystem2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/_rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/anvil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/basespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/invenio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/onedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/posix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.758559 galaxy-files-24.0.0/galaxy/files/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/uris.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.762559 galaxy-files-24.0.0/galaxy_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-03 02:44:16.762559 galaxy-files-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-files-23.2.1/HISTORY.rst` & `galaxy-files-24.0.0/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,28 @@
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
+* Add support for Python 3.12 by `@tuncK <https://github.com/tuncK>`_ in `#16796 <https://github.com/galaxyproject/galaxy/pull/16796>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* fix s3fs templating by `@bgruening <https://github.com/bgruening>`_ in `#17311 <https://github.com/galaxyproject/galaxy/pull/17311>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -19,15 +34,15 @@
 
 ============
 Enhancements
 ============
 
 * Add Invenio RDM repository integration by `@davelopez <https://github.com/davelopez>`_ in `#16381 <https://github.com/galaxyproject/galaxy/pull/16381>`_
 * Refactor FilesDialog + Remote Files API schema improvements by `@davelopez <https://github.com/davelopez>`_ in `#16420 <https://github.com/galaxyproject/galaxy/pull/16420>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Remove record access handling for Invenio RDM plugin by `@davelopez <https://github.com/davelopez>`_ in `#16900 <https://github.com/galaxyproject/galaxy/pull/16900>`_
 * Enhance Invenio RDM integration by `@davelopez <https://github.com/davelopez>`_ in `#16964 <https://github.com/galaxyproject/galaxy/pull/16964>`_
 
 -------------------
 23.1.4 (2024-01-04)
 -------------------
```

### Comparing `galaxy-files-23.2.1/LICENSE.txt` & `galaxy-files-24.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/PKG-INFO` & `galaxy-files-24.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy file source framework and default plugins
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
+Requires-Dist: galaxy-util
+Requires-Dist: fs
+Requires-Dist: isal
+Requires-Dist: typing-extensions
 
 
 .. image:: https://badge.fury.io/py/galaxy-files.svg
    :target: https://pypi.org/project/galaxy-files/
 
 
 
@@ -42,14 +46,29 @@
 
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
+* Add support for Python 3.12 by `@tuncK <https://github.com/tuncK>`_ in `#16796 <https://github.com/galaxyproject/galaxy/pull/16796>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* fix s3fs templating by `@bgruening <https://github.com/bgruening>`_ in `#17311 <https://github.com/galaxyproject/galaxy/pull/17311>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -61,15 +80,15 @@
 
 ============
 Enhancements
 ============
 
 * Add Invenio RDM repository integration by `@davelopez <https://github.com/davelopez>`_ in `#16381 <https://github.com/galaxyproject/galaxy/pull/16381>`_
 * Refactor FilesDialog + Remote Files API schema improvements by `@davelopez <https://github.com/davelopez>`_ in `#16420 <https://github.com/galaxyproject/galaxy/pull/16420>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Remove record access handling for Invenio RDM plugin by `@davelopez <https://github.com/davelopez>`_ in `#16900 <https://github.com/galaxyproject/galaxy/pull/16900>`_
 * Enhance Invenio RDM integration by `@davelopez <https://github.com/davelopez>`_ in `#16964 <https://github.com/galaxyproject/galaxy/pull/16964>`_
 
 -------------------
 23.1.4 (2024-01-04)
 -------------------
```

### Comparing `galaxy-files-23.2.1/galaxy/files/__init__.py` & `galaxy-files-24.0.0/galaxy/files/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/__init__.py` & `galaxy-files-24.0.0/galaxy/files/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/_pyfilesystem2.py` & `galaxy-files-24.0.0/galaxy/files/sources/_pyfilesystem2.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/_rdm.py` & `galaxy-files-24.0.0/galaxy/files/sources/_rdm.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/anvil.py` & `galaxy-files-24.0.0/galaxy/files/sources/anvil.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/base64.py` & `galaxy-files-24.0.0/galaxy/files/sources/base64.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/basespace.py` & `galaxy-files-24.0.0/galaxy/files/sources/basespace.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/dropbox.py` & `galaxy-files-24.0.0/galaxy/files/sources/dropbox.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/drs.py` & `galaxy-files-24.0.0/galaxy/files/sources/drs.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,16 +60,15 @@
             force_http=self._force_http,
         )
 
     def _write_from(self, target_path, native_path, user_context=None, opts: Optional[FilesSourceOptions] = None):
         raise NotImplementedError()
 
     def score_url_match(self, url: str):
-        match = self._url_regex.match(url)
-        if match:
+        if match := self._url_regex.match(url):
             return match.span()[1]
         else:
             return 0
 
     def _serialization_props(self, user_context=None) -> DRSFilesSourceProperties:
         effective_props = {}
         for key, val in self._props.items():
```

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/ftp.py` & `galaxy-files-24.0.0/galaxy/files/sources/ftp.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/galaxy.py` & `galaxy-files-24.0.0/galaxy/files/sources/galaxy.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/googlecloudstorage.py` & `galaxy-files-24.0.0/galaxy/files/sources/googlecloudstorage.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/googledrive.py` & `galaxy-files-24.0.0/galaxy/files/sources/googledrive.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/http.py` & `galaxy-files-24.0.0/galaxy/files/sources/http.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/invenio.py` & `galaxy-files-24.0.0/galaxy/files/sources/invenio.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
             file_details_url = self._to_draft_url(file_details_url)
             download_file_content_url = self._to_draft_url(download_file_content_url)
         file_details = self._get_response(user_context, file_details_url)
         if not self._can_download_from_api(file_details):
             # TODO: This is a temporary workaround for the fact that the "content" API
             # does not support downloading files from S3 or other remote storage classes.
             # More info: https://inveniordm.docs.cern.ch/reference/file_storage/#remote-files-r
-            download_file_content_url = f"{file_details_url.replace('/api','')}?download=1"
+            download_file_content_url = f"{file_details_url.replace('/api', '')}?download=1"
         return download_file_content_url
 
     def _is_api_url(self, url: str) -> bool:
         return "/api/" in url
 
     def _to_draft_url(self, url: str) -> str:
         return url.replace("/files/", "/draft/files/")
```

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/onedata.py` & `galaxy-files-24.0.0/galaxy/files/sources/onedata.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/posix.py` & `galaxy-files-24.0.0/galaxy/files/sources/posix.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/s3fs.py` & `galaxy-files-24.0.0/galaxy/files/sources/s3fs.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,54 +40,68 @@
 class S3FsFilesSource(BaseFilesSource):
     plugin_type = "s3fs"
 
     def __init__(self, **kwd: Unpack[S3FsFilesSourceProperties]):
         if s3fs is None:
             raise Exception("Package s3fs unavailable but required for this file source plugin.")
         props: S3FsFilesSourceProperties = cast(S3FsFilesSourceProperties, self._parse_common_config_opts(kwd))
-        self._bucket = props.pop("bucket", "")
+        # There is a possibility that the bucket name could be parameterized: e.g.
+        # bucket: ${user.preferences['generic_s3|bucket']}
+        # that's ok, because we evaluate the bucket name again later. The bucket property here will only
+        # be used by `score_url_match`. In the case of a parameterized bucket name, we will always return
+        # a score of 4 as the url will only match the s3:// part.
+        self._bucket = props.get("bucket", "")
         self._endpoint_url = props.pop("endpoint_url", None)
         self._props = props
         if self._endpoint_url:
             self._props.update({"client_kwargs": {"endpoint_url": self._endpoint_url}})
 
     def _list(self, path="/", recursive=True, user_context=None, opts: Optional[FilesSourceOptions] = None):
-        fs = self._open_fs(user_context=user_context, opts=opts)
+        _props = self._serialization_props(user_context)
+        # we need to pop the 'bucket' here, because the argument is not recognised in a downstream function
+        _bucket_name = _props.pop("bucket", "")
+        fs = self._open_fs(props=_props, opts=opts)
         if recursive:
             res: List[Dict[str, Any]] = []
-            bucket_path = self._bucket_path(path)
+            bucket_path = self._bucket_path(_bucket_name, path)
             for p, dirs, files in fs.walk(bucket_path, detail=True):
                 to_dict = functools.partial(self._resource_info_to_dict, p)
                 res.extend(map(to_dict, dirs.values()))
                 res.extend(map(to_dict, files.values()))
             return res
         else:
-            bucket_path = self._bucket_path(path)
+            bucket_path = self._bucket_path(_bucket_name, path)
             res = fs.ls(bucket_path, detail=True)
             to_dict = functools.partial(self._resource_info_to_dict, path)
             return list(map(to_dict, res))
 
     def _realize_to(self, source_path, native_path, user_context=None, opts: Optional[FilesSourceOptions] = None):
-        bucket_path = self._bucket_path(source_path)
-        self._open_fs(user_context=user_context, opts=opts).download(bucket_path, native_path)
+        _props = self._serialization_props(user_context)
+        _bucket_name = _props.pop("bucket", "")
+        fs = self._open_fs(props=_props, opts=opts)
+        bucket_path = self._bucket_path(_bucket_name, source_path)
+        fs.download(bucket_path, native_path)
 
     def _write_from(self, target_path, native_path, user_context=None, opts: Optional[FilesSourceOptions] = None):
-        bucket_path = self._bucket_path(target_path)
-        self._open_fs(user_context=user_context, opts=opts).upload(native_path, bucket_path)
+        _props = self._serialization_props(user_context)
+        _bucket_name = _props.pop("bucket", "")
+        fs = self._open_fs(props=_props, opts=opts)
+        bucket_path = self._bucket_path(_bucket_name, target_path)
+        fs.upload(native_path, bucket_path)
 
-    def _bucket_path(self, path: str):
+    def _bucket_path(self, bucket_name: str, path: str):
         if path.startswith("s3://"):
             return path.replace("s3://", "")
         elif not path.startswith("/"):
             path = f"/{path}"
-        return f"{self._bucket}{path}"
+        return f"{bucket_name}{path}"
 
-    def _open_fs(self, user_context=None, opts: Optional[FilesSourceOptions] = None):
+    def _open_fs(self, props: FilesSourceProperties, opts: Optional[FilesSourceOptions] = None):
         extra_props = opts.extra_props or {} if opts else {}
-        fs = s3fs.S3FileSystem(**{**self._props, **extra_props})
+        fs = s3fs.S3FileSystem(**{**props, **extra_props})
         return fs
 
     def _resource_info_to_dict(self, dir_path: str, resource_info):
         name = os.path.basename(resource_info["name"])
         path = os.path.join(dir_path, name)
         uri = self.uri_from_path(path)
         if resource_info["type"] == "directory":
@@ -99,20 +113,19 @@
                 "size": resource_info["size"],
                 # should this be mtime...
                 "ctime": self.to_dict_time(resource_info["LastModified"]),
                 "uri": uri,
                 "path": path,
             }
 
-    def _serialization_props(self, user_context=None):
+    def _serialization_props(self, user_context=None) -> S3FsFilesSourceProperties:
         effective_props = {}
         for key, val in self._props.items():
             effective_props[key] = self._evaluate_prop(val, user_context=user_context)
-        effective_props["bucket"] = self._bucket
-        return effective_props
+        return cast(S3FsFilesSourceProperties, effective_props)
 
     def score_url_match(self, url: str):
         # For security, we need to ensure that a partial match doesn't work. e.g. s3://{bucket}something/myfiles
         if self._bucket and (url.startswith(f"s3://{self._bucket}/") or url == f"s3://{self._bucket}"):
             return len(f"s3://{self._bucket}")
         elif not self._bucket and url.startswith("s3://"):
             return len("s3://")
```

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/ssh.py` & `galaxy-files-24.0.0/galaxy/files/sources/ssh.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/sources/webdav.py` & `galaxy-files-24.0.0/galaxy/files/sources/webdav.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/unittest_utils/__init__.py` & `galaxy-files-24.0.0/galaxy/files/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy/files/uris.py` & `galaxy-files-24.0.0/galaxy/files/uris.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/galaxy_files.egg-info/PKG-INFO` & `galaxy-files-24.0.0/galaxy_files.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy file source framework and default plugins
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
+Requires-Dist: galaxy-util
+Requires-Dist: fs
+Requires-Dist: isal
+Requires-Dist: typing-extensions
 
 
 .. image:: https://badge.fury.io/py/galaxy-files.svg
    :target: https://pypi.org/project/galaxy-files/
 
 
 
@@ -42,14 +46,29 @@
 
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
+* Add support for Python 3.12 by `@tuncK <https://github.com/tuncK>`_ in `#16796 <https://github.com/galaxyproject/galaxy/pull/16796>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* fix s3fs templating by `@bgruening <https://github.com/bgruening>`_ in `#17311 <https://github.com/galaxyproject/galaxy/pull/17311>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -61,15 +80,15 @@
 
 ============
 Enhancements
 ============
 
 * Add Invenio RDM repository integration by `@davelopez <https://github.com/davelopez>`_ in `#16381 <https://github.com/galaxyproject/galaxy/pull/16381>`_
 * Refactor FilesDialog + Remote Files API schema improvements by `@davelopez <https://github.com/davelopez>`_ in `#16420 <https://github.com/galaxyproject/galaxy/pull/16420>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Remove record access handling for Invenio RDM plugin by `@davelopez <https://github.com/davelopez>`_ in `#16900 <https://github.com/galaxyproject/galaxy/pull/16900>`_
 * Enhance Invenio RDM integration by `@davelopez <https://github.com/davelopez>`_ in `#16964 <https://github.com/galaxyproject/galaxy/pull/16964>`_
 
 -------------------
 23.1.4 (2024-01-04)
 -------------------
```

### Comparing `galaxy-files-23.2.1/galaxy_files.egg-info/SOURCES.txt` & `galaxy-files-24.0.0/galaxy_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.2.1/setup.cfg` & `galaxy-files-24.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,43 +5,43 @@
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
 description = Galaxy file source framework and default plugins
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-files
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	fs
 	isal
 	typing-extensions
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

