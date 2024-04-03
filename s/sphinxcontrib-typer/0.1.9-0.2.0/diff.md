# Comparing `tmp/sphinxcontrib_typer-0.1.9.tar.gz` & `tmp/sphinxcontrib_typer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_typer-0.1.9.tar", max compression
+gzip compressed data, was "sphinxcontrib_typer-0.2.0.tar", max compression
```

## Comparing `sphinxcontrib_typer-0.1.9.tar` & `sphinxcontrib_typer-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-12-14 00:10:27.893967 sphinxcontrib_typer-0.1.9/LICENSE
--rw-r--r--   0        0        0     5672 2023-12-29 18:54:23.227545 sphinxcontrib_typer-0.1.9/README.rst
--rw-r--r--   0        0        0     2928 2024-02-22 07:20:51.993977 sphinxcontrib_typer-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    34484 2024-02-22 07:20:45.089245 sphinxcontrib_typer-0.1.9/sphinxcontrib/typer/__init__.py
--rw-r--r--   0        0        0     7249 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-03 19:52:41.798588 sphinxcontrib_typer-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5672 2024-04-03 19:52:41.799025 sphinxcontrib_typer-0.2.0/README.rst
+-rw-r--r--   0        0        0     3120 2024-04-03 19:53:19.565537 sphinxcontrib_typer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    34776 2024-04-03 20:18:25.421226 sphinxcontrib_typer-0.2.0/sphinxcontrib/typer/__init__.py
+-rw-r--r--   0        0        0     7304 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.0/PKG-INFO
```

### Comparing `sphinxcontrib_typer-0.1.9/LICENSE` & `sphinxcontrib_typer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.1.9/README.rst` & `sphinxcontrib_typer-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.1.9/sphinxcontrib/typer/__init__.py` & `sphinxcontrib_typer-0.2.0/sphinxcontrib/typer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,20 +38,21 @@
 from docutils.parsers import rst
 from docutils.parsers.rst import directives
 from rich import terminal_theme as rich_theme
 from rich.console import Console
 from rich.theme import Theme
 from sphinx import application
 from sphinx.util import logging
+
 from typer import rich_utils as typer_rich_utils
 from typer.main import Typer, TyperGroup
 from typer.main import get_command as get_typer_command
 from typer.models import Context as TyperContext
 
-VERSION = (0, 1, 9)
+VERSION = (0, 2, 0)
 
 __title__ = 'SphinxContrib Typer'
 __version__ = '.'.join(str(i) for i in VERSION)
 __author__ = 'Brian Kohan'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Brian Kohan'
 
@@ -919,32 +920,42 @@
             im.save(str(png_path))  # Saves the screenshot
 
 
 def setup(app: application.Sphinx) -> t.Dict[str, t.Any]:
     # Need autodoc to support mocking modules
     app.add_directive('typer', TyperDirective)
 
+    def get_default_render_html(_):
+        return typer_render_html
+
+    def get_default_get_iframe_height(_):
+        return typer_get_iframe_height
+
+    def get_default_svg2pdf(_):
+        return typer_svg2pdf
+
+    def get_default_convert_png(_):
+        return typer_convert_png
+
+    def get_default_web_driver(_):
+        return typer_get_web_driver
+
+    app.add_config_value('typer_render_html', get_default_render_html, 'env')
+
     app.add_config_value(
-        'typer_render_html', lambda _: typer_render_html, 'env'
-    )
-    app.add_config_value(
-        'typer_get_iframe_height', lambda _: typer_get_iframe_height, 'env'
+        'typer_get_iframe_height', get_default_get_iframe_height, 'env'
     )
-    app.add_config_value('typer_svg2pdf', lambda _: typer_svg2pdf, 'env')
+    app.add_config_value('typer_svg2pdf', get_default_svg2pdf, 'env')
     app.add_config_value('typer_iframe_height_padding', 30, 'env')
     app.add_config_value(
         'typer_iframe_height_cache_path',
         Path(app.confdir) / 'typer_cache.json',
         'env',
     )
 
-    app.add_config_value(
-        'typer_convert_png', lambda _: typer_convert_png, 'env'
-    )
-    app.add_config_value(
-        'typer_get_web_driver', lambda _: typer_get_web_driver, 'env'
-    )
+    app.add_config_value('typer_convert_png', get_default_convert_png, 'env')
+    app.add_config_value('typer_get_web_driver', get_default_web_driver, 'env')
 
     return {
         'parallel_read_safe': True,
         'parallel_write_safe': True,
     }
```

### Comparing `sphinxcontrib_typer-0.1.9/PKG-INFO` & `sphinxcontrib_typer-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-typer
-Version: 0.1.9
+Version: 0.2.0
 Summary: Auto generate docs for typer commands.
 Home-page: https://sphinxcontrib-typer.readthedocs.io
 License: MIT
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,17 +25,18 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: html
 Provides-Extra: pdf
 Provides-Extra: png
 Requires-Dist: cairosvg (>=2.4.0,<3.0.0) ; extra == "pdf"
 Requires-Dist: lxml (>=4.2.0,<6.0.0) ; extra == "pdf"
+Requires-Dist: pillow (>=8.0.0) ; extra == "png"
 Requires-Dist: selenium (>=4.0.0,<5.0.0) ; extra == "html" or extra == "png"
 Requires-Dist: sphinx (>=4.0.0)
-Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
+Requires-Dist: typer-slim[all] (>=0.12.0,<1.0.0)
 Requires-Dist: webdriver-manager (>=3.0.0,<5.0.0) ; extra == "html" or extra == "png"
 Project-URL: Repository, https://github.com/sphinx-contrib/typer
 Description-Content-Type: text/x-rst
 
 |MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPI status| |Documentation Status|
 |Code Cov| |Test Status|
```

