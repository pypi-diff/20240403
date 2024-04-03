# Comparing `tmp/vite_to_flask-0.3.0.tar.gz` & `tmp/vite_to_flask-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_to_flask-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_to_flask-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_to_flask-0.3.0.tar` & `vite_to_flask-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     5173 2024-04-01 21:09:14.191229 vite_to_flask-0.3.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_to_flask-0.3.0/LICENSE
--rw-r--r--   0        0        0     2667 2024-04-02 13:53:38.931854 vite_to_flask-0.3.0/README.md
--rw-r--r--   0        0        0      349 2024-04-02 13:51:54.853593 vite_to_flask-0.3.0/app_flask_demo/__init__.py
--rw-r--r--   0        0        0       69 2024-04-01 10:28:05.818282 vite_to_flask-0.3.0/app_flask_demo/extensions/__init__.py
--rw-r--r--   0        0        0    39139 2024-04-01 20:19:37.795932 vite_to_flask-0.3.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    32826 2024-04-01 20:19:37.796632 vite_to_flask-0.3.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css
--rw-r--r--   0        0        0    20114 2024-04-01 20:19:37.797165 vite_to_flask-0.3.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js
--rw-r--r--   0        0        0      203 2024-04-01 19:32:58.177827 vite_to_flask-0.3.0/app_flask_demo/www/__init__.py
--rw-r--r--   0        0        0      174 2024-04-01 19:35:46.379933 vite_to_flask-0.3.0/app_flask_demo/www/templates/www/index.html
--rw-r--r--   0        0        0      194 2024-04-01 20:19:30.615319 vite_to_flask-0.3.0/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-03-13 09:34:18.030126 vite_to_flask-0.3.0/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_to_flask-0.3.0/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      262 2024-03-31 09:43:57.345376 vite_to_flask-0.3.0/app_vite_demo/index.css
--rw-r--r--   0        0        0      413 2024-03-13 08:00:10.035867 vite_to_flask-0.3.0/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-03-31 10:00:53.866729 vite_to_flask-0.3.0/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-03-31 09:46:57.981095 vite_to_flask-0.3.0/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_to_flask-0.3.0/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_to_flask-0.3.0/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_to_flask-0.3.0/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0      961 2024-04-02 13:48:05.943610 vite_to_flask-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        5 2024-04-01 21:13:09.994976 vite_to_flask-0.3.0/requirements/needed.txt
--rw-r--r--   0        0        0     1741 2024-04-02 13:53:53.811624 vite_to_flask-0.3.0/vite_to_flask/__init__.py
--rw-r--r--   0        0        0     4943 2024-04-01 19:39:45.691324 vite_to_flask-0.3.0/vite_to_flask/_html_tags.py
--rw-r--r--   0        0        0     4025 2024-04-02 13:50:42.466088 vite_to_flask-0.3.0/vite_to_flask/flask_extension.py
--rw-r--r--   0        0        0     3703 2024-04-01 20:17:48.087356 vite_to_flask-0.3.0/vite_to_flask/helpers.py
--rw-r--r--   0        0        0      788 2024-04-01 20:39:57.723948 vite_to_flask-0.3.0/vite_to_flask/parser.py
--rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 vite_to_flask-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5173 2024-04-01 21:09:14.191229 vite_to_flask-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_to_flask-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2667 2024-04-02 13:53:38.931854 vite_to_flask-0.4.0/README.md
+-rw-r--r--   0        0        0      349 2024-04-02 13:51:54.853593 vite_to_flask-0.4.0/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0       69 2024-04-01 10:28:05.818282 vite_to_flask-0.4.0/app_flask_demo/extensions/__init__.py
+-rw-r--r--   0        0        0    39139 2024-04-03 07:34:09.601576 vite_to_flask-0.4.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    32826 2024-04-03 07:34:09.601913 vite_to_flask-0.4.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css
+-rw-r--r--   0        0        0    20114 2024-04-03 07:34:09.602143 vite_to_flask-0.4.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js
+-rw-r--r--   0        0        0      203 2024-04-01 19:32:58.177827 vite_to_flask-0.4.0/app_flask_demo/www/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-01 19:35:46.379933 vite_to_flask-0.4.0/app_flask_demo/www/templates/www/index.html
+-rw-r--r--   0        0        0      194 2024-04-01 20:19:30.615319 vite_to_flask-0.4.0/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-03-13 09:34:18.030126 vite_to_flask-0.4.0/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_to_flask-0.4.0/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      262 2024-03-31 09:43:57.345376 vite_to_flask-0.4.0/app_vite_demo/index.css
+-rw-r--r--   0        0        0      413 2024-03-13 08:00:10.035867 vite_to_flask-0.4.0/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-03-31 10:00:53.866729 vite_to_flask-0.4.0/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-03-31 09:46:57.981095 vite_to_flask-0.4.0/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_to_flask-0.4.0/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_to_flask-0.4.0/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_to_flask-0.4.0/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0      961 2024-04-02 13:48:05.943610 vite_to_flask-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        5 2024-04-01 21:13:09.994976 vite_to_flask-0.4.0/requirements/needed.txt
+-rw-r--r--   0        0        0     2005 2024-04-03 07:36:12.516779 vite_to_flask-0.4.0/vite_to_flask/__init__.py
+-rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_to_flask-0.4.0/vite_to_flask/_html_tags.py
+-rw-r--r--   0        0        0     4041 2024-04-03 07:34:32.708734 vite_to_flask-0.4.0/vite_to_flask/flask_extension.py
+-rw-r--r--   0        0        0     4189 2024-04-03 07:34:32.708745 vite_to_flask-0.4.0/vite_to_flask/helpers.py
+-rw-r--r--   0        0        0      788 2024-04-01 20:39:57.723948 vite_to_flask-0.4.0/vite_to_flask/parser.py
+-rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 vite_to_flask-0.4.0/PKG-INFO
```

### Comparing `vite_to_flask-0.3.0/.gitignore` & `vite_to_flask-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/LICENSE` & `vite_to_flask-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/README.md` & `vite_to_flask-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif` & `vite_to_flask-0.4.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css` & `vite_to_flask-0.4.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js` & `vite_to_flask-0.4.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/app_vite_demo/__router__.jsx` & `vite_to_flask-0.4.0/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/app_vite_demo/assets/ili.gif` & `vite_to_flask-0.4.0/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/app_vite_demo/package-lock.json` & `vite_to_flask-0.4.0/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/app_vite_demo/package.json` & `vite_to_flask-0.4.0/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/pyproject.toml` & `vite_to_flask-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/vite_to_flask/__init__.py` & `vite_to_flask-0.4.0/vite_to_flask/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import sys
 
 from .flask_extension import ViteToFlask
 from .helpers import PyProjectConfig, _compile, Colr
 from .parser import ArgumentParser
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __all__ = ["ViteToFlask"]
 
 
 def _cli():
     pars = ArgumentParser(prog="vtf", add_help=False)
     pars.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
     )
     pars.add_argument("--help", "-h", action="help")
 
     subparsers = pars.add_subparsers()
 
     compile_parser = subparsers.add_parser("compile")
     compile_parser.set_defaults(compile=False)
