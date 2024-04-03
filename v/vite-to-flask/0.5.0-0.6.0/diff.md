# Comparing `tmp/vite_to_flask-0.5.0.tar.gz` & `tmp/vite_to_flask-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_to_flask-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_to_flask-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_to_flask-0.5.0.tar` & `vite_to_flask-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     5173 2024-04-01 21:09:14.191229 vite_to_flask-0.5.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_to_flask-0.5.0/LICENSE
--rw-r--r--   0        0        0     2667 2024-04-02 13:53:38.931854 vite_to_flask-0.5.0/README.md
--rw-r--r--   0        0        0      349 2024-04-02 13:51:54.853593 vite_to_flask-0.5.0/app_flask_demo/__init__.py
--rw-r--r--   0        0        0       69 2024-04-01 10:28:05.818282 vite_to_flask-0.5.0/app_flask_demo/extensions/__init__.py
--rw-r--r--   0        0        0    39139 2024-04-03 07:34:09.601576 vite_to_flask-0.5.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    32826 2024-04-03 07:34:09.601913 vite_to_flask-0.5.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css
--rw-r--r--   0        0        0    20114 2024-04-03 07:34:09.602143 vite_to_flask-0.5.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js
--rw-r--r--   0        0        0      203 2024-04-01 19:32:58.177827 vite_to_flask-0.5.0/app_flask_demo/www/__init__.py
--rw-r--r--   0        0        0      174 2024-04-01 19:35:46.379933 vite_to_flask-0.5.0/app_flask_demo/www/templates/www/index.html
--rw-r--r--   0        0        0      194 2024-04-01 20:19:30.615319 vite_to_flask-0.5.0/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-03-13 09:34:18.030126 vite_to_flask-0.5.0/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_to_flask-0.5.0/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      262 2024-03-31 09:43:57.345376 vite_to_flask-0.5.0/app_vite_demo/index.css
--rw-r--r--   0        0        0      413 2024-03-13 08:00:10.035867 vite_to_flask-0.5.0/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-03-31 10:00:53.866729 vite_to_flask-0.5.0/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-03-31 09:46:57.981095 vite_to_flask-0.5.0/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_to_flask-0.5.0/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_to_flask-0.5.0/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_to_flask-0.5.0/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0      961 2024-04-02 13:48:05.943610 vite_to_flask-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        5 2024-04-01 21:13:09.994976 vite_to_flask-0.5.0/requirements/needed.txt
--rw-r--r--   0        0        0     1985 2024-04-03 08:22:19.275099 vite_to_flask-0.5.0/vite_to_flask/__init__.py
--rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_to_flask-0.5.0/vite_to_flask/_html_tags.py
--rw-r--r--   0        0        0     4041 2024-04-03 07:34:32.708734 vite_to_flask-0.5.0/vite_to_flask/flask_extension.py
--rw-r--r--   0        0        0     4189 2024-04-03 07:34:32.708745 vite_to_flask-0.5.0/vite_to_flask/helpers.py
--rw-r--r--   0        0        0      788 2024-04-01 20:39:57.723948 vite_to_flask-0.5.0/vite_to_flask/parser.py
--rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 vite_to_flask-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5173 2024-04-01 21:09:14.191229 vite_to_flask-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_to_flask-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2667 2024-04-02 13:53:38.931854 vite_to_flask-0.6.0/README.md
+-rw-r--r--   0        0        0      349 2024-04-02 13:51:54.853593 vite_to_flask-0.6.0/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0       69 2024-04-01 10:28:05.818282 vite_to_flask-0.6.0/app_flask_demo/extensions/__init__.py
+-rw-r--r--   0        0        0    39139 2024-04-03 07:34:09.601576 vite_to_flask-0.6.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    32826 2024-04-03 07:34:09.601913 vite_to_flask-0.6.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css
+-rw-r--r--   0        0        0    20114 2024-04-03 07:34:09.602143 vite_to_flask-0.6.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js
+-rw-r--r--   0        0        0      203 2024-04-01 19:32:58.177827 vite_to_flask-0.6.0/app_flask_demo/www/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-01 19:35:46.379933 vite_to_flask-0.6.0/app_flask_demo/www/templates/www/index.html
+-rw-r--r--   0        0        0      194 2024-04-01 20:19:30.615319 vite_to_flask-0.6.0/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-03-13 09:34:18.030126 vite_to_flask-0.6.0/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_to_flask-0.6.0/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      262 2024-03-31 09:43:57.345376 vite_to_flask-0.6.0/app_vite_demo/index.css
+-rw-r--r--   0        0        0      413 2024-03-13 08:00:10.035867 vite_to_flask-0.6.0/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-03-31 10:00:53.866729 vite_to_flask-0.6.0/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-03-31 09:46:57.981095 vite_to_flask-0.6.0/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_to_flask-0.6.0/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_to_flask-0.6.0/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_to_flask-0.6.0/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0      961 2024-04-02 13:48:05.943610 vite_to_flask-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        5 2024-04-01 21:13:09.994976 vite_to_flask-0.6.0/requirements/needed.txt
+-rw-r--r--   0        0        0     1985 2024-04-03 08:40:06.458486 vite_to_flask-0.6.0/vite_to_flask/__init__.py
+-rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_to_flask-0.6.0/vite_to_flask/_html_tags.py
+-rw-r--r--   0        0        0     4041 2024-04-03 07:34:32.708734 vite_to_flask-0.6.0/vite_to_flask/flask_extension.py
+-rw-r--r--   0        0        0     4189 2024-04-03 07:34:32.708745 vite_to_flask-0.6.0/vite_to_flask/helpers.py
+-rw-r--r--   0        0        0      902 2024-04-03 08:38:30.650239 vite_to_flask-0.6.0/vite_to_flask/parser.py
+-rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 vite_to_flask-0.6.0/PKG-INFO
```

### Comparing `vite_to_flask-0.5.0/.gitignore` & `vite_to_flask-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/LICENSE` & `vite_to_flask-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/README.md` & `vite_to_flask-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif` & `vite_to_flask-0.6.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css` & `vite_to_flask-0.6.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js` & `vite_to_flask-0.6.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/app_vite_demo/__router__.jsx` & `vite_to_flask-0.6.0/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/app_vite_demo/assets/ili.gif` & `vite_to_flask-0.6.0/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/app_vite_demo/package-lock.json` & `vite_to_flask-0.6.0/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/app_vite_demo/package.json` & `vite_to_flask-0.6.0/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/pyproject.toml` & `vite_to_flask-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/vite_to_flask/__init__.py` & `vite_to_flask-0.6.0/vite_to_flask/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from .flask_extension import ViteToFlask
 from .helpers import PyProjectConfig, _compile, Colr
 from .parser import ArgumentParser
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 __all__ = ["ViteToFlask"]
 
 
 def _cli():
     pars = ArgumentParser(prog="vtf", add_help=False)
     pars.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
