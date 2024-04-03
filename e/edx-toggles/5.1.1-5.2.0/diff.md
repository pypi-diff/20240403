# Comparing `tmp/edx-toggles-5.1.1.tar.gz` & `tmp/edx-toggles-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-toggles-5.1.1.tar", last modified: Wed Jan 31 19:43:50 2024, max compression
+gzip compressed data, was "edx-toggles-5.2.0.tar", last modified: Wed Apr  3 20:39:42 2024, max compression
```

## Comparing `edx-toggles-5.1.1.tar` & `edx-toggles-5.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.813598 edx-toggles-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35119 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-01-31 19:43:50.813598 edx-toggles-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.809598 edx-toggles-5.1.1/edx_toggles/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.809598 edx-toggles-5.1.1/edx_toggles/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/tests/test_setting_toggles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/tests/test_waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.809598 edx-toggles-5.1.1/edx_toggles/toggles/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.809598 edx-toggles-5.1.1/edx_toggles/toggles/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/internal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/internal/setting_toggle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.809598 edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.809598 edx-toggles-5.1.1/edx_toggles/toggles/state/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.813598 edx-toggles-5.1.1/edx_toggles/toggles/state/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/state/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/state/internal/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/toggles/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/edx_toggles/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.813598 edx-toggles-5.1.1/edx_toggles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-01-31 19:43:50.000000 edx-toggles-5.1.1/edx_toggles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-01-31 19:43:50.000000 edx-toggles-5.1.1/edx_toggles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 19:43:50.000000 edx-toggles-5.1.1/edx_toggles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-31 19:43:50.000000 edx-toggles-5.1.1/edx_toggles.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 19:43:50.000000 edx-toggles-5.1.1/edx_toggles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-31 19:43:50.000000 edx-toggles-5.1.1/edx_toggles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-31 19:43:50.000000 edx-toggles-5.1.1/edx_toggles.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:43:50.813598 edx-toggles-5.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-31 19:43:50.813598 edx-toggles-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-01-31 19:43:47.000000 edx-toggles-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.651953 edx-toggles-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35119 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-03 20:39:42.651953 edx-toggles-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.647953 edx-toggles-5.2.0/edx_toggles/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.647953 edx-toggles-5.2.0/edx_toggles/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/tests/test_setting_toggles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/tests/test_waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.647953 edx-toggles-5.2.0/edx_toggles/toggles/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.647953 edx-toggles-5.2.0/edx_toggles/toggles/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/internal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/internal/setting_toggle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.647953 edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.647953 edx-toggles-5.2.0/edx_toggles/toggles/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.647953 edx-toggles-5.2.0/edx_toggles/toggles/state/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/state/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/state/internal/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/toggles/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/edx_toggles/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.651953 edx-toggles-5.2.0/edx_toggles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-03 20:39:42.000000 edx-toggles-5.2.0/edx_toggles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-03 20:39:42.000000 edx-toggles-5.2.0/edx_toggles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:39:42.000000 edx-toggles-5.2.0/edx_toggles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 20:39:42.000000 edx-toggles-5.2.0/edx_toggles.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:39:42.000000 edx-toggles-5.2.0/edx_toggles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 20:39:42.000000 edx-toggles-5.2.0/edx_toggles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 20:39:42.000000 edx-toggles-5.2.0/edx_toggles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:39:42.651953 edx-toggles-5.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 20:39:42.651953 edx-toggles-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-03 20:39:39.000000 edx-toggles-5.2.0/setup.py
```

### Comparing `edx-toggles-5.1.1/CHANGELOG.rst` & `edx-toggles-5.2.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.2.0] - 2024-03-31
+--------------------
+
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
 [5.1.1] - 2024-01-31
 --------------------
 
 * Fix toggle report to output all settings.
 
 [5.1.0] - 2023-08-02
 --------------------
```

### Comparing `edx-toggles-5.1.1/LICENSE.txt` & `edx-toggles-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/PKG-INFO` & `edx-toggles-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: edx-toggles
-Version: 5.1.1
+Version: 5.2.0
 Summary: Library and utilities for feature toggles
 Home-page: https://github.com/openedx/edx-toggles
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 Requires-Dist: Django>=2.2
 Requires-Dist: code-annotations
 Requires-Dist: django-crum
 Requires-Dist: django-waffle
 Requires-Dist: edx-django-utils
 
@@ -114,14 +115,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.2.0] - 2024-03-31
+--------------------
+
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
 [5.1.1] - 2024-01-31
 --------------------
 
 * Fix toggle report to output all settings.
 
 [5.1.0] - 2023-08-02
 --------------------
```

### Comparing `edx-toggles-5.1.1/README.rst` & `edx-toggles-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/tests/test_setting_toggles.py` & `edx-toggles-5.2.0/edx_toggles/tests/test_setting_toggles.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/tests/test_state.py` & `edx-toggles-5.2.0/edx_toggles/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/tests/test_testutils.py` & `edx-toggles-5.2.0/edx_toggles/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/tests/test_waffle.py` & `edx-toggles-5.2.0/edx_toggles/tests/test_waffle.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/toggles/internal/base.py` & `edx-toggles-5.2.0/edx_toggles/toggles/internal/base.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/toggles/internal/setting_toggle.py` & `edx-toggles-5.2.0/edx_toggles/toggles/internal/setting_toggle.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/base.py` & `edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/base.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/flag.py` & `edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/flag.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/toggles/internal/waffle/switch.py` & `edx-toggles-5.2.0/edx_toggles/toggles/internal/waffle/switch.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/toggles/state/internal/report.py` & `edx-toggles-5.2.0/edx_toggles/toggles/state/internal/report.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles/toggles/testutils.py` & `edx-toggles-5.2.0/edx_toggles/toggles/testutils.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/edx_toggles.egg-info/PKG-INFO` & `edx-toggles-5.2.0/edx_toggles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: edx-toggles
-Version: 5.1.1
+Version: 5.2.0
 Summary: Library and utilities for feature toggles
 Home-page: https://github.com/openedx/edx-toggles
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 Requires-Dist: Django>=2.2
 Requires-Dist: code-annotations
 Requires-Dist: django-crum
 Requires-Dist: django-waffle
 Requires-Dist: edx-django-utils
 
@@ -114,14 +115,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.2.0] - 2024-03-31
+--------------------
+
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
 [5.1.1] - 2024-01-31
 --------------------
 
 * Fix toggle report to output all settings.
 
 [5.1.0] - 2023-08-02
 --------------------
```

### Comparing `edx-toggles-5.1.1/edx_toggles.egg-info/SOURCES.txt` & `edx-toggles-5.2.0/edx_toggles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.1.1/setup.py` & `edx-toggles-5.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,16 +118,17 @@
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