+    compile_parser.add_argument("-y", action="store_true")
 
     list_parser = subparsers.add_parser("list")
     list_parser.set_defaults(list=False)
 
     with PyProjectConfig() as pyproject:
         for vite_app in pyproject.vite_apps:
             pars.vite_apps.append(
@@ -30,29 +31,36 @@
                     "vite_app": vite_app,
                     "flask_app_dir": pyproject.vtf_config.get("flask_app_dir"),
                 }
             )
 
         args = pars.parse_args()
 
+        print(args)
         if hasattr(args, "compile"):
-            _compile(pyproject, pars.vite_apps)
+            _compile(
+                pyproject,
+                pars.vite_apps,
+                replace=True if hasattr(args, "y") and args.y else False,
+            )
+
+            # exit after compiling
             sys.exit(0)
 
         if hasattr(args, "list"):
-            print(
-                "\n\r"
-                "Vite apps in pyproject.toml:"
-            )
+            print("\n\r" "Vite apps in pyproject.toml:")
             if not pars.vite_apps:
                 print(f" {Colr.WARNING}No vite apps found in pyproject.toml{Colr.END}")
             else:
                 for app in pars.vite_apps:
                     print(
                         f" {Colr.OKCYAN}{app.get('vite_app')}{Colr.END} "
                         f"{Colr.BOLD}=>{Colr.END} "
                         f"{app.get('flask_app_dir')}/vtf/{app.get('vite_app')}/"
                     )
             print("")
+
+            # exit after listing
             sys.exit(0)
 
+    # print help if no command is given
     pars.print_help()
```

### Comparing `vite_to_flask-0.3.0/vite_to_flask/_html_tags.py` & `vite_to_flask-0.4.0/vite_to_flask/_html_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     _rel: str = None
     _href: str = None
     _sizes: str = None
     _type: str = None
     _hreflang: str = None
 
     def __init__(
-            self,
-            rel: str,
-            href: Optional[str] = None,
-            sizes: Optional[str] = None,
-            type_: Optional[str] = None,
-            hreflang: Optional[str] = None,
+        self,
+        rel: str,
+        href: Optional[str] = None,
+        sizes: Optional[str] = None,
+        type_: Optional[str] = None,
+        hreflang: Optional[str] = None,
     ):
         self.rel = rel
         self.href = href
         self.sizes = sizes
         self.type = type_
         self.hreflang = hreflang
 
@@ -76,23 +76,23 @@
     _defer: str = None
     _crossorigin: str = None
     _integrity: str = None
     _nomodule: str = None
     _referrerpolicy: str = None
 
     def __init__(
-            self,
-            src: str,
-            type_: Optional[str] = None,
-            async_: bool = False,
-            defer: bool = False,
-            crossorigin: Optional[str] = None,
-            integrity: Optional[str] = None,
-            nomodule: bool = False,
-            referrerpolicy: Optional[str] = None,
+        self,
+        src: str,
+        type_: Optional[str] = None,
+        async_: bool = False,
+        defer: bool = False,
+        crossorigin: Optional[str] = None,
+        integrity: Optional[str] = None,
+        nomodule: bool = False,
+        referrerpolicy: Optional[str] = None,
     ):
         self.src = src
         self.type = type_
         self.async_ = async_
         self.defer = defer
         self.crossorigin = crossorigin
         self.integrity = integrity
