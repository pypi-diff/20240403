# Comparing `tmp/sphinx-ref-in-plantuml-hyperlinks-0.5.0.tar.gz` & `tmp/sphinx-ref-in-plantuml-hyperlinks-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-ref-in-plantuml-hyperlinks-0.5.0.tar", last modified: Wed Apr  3 15:57:32 2024, max compression
+gzip compressed data, was "sphinx-ref-in-plantuml-hyperlinks-0.6.0.tar", last modified: Wed Apr  3 16:09:36 2024, max compression
```

## Comparing `sphinx-ref-in-plantuml-hyperlinks-0.5.0.tar` & `sphinx-ref-in-plantuml-hyperlinks-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 radekhampl   (501) staff       (20)        0 2024-04-03 15:57:32.914061 sphinx-ref-in-plantuml-hyperlinks-0.5.0/
--rw-r--r--   0 radekhampl   (501) staff       (20)     1066 2024-03-28 19:32:35.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/LICENSE
--rw-r--r--   0 radekhampl   (501) staff       (20)       25 2024-03-30 15:31:34.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/MANIFEST.in
--rw-r--r--   0 radekhampl   (501) staff       (20)     2399 2024-04-03 15:57:32.913663 sphinx-ref-in-plantuml-hyperlinks-0.5.0/PKG-INFO
--rw-r--r--   0 radekhampl   (501) staff       (20)     1606 2024-04-02 18:52:37.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/README.md
--rw-r--r--   0 radekhampl   (501) staff       (20)       38 2024-04-03 15:57:32.914100 sphinx-ref-in-plantuml-hyperlinks-0.5.0/setup.cfg
--rw-r--r--   0 radekhampl   (501) staff       (20)     1041 2024-03-31 08:45:20.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/setup.py
-drwxr-xr-x   0 radekhampl   (501) staff       (20)        0 2024-04-03 15:57:32.909644 sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks/
--rw-r--r--   0 radekhampl   (501) staff       (20)     4023 2024-04-03 05:51:13.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks/__init__.py
-drwxr-xr-x   0 radekhampl   (501) staff       (20)        0 2024-04-03 15:57:32.913354 sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/
--rw-r--r--   0 radekhampl   (501) staff       (20)     2399 2024-04-03 15:57:32.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/PKG-INFO
--rw-r--r--   0 radekhampl   (501) staff       (20)      368 2024-04-03 15:57:32.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/SOURCES.txt
--rw-r--r--   0 radekhampl   (501) staff       (20)        1 2024-04-03 15:57:32.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/dependency_links.txt
--rw-r--r--   0 radekhampl   (501) staff       (20)       14 2024-04-03 15:57:32.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/requires.txt
--rw-r--r--   0 radekhampl   (501) staff       (20)       34 2024-04-03 15:57:32.000000 sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/top_level.txt
+drwxr-xr-x   0 radekhampl   (501) staff       (20)        0 2024-04-03 16:09:36.860450 sphinx-ref-in-plantuml-hyperlinks-0.6.0/
+-rw-r--r--   0 radekhampl   (501) staff       (20)     1066 2024-03-28 19:32:35.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/LICENSE
+-rw-r--r--   0 radekhampl   (501) staff       (20)       25 2024-03-30 15:31:34.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/MANIFEST.in
+-rw-r--r--   0 radekhampl   (501) staff       (20)     2592 2024-04-03 16:09:36.860084 sphinx-ref-in-plantuml-hyperlinks-0.6.0/PKG-INFO
+-rw-r--r--   0 radekhampl   (501) staff       (20)     1799 2024-04-03 16:05:38.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/README.md
+-rw-r--r--   0 radekhampl   (501) staff       (20)       38 2024-04-03 16:09:36.860505 sphinx-ref-in-plantuml-hyperlinks-0.6.0/setup.cfg
+-rw-r--r--   0 radekhampl   (501) staff       (20)     1041 2024-04-03 16:06:54.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/setup.py
+drwxr-xr-x   0 radekhampl   (501) staff       (20)        0 2024-04-03 16:09:36.856628 sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks/
+-rw-r--r--   0 radekhampl   (501) staff       (20)     4023 2024-04-03 16:07:07.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks/__init__.py
+drwxr-xr-x   0 radekhampl   (501) staff       (20)        0 2024-04-03 16:09:36.859752 sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/
+-rw-r--r--   0 radekhampl   (501) staff       (20)     2592 2024-04-03 16:09:36.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/PKG-INFO
+-rw-r--r--   0 radekhampl   (501) staff       (20)      368 2024-04-03 16:09:36.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/SOURCES.txt
+-rw-r--r--   0 radekhampl   (501) staff       (20)        1 2024-04-03 16:09:36.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/dependency_links.txt
+-rw-r--r--   0 radekhampl   (501) staff       (20)       14 2024-04-03 16:09:36.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/requires.txt
+-rw-r--r--   0 radekhampl   (501) staff       (20)       34 2024-04-03 16:09:36.000000 sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/top_level.txt
```

### Comparing `sphinx-ref-in-plantuml-hyperlinks-0.5.0/LICENSE` & `sphinx-ref-in-plantuml-hyperlinks-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-ref-in-plantuml-hyperlinks-0.5.0/PKG-INFO` & `sphinx-ref-in-plantuml-hyperlinks-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-ref-in-plantuml-hyperlinks
-Version: 0.5.0
+Version: 0.6.0
 Summary: sphinx-ref-in-plantuml-hyperlinks is a Sphinx extension to resolve std:ref-s defined in plantuml files
 Home-page: https://github.com/mi-parkes/sphinx-ref-in-plantuml-hyperlinks
 Author: Michael Parkes
 Author-email: mparkes@post.cz
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -35,15 +35,23 @@
     
         *[#Orange] Example of clickable references
         **[#lightgreen] [[ ":ref:`plantuml label1`" Internal Page Reference1 ]]
         **[#lightblue] [[ ":ref:`N_00001`" Internal Page Reference2 on Sphinx-Needs ]]
 
         @endmindmap
 
-## Installation (Linux)
+## Installation
+
+You can install [sphinx-ref-in-plantuml-hyperlinks](https://pypi.org/project/sphinx-ref-in-plantuml-hyperlinks/) with pip
+
+```
+pip install sphinx-ref-in-plantuml-hyperlinks
+```
+
+Alternatively (Linux)
 
     git clone https://github.com/mi-parkes/sphinx-ref-in-plantuml-hyperlinks.git
     cd sphinx-ref-in-plantuml-hyperlinks
 
     python3 -m venv .venv
     source .venv/bin/activate
     pip install -r doc/requirements.txt
```

### Comparing `sphinx-ref-in-plantuml-hyperlinks-0.5.0/README.md` & `sphinx-ref-in-plantuml-hyperlinks-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,23 @@
     
         *[#Orange] Example of clickable references
         **[#lightgreen] [[ ":ref:`plantuml label1`" Internal Page Reference1 ]]
         **[#lightblue] [[ ":ref:`N_00001`" Internal Page Reference2 on Sphinx-Needs ]]
 
         @endmindmap
 
-## Installation (Linux)
+## Installation
+
+You can install [sphinx-ref-in-plantuml-hyperlinks](https://pypi.org/project/sphinx-ref-in-plantuml-hyperlinks/) with pip
+
+```
+pip install sphinx-ref-in-plantuml-hyperlinks
+```
+
+Alternatively (Linux)
 
     git clone https://github.com/mi-parkes/sphinx-ref-in-plantuml-hyperlinks.git
     cd sphinx-ref-in-plantuml-hyperlinks
 
     python3 -m venv .venv
     source .venv/bin/activate
     pip install -r doc/requirements.txt
```

### Comparing `sphinx-ref-in-plantuml-hyperlinks-0.5.0/setup.py` & `sphinx-ref-in-plantuml-hyperlinks-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sphinx-ref-in-plantuml-hyperlinks',
-    version='0.5.0',
+    version='0.6.0',
     packages=['sphinx_ref_in_plantuml_hyperlinks'],
     py_modules=[],
     author='Michael Parkes',
     author_email='mparkes@post.cz',
     description='sphinx-ref-in-plantuml-hyperlinks is a Sphinx extension to resolve std:ref-s defined in plantuml files',
     url='https://github.com/mi-parkes/sphinx-ref-in-plantuml-hyperlinks',
     license="MIT License",
```

### Comparing `sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks/__init__.py` & `sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import re
 import xml.etree.ElementTree as ET
 from sphinx.events import EventListener
 from sphinx_needs.needsfile import NeedsList
 
 logger = sphinx.util.logging.getLogger(__name__)
 
-__version__ = "0.5.0"
-version_info = (0,5,0)
+__version__ = "0.6.0"
+version_info = (0,6,0)
 
 def init_needs(app):
     needs_list = NeedsList(app.env.config,app.outdir,app.srcdir)
     needs_list.load_json(os.path.join(app.builder.outdir,"needs.json"))
     if needs_list and needs_list.needs_list:
         if "versions" in needs_list.needs_list:
             keys=list(needs_list.needs_list["versions"].keys())
```

### Comparing `sphinx-ref-in-plantuml-hyperlinks-0.5.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/PKG-INFO` & `sphinx-ref-in-plantuml-hyperlinks-0.6.0/sphinx_ref_in_plantuml_hyperlinks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-ref-in-plantuml-hyperlinks
-Version: 0.5.0
+Version: 0.6.0
 Summary: sphinx-ref-in-plantuml-hyperlinks is a Sphinx extension to resolve std:ref-s defined in plantuml files
 Home-page: https://github.com/mi-parkes/sphinx-ref-in-plantuml-hyperlinks
 Author: Michael Parkes
 Author-email: mparkes@post.cz
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -35,15 +35,23 @@
     
         *[#Orange] Example of clickable references
         **[#lightgreen] [[ ":ref:`plantuml label1`" Internal Page Reference1 ]]
         **[#lightblue] [[ ":ref:`N_00001`" Internal Page Reference2 on Sphinx-Needs ]]
 
         @endmindmap
 
-## Installation (Linux)
+## Installation
+
+You can install [sphinx-ref-in-plantuml-hyperlinks](https://pypi.org/project/sphinx-ref-in-plantuml-hyperlinks/) with pip
+
+```
+pip install sphinx-ref-in-plantuml-hyperlinks
+```
+
+Alternatively (Linux)
 
     git clone https://github.com/mi-parkes/sphinx-ref-in-plantuml-hyperlinks.git
     cd sphinx-ref-in-plantuml-hyperlinks
 
     python3 -m venv .venv
     source .venv/bin/activate
     pip install -r doc/requirements.txt
```