```

### Comparing `vite_to_flask-0.5.0/vite_to_flask/_html_tags.py` & `vite_to_flask-0.6.0/vite_to_flask/_html_tags.py`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/vite_to_flask/flask_extension.py` & `vite_to_flask-0.6.0/vite_to_flask/flask_extension.py`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/vite_to_flask/helpers.py` & `vite_to_flask-0.6.0/vite_to_flask/helpers.py`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.5.0/vite_to_flask/parser.py` & `vite_to_flask-0.6.0/vite_to_flask/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,18 +7,20 @@
     def __init__(self, *args, **kwargs):
         super(ArgumentParser, self).__init__(*args, **kwargs)
         self.vite_apps: list[dict] = []
 
     def print_help(self, file=None):
         print(
             "\n\r"
-            "Usage: vtf <command>"
+            "Usage: vtf <option>"
             "\n\r\n\r"
-            f" {Colr.BOLD}compile{Colr.END} => Attempt to compile all vite apps"
+            f" {Colr.OKCYAN}list{Colr.END} => List all vite apps in pyproject.toml"
             "\n\r"
-            f" {Colr.BOLD}list{Colr.END} => List all vite apps in pyproject.toml"
+            f" {Colr.OKCYAN}compile (-y){Colr.END} => Attempt to compile all vite apps"
             "\n\r"
-            f" {Colr.BOLD}-h, --help{Colr.END} => Show the help message and exit"
+            f"  | {Colr.OKCYAN}-y{Colr.END} => Accept all prompts while compiling"
             "\n\r"
-            f" {Colr.BOLD}-v, --version{Colr.END} => Show the version and exit"
+            f" {Colr.OKCYAN}-h, --help{Colr.END} => Show the help message and exit"
+            "\n\r"
+            f" {Colr.OKCYAN}-v, --version{Colr.END} => Show the version and exit"
         )
         print("")
```

### Comparing `vite_to_flask-0.5.0/PKG-INFO` & `vite_to_flask-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-to-flask
-Version: 0.5.0
+Version: 0.6.0
 Summary: Transport Vite apps to Flask / Flask blueprints.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