@@ -143,17 +143,17 @@
 
 
 class BodyContent:
     div_id: str = None
     noscript_message: str = None
 
     def __init__(
-            self,
-            div_id: str = "root",
-            noscript_message: str = "You need to enable JavaScript to run this app.",
+        self,
+        div_id: str = "root",
+        noscript_message: str = "You need to enable JavaScript to run this app.",
     ):
         self.div_id = div_id
         self.noscript_message = noscript_message
 
     def __repr__(self):
         return (
             "BodyContent< "
```

### Comparing `vite_to_flask-0.3.0/vite_to_flask/flask_extension.py` & `vite_to_flask-0.4.0/vite_to_flask/flask_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,28 +85,30 @@
                 return Markup("".join([tag.raw() for tag in tags]))
 
             return dict(vtf_head=vtf_head)
 
         @app.context_processor
         def vtf_body_processor():
             def vtf_body(
-                    root_id: str = "root",
-                    noscript_message: str = "You need to enable JavaScript to run this app.",
+                root_id: str = "root",
+                noscript_message: str = "You need to enable JavaScript to run this app.",
             ) -> t.Any:
                 return BodyContent(root_id, noscript_message)()
 
             return dict(vtf_body=vtf_body)
 
     @staticmethod
     def _load_cors_headers(app: Flask) -> None:
-        if app.debug and not app.config.get('VTF_DISABLE_DEBUG_CORS', False):
-            print(f"{Colr.OKCYAN}{Colr.BOLD}vite-to-flask: Flask debug mode detected"
-                  f"{Colr.END}{Colr.END}\n\r"
-                  f"{Colr.OKCYAN}Allow all CORS headers will be added to "
-                  f"every response to allow for frontend development.{Colr.END}")
+        if app.debug and not app.config.get("VTF_DISABLE_DEBUG_CORS", False):
+            print(
+                f"{Colr.OKCYAN}{Colr.BOLD}vite-to-flask: Flask debug mode detected"
+                f"{Colr.END}{Colr.END}\n\r"
+                f"{Colr.OKCYAN}Allow all CORS headers will be added to "
+                f"every response to allow for frontend development.{Colr.END}"
+            )
 
             @app.after_request
             def after_request(response):
                 response.headers["Access-Control-Allow-Origin"] = "*"
                 response.headers["Access-Control-Allow-Headers"] = "*"
                 response.headers["Access-Control-Allow-Methods"] = "*"
                 return response
```

### Comparing `vite_to_flask-0.3.0/vite_to_flask/helpers.py` & `vite_to_flask-0.4.0/vite_to_flask/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import shlex
 import shutil
 import subprocess
+import sys
 from pathlib import Path
 from tomllib import loads
 
 
 class Colr:
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
@@ -83,25 +84,42 @@
         return None
 
     def run(self, command: str):
         subprocess.run([self.npx_binary, *shlex.split(command)], cwd=self.workdir)
         pass
 
 
-def _compile(pypro: PyProjectConfig, vite_apps: list[dict]):
+def _compile(pypro: PyProjectConfig, vite_apps: list[dict], replace: bool = False):
     print("Compiling Vite apps...")
     flask_vtf_dir = pypro.cwd / pypro.flask_app_dir / "vtf"
 
     # Delete contents of vtf_dir
     if flask_vtf_dir.exists():
-        for item in flask_vtf_dir.iterdir():
-            if item.is_dir():
-                shutil.rmtree(item)
-            else:
-                item.unlink()
+        if not replace:
+            prompt = input(
+                f"Continuing will replace the contents of \n\r"
+                f"{flask_vtf_dir} \n\r"
+                f"Do you want to continue? (Y/n): "
+            )
+        else:
+            prompt = "y"
+
+        if prompt.lower() == "y" or prompt == "":
+            for item in flask_vtf_dir.iterdir():
+                if item.is_dir():
+                    shutil.rmtree(item)
+                else:
+                    item.unlink()
+
+        else:
+            print("Operation aborted.")
+            sys.exit(0)
+
+    else:
+        flask_vtf_dir.mkdir()
 
     # Create directories for vite apps
     for app in vite_apps:
         flask_vtf_app_dir = flask_vtf_dir / app.get("vite_app")
         this_vite_app_path = pypro.cwd / app.get("vite_app")
         this_vite_app_dist = this_vite_app_path / "dist"
         this_vite_app_dist_assets = this_vite_app_dist / "assets"
```

### Comparing `vite_to_flask-0.3.0/vite_to_flask/parser.py` & `vite_to_flask-0.4.0/vite_to_flask/parser.py`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.3.0/PKG-INFO` & `vite_to_flask-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-to-flask
-Version: 0.3.0
+Version: 0.4.0
 Summary: Transport Vite apps to Flask / Flask blueprints.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

