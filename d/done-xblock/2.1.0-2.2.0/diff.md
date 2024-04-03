# Comparing `tmp/done-xblock-2.1.0.tar.gz` & `tmp/done-xblock-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "done-xblock-2.1.0.tar", last modified: Fri Jul 21 14:27:17 2023, max compression
+gzip compressed data, was "done-xblock-2.2.0.tar", last modified: Thu Nov  2 08:55:55 2023, max compression
```

## Comparing `done-xblock-2.1.0.tar` & `done-xblock-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.918882 done-xblock-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-07-21 14:27:14.000000 done-xblock-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-21 14:27:14.000000 done-xblock-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-21 14:27:14.000000 done-xblock-2.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)     5658 2023-07-21 14:27:17.918882 done-xblock-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4370 2023-07-21 14:27:14.000000 done-xblock-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/done.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/public/
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/public/check-empty.png
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/public/check-full.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/static/css/done.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/static/js/src/done.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.918882 done-xblock-2.1.0/done/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      794 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/templates/done.html
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/templates/studioview.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.918882 done-xblock-2.1.0/done_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5658 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.918882 done-xblock-2.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-21 14:27:14.000000 done-xblock-2.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-21 14:27:14.000000 done-xblock-2.1.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 14:27:17.918882 done-xblock-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-07-21 14:27:14.000000 done-xblock-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.480941 done-xblock-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2023-11-02 08:55:52.000000 done-xblock-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-02 08:55:52.000000 done-xblock-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2023-11-02 08:55:52.000000 done-xblock-2.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2023-11-02 08:55:55.480941 done-xblock-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2023-11-02 08:55:52.000000 done-xblock-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.476941 done-xblock-2.2.0/done/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-02 08:55:52.000000 done-xblock-2.2.0/done/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2023-11-02 08:55:52.000000 done-xblock-2.2.0/done/done.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.480941 done-xblock-2.2.0/done/public/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-11-02 08:55:52.000000 done-xblock-2.2.0/done/public/check-empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2023-11-02 08:55:52.000000 done-xblock-2.2.0/done/public/check-full.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.476941 done-xblock-2.2.0/done/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.480941 done-xblock-2.2.0/done/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-11-02 08:55:52.000000 done-xblock-2.2.0/done/static/css/done.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.476941 done-xblock-2.2.0/done/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.480941 done-xblock-2.2.0/done/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-11-02 08:55:52.000000 done-xblock-2.2.0/done/static/js/src/done.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.480941 done-xblock-2.2.0/done/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-11-02 08:55:52.000000 done-xblock-2.2.0/done/templates/done.html
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-11-02 08:55:52.000000 done-xblock-2.2.0/done/templates/studioview.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.480941 done-xblock-2.2.0/done_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2023-11-02 08:55:55.000000 done-xblock-2.2.0/done_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-11-02 08:55:55.000000 done-xblock-2.2.0/done_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 08:55:55.000000 done-xblock-2.2.0/done_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-02 08:55:55.000000 done-xblock-2.2.0/done_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-02 08:55:55.000000 done-xblock-2.2.0/done_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-02 08:55:55.000000 done-xblock-2.2.0/done_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 08:55:55.480941 done-xblock-2.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2023-11-02 08:55:52.000000 done-xblock-2.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-11-02 08:55:52.000000 done-xblock-2.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 08:55:55.480941 done-xblock-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2023-11-02 08:55:52.000000 done-xblock-2.2.0/setup.py
```

### Comparing `done-xblock-2.1.0/LICENSE` & `done-xblock-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `done-xblock-2.1.0/NOTICE` & `done-xblock-2.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `done-xblock-2.1.0/PKG-INFO` & `done-xblock-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: done-xblock
-Version: 2.1.0
+Version: 2.2.0
 Summary: done XBlock
