# Comparing `tmp/xyzstyle-0.0.6.tar.gz` & `tmp/xyzstyle-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyzstyle-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xyzstyle-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xyzstyle-0.0.6.tar` & `xyzstyle-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-03-06 05:54:40.735867 xyzstyle-0.0.6/LICENSE
--rw-r--r--   0        0        0     2208 2024-03-06 05:54:40.735867 xyzstyle-0.0.6/README.md
--rw-r--r--   0        0        0     1485 2024-03-06 05:54:40.739867 xyzstyle-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1052 2024-03-06 05:54:40.739867 xyzstyle-0.0.6/src/xyzstyle/__init__.py
--rw-r--r--   0        0        0      244 2024-03-06 05:54:40.739867 xyzstyle-0.0.6/src/xyzstyle/themes/xyzstyle/layout.html
--rw-r--r--   0        0        0      306 2024-03-06 05:54:40.739867 xyzstyle-0.0.6/src/xyzstyle/themes/xyzstyle/theme.conf
--rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 xyzstyle-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 13:14:22.145236 xyzstyle-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2208 2024-04-03 13:14:22.145236 xyzstyle-0.0.7/README.md
+-rw-r--r--   0        0        0     1538 2024-04-03 13:14:22.145236 xyzstyle-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1052 2024-04-03 13:14:22.149236 xyzstyle-0.0.7/src/xyzstyle/__init__.py
+-rw-r--r--   0        0        0      242 2024-04-03 13:14:22.149236 xyzstyle-0.0.7/src/xyzstyle/themes/xyzstyle/layout.html
+-rw-r--r--   0        0        0      199 2024-04-03 13:14:22.149236 xyzstyle-0.0.7/src/xyzstyle/themes/xyzstyle/theme.conf
+-rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 xyzstyle-0.0.7/PKG-INFO
```

### Comparing `xyzstyle-0.0.6/LICENSE` & `xyzstyle-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xyzstyle-0.0.6/README.md` & `xyzstyle-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `xyzstyle-0.0.6/pyproject.toml` & `xyzstyle-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 license = {file = "LICENSE"}
 name = "xyzstyle"
 readme = "README.md"
 requires-python = ">=3.8"
 
 dependencies = [
   "d2py",
-  "pydata-sphinx-theme>=0.7.2"
+  "sphinx_book_theme"
 ]
 
 maintainers = [
   {name = "xinetzone", email = "735613050@qq.com"},
 ]
 
 classifiers = [
@@ -30,28 +30,31 @@
 
 [project.urls]
 Home = "https://github.com/xinetzone/xyzstyle"
 
 [project.optional-dependencies]
 doc = [
   "myst-nb",
+  "sphinx==7.2.5",
   "sphinxext-rediraffe",
   "sphinx-copybutton",
   "sphinx_design",
   'jupyterlite-sphinx',
   "jupyterlite-xeus",
   "jupyterlite-core",
   "jupyterlite-pyodide-kernel",
   "jupyterlab",
   "jupyter_server",
   "jupyterlab_server",
   "sphinx-autoapi",
   "linkify-it-py",
-  "jupyter-sphinx",
+  # "jupyter-sphinx",
   "sphinx-sitemap",
+  "sphinxcontrib-katex",
+  "sphinx-thebe",
 ]
 
 coverage = [
   "pytest-cov",
   "pytest-regressions",
   "codecov",
   "xyzstyle[test]",
@@ -70,9 +73,9 @@
   "xyzstyle[doc]"
 ]
 
 [project.entry-points]
 "sphinx.html_themes" = {xyzstyle = "xyzstyle"}
 
 [tool.flit.sdist]
-# include = ["docs/"]
-exclude = ['docs', '.git', '.github']
+# include = ["doc/"]
+exclude = ['doc', '.git', '.github']
```

### Comparing `xyzstyle-0.0.6/src/xyzstyle/__init__.py` & `xyzstyle-0.0.7/src/xyzstyle/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 import sys
 
 if sys.platform == 'win32':
     import asyncio
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 __version_full__ = __version__
 
 
 def get_html_theme_path():
     """
     Return path to Sphinx templates folder.
     """
```

### Comparing `xyzstyle-0.0.6/PKG-INFO` & `xyzstyle-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: xyzstyle
-Version: 0.0.6
+Version: 0.0.7
 Summary: Sphinx demo.
 Author-email: xinetzone <735613050@qq.com>
 Maintainer-email: xinetzone <735613050@qq.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Dist: d2py
-Requires-Dist: pydata-sphinx-theme>=0.7.2
+Requires-Dist: sphinx_book_theme
 Requires-Dist: pytest-cov ; extra == "coverage"
 Requires-Dist: pytest-regressions ; extra == "coverage"
 Requires-Dist: codecov ; extra == "coverage"
 Requires-Dist: xyzstyle[test] ; extra == "coverage"
 Requires-Dist: pyyaml ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: xyzstyle[coverage] ; extra == "dev"
 Requires-Dist: myst-nb ; extra == "doc"
+Requires-Dist: sphinx==7.2.5 ; extra == "doc"
 Requires-Dist: sphinxext-rediraffe ; extra == "doc"
 Requires-Dist: sphinx-copybutton ; extra == "doc"
 Requires-Dist: sphinx_design ; extra == "doc"
 Requires-Dist: jupyterlite-sphinx ; extra == "doc"
 Requires-Dist: jupyterlite-xeus ; extra == "doc"
 Requires-Dist: jupyterlite-core ; extra == "doc"
 Requires-Dist: jupyterlite-pyodide-kernel ; extra == "doc"
 Requires-Dist: jupyterlab ; extra == "doc"
 Requires-Dist: jupyter_server ; extra == "doc"
 Requires-Dist: jupyterlab_server ; extra == "doc"
 Requires-Dist: sphinx-autoapi ; extra == "doc"
 Requires-Dist: linkify-it-py ; extra == "doc"
-Requires-Dist: jupyter-sphinx ; extra == "doc"
 Requires-Dist: sphinx-sitemap ; extra == "doc"
+Requires-Dist: sphinxcontrib-katex ; extra == "doc"
+Requires-Dist: sphinx-thebe ; extra == "doc"
 Requires-Dist: python-docx ; extra == "docx"
 Requires-Dist: xyzstyle[doc] ; extra == "docx"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: xyzstyle[doc] ; extra == "test"
 Project-URL: Home, https://github.com/xinetzone/xyzstyle
 Provides-Extra: coverage
 Provides-Extra: dev
```

