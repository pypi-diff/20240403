# Comparing `tmp/style50-2.9.0.tar.gz` & `tmp/style50-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "style50-2.9.0.tar", last modified: Fri Oct 27 20:00:32 2023, max compression
+gzip compressed data, was "style50-2.9.1.tar", last modified: Sun Nov 19 06:10:49 2023, max compression
```

## Comparing `style50-2.9.0.tar` & `style50-2.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 20:00:32.533864 style50-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-27 20:00:15.000000 style50-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-27 20:00:15.000000 style50-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2023-10-27 20:00:32.533864 style50-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-10-27 20:00:15.000000 style50-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 20:00:32.533864 style50-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-10-27 20:00:15.000000 style50-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 20:00:32.533864 style50-2.9.0/style50/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-10-27 20:00:15.000000 style50-2.9.0/style50/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-10-27 20:00:15.000000 style50-2.9.0/style50/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13840 2023-10-27 20:00:15.000000 style50-2.9.0/style50/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-10-27 20:00:15.000000 style50-2.9.0/style50/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 20:00:32.533864 style50-2.9.0/style50/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-27 20:00:15.000000 style50-2.9.0/style50/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-10-27 20:00:15.000000 style50-2.9.0/style50/renderer/_renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 20:00:32.533864 style50-2.9.0/style50/renderer/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-10-27 20:00:15.000000 style50-2.9.0/style50/renderer/templates/results.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 20:00:32.533864 style50-2.9.0/style50.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2023-10-27 20:00:32.000000 style50-2.9.0/style50.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-10-27 20:00:32.000000 style50-2.9.0/style50.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-27 20:00:32.000000 style50-2.9.0/style50.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-27 20:00:32.000000 style50-2.9.0/style50.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-27 20:00:32.000000 style50-2.9.0/style50.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-27 20:00:32.000000 style50-2.9.0/style50.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 06:10:49.832689 style50-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-19 06:10:35.000000 style50-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-19 06:10:35.000000 style50-2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2023-11-19 06:10:49.832689 style50-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-11-19 06:10:35.000000 style50-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-19 06:10:49.832689 style50-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-11-19 06:10:35.000000 style50-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 06:10:49.828689 style50-2.9.1/style50/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2023-11-19 06:10:35.000000 style50-2.9.1/style50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-11-19 06:10:35.000000 style50-2.9.1/style50/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13840 2023-11-19 06:10:35.000000 style50-2.9.1/style50/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-11-19 06:10:35.000000 style50-2.9.1/style50/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 06:10:49.832689 style50-2.9.1/style50/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-19 06:10:35.000000 style50-2.9.1/style50/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-11-19 06:10:35.000000 style50-2.9.1/style50/renderer/_renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 06:10:49.832689 style50-2.9.1/style50/renderer/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-11-19 06:10:35.000000 style50-2.9.1/style50/renderer/templates/results.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 06:10:49.828689 style50-2.9.1/style50.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2023-11-19 06:10:49.000000 style50-2.9.1/style50.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-19 06:10:49.000000 style50-2.9.1/style50.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-19 06:10:49.000000 style50-2.9.1/style50.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-19 06:10:49.000000 style50-2.9.1/style50.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-19 06:10:49.000000 style50-2.9.1/style50.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-19 06:10:49.000000 style50-2.9.1/style50.egg-info/top_level.txt
```

### Comparing `style50-2.9.0/LICENSE` & `style50-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `style50-2.9.0/PKG-INFO` & `style50-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: style50
-Version: 2.9.0
+Version: 2.9.1
 Summary: This is style50, with which code can be checked against the CS50 style guide
 Home-page: https://github.com/cs50/style50
 Author: CS50
 Author-email: sysadmins@cs50.harvard.edu
 License: GPLv3
 Keywords: style,style50
 Classifier: Intended Audience :: Education
```

### Comparing `style50-2.9.0/README.md` & `style50-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `style50-2.9.0/setup.py` & `style50-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     entry_points={
         "console_scripts": [
             "style50=style50.__main__:main",
             "style50-cli=style50.__main__:main",
         ]
     },
     url="https://github.com/cs50/style50",
-    version="2.9.0",
+    version="2.9.1",
     include_package_data=True,
 )
```

### Comparing `style50-2.9.0/style50/__main__.py` & `style50-2.9.1/style50/__main__.py`

 * *Files identical despite different names*

### Comparing `style50-2.9.0/style50/_api.py` & `style50-2.9.1/style50/_api.py`

 * *Files identical despite different names*

### Comparing `style50-2.9.0/style50/languages.py` & `style50-2.9.1/style50/languages.py`

 * *Files identical despite different names*

### Comparing `style50-2.9.0/style50/renderer/_renderers.py` & `style50-2.9.1/style50/renderer/_renderers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import pathlib
 
 import jinja2
-import pkg_resources
 import termcolor
 
+from importlib.resources import files
 
-TEMPLATES = pathlib.Path(pkg_resources.resource_filename("style50.renderer", "templates"))
+
+TEMPLATES = pathlib.Path(files("style50.renderer").joinpath("templates"))
 
 
 def to_ansi(files, score, version):
         lines = [termcolor.colored("Results generated by style50 v{}".format(version), "white", attrs=["bold"])]
 
         # Use same header as more.
         header = termcolor.colored("{0}\n{{}}\n{0}".format(
```

### Comparing `style50-2.9.0/style50/renderer/templates/results.html` & `style50-2.9.1/style50/renderer/templates/results.html`

 * *Files identical despite different names*

### Comparing `style50-2.9.0/style50.egg-info/PKG-INFO` & `style50-2.9.1/style50.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: style50
-Version: 2.9.0
+Version: 2.9.1
 Summary: This is style50, with which code can be checked against the CS50 style guide
 Home-page: https://github.com/cs50/style50
 Author: CS50
 Author-email: sysadmins@cs50.harvard.edu
 License: GPLv3
 Keywords: style,style50
 Classifier: Intended Audience :: Education
```