-Home-page: UNKNOWN
+Home-page: https://github.com/openedx/DoneXBlock
 License: UNKNOWN
 Description: ##########
         DoneXBlock
         ##########
         | |License: AGPL v3| |Status| |Python CI| |Publish package to PyPi|
         
         .. |License: AGPL v3| image:: https://img.shields.io/badge/License-AGPL_v3-blue.svg
@@ -104,15 +104,15 @@
         may be found in `Backstage`_ or groked from inspecting catalog-info.yaml.
         
         .. _Backstage: https://open-edx-backstage.herokuapp.com/catalog/default/component/DoneXBlock
         
         Reporting Security Issues
         =========================
         
-        Please do not report security issues in public. Please email security@edx.org.
+        Please do not report security issues in public. Please email security@openedx.org.
         
         
         History
         =======
         
         FutureLearn uses this kind of thing to great effect. Students can read
         text, watch videos, etc., and indicate when their done. This is
```

### Comparing `done-xblock-2.1.0/README.rst` & `done-xblock-2.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 may be found in `Backstage`_ or groked from inspecting catalog-info.yaml.
 
 .. _Backstage: https://open-edx-backstage.herokuapp.com/catalog/default/component/DoneXBlock
 
 Reporting Security Issues
 =========================
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 History
 =======
 
 FutureLearn uses this kind of thing to great effect. Students can read
 text, watch videos, etc., and indicate when their done. This is
```

### Comparing `done-xblock-2.1.0/done/done.py` & `done-xblock-2.2.0/done/done.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 import uuid
 
 import pkg_resources
 from web_fragments.fragment import Fragment
 from xblock.core import XBlock
 from xblock.fields import Boolean, DateTime, Float, Scope, String
-from xblockutils.resources import ResourceLoader
+try:
+    from xblock.utils.resources import ResourceLoader
+except ModuleNotFoundError:  # For backward compatibility with releases older than Quince.
+    from xblockutils.resources import ResourceLoader
 
 resource_loader = ResourceLoader(__name__)
 
 
 def _(text):
     """
     Make '_' a no-op, so we can scrape strings
```

### Comparing `done-xblock-2.1.0/done/static/css/done.css` & `done-xblock-2.2.0/done/static/css/done.css`

 * *Files identical despite different names*

### Comparing `done-xblock-2.1.0/done/static/js/src/done.js` & `done-xblock-2.2.0/done/static/js/src/done.js`

 * *Files identical despite different names*

### Comparing `done-xblock-2.1.0/done/templates/done.html` & `done-xblock-2.2.0/done/templates/done.html`

 * *Files identical despite different names*

### Comparing `done-xblock-2.1.0/done/templates/studioview.html` & `done-xblock-2.2.0/done/templates/studioview.html`

 * *Files identical despite different names*

### Comparing `done-xblock-2.1.0/done_xblock.egg-info/PKG-INFO` & `done-xblock-2.2.0/done_xblock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: done-xblock
-Version: 2.1.0
+Version: 2.2.0
 Summary: done XBlock
-Home-page: UNKNOWN
+Home-page: https://github.com/openedx/DoneXBlock
 License: UNKNOWN
 Description: ##########
         DoneXBlock
         ##########
         | |License: AGPL v3| |Status| |Python CI| |Publish package to PyPi|
         
         .. |License: AGPL v3| image:: https://img.shields.io/badge/License-AGPL_v3-blue.svg
@@ -104,15 +104,15 @@
         may be found in `Backstage`_ or groked from inspecting catalog-info.yaml.
         
         .. _Backstage: https://open-edx-backstage.herokuapp.com/catalog/default/component/DoneXBlock
         
         Reporting Security Issues
         =========================
         
-        Please do not report security issues in public. Please email security@edx.org.
+        Please do not report security issues in public. Please email security@openedx.org.
         
         
         History
         =======
         
         FutureLearn uses this kind of thing to great effect. Students can read
         text, watch videos, etc., and indicate when their done. This is
```

### Comparing `done-xblock-2.1.0/requirements/constraints.txt` & `done-xblock-2.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

