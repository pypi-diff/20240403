# Comparing `tmp/galaxy-tours-23.2.1.tar.gz` & `tmp/galaxy-tours-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tours/dist/.tmp-o7di88f7/galaxy-tours-23.2.1.tar", last modified: Thu Feb 22 03:54:28 2024, max compression
+gzip compressed data, was "galaxy-tours-24.0.0.tar", last modified: Wed Apr  3 02:45:32 2024, max compression
```

## Comparing `galaxy-tours-23.2.1.tar` & `galaxy-tours-24.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy/tours/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/galaxy/tours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/galaxy/tours/_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/galaxy/tours/_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/galaxy/tours/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/galaxy/tours/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy_tours.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy_tours.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy_tours.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy_tours.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy_tours.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy_tours.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/galaxy_tours.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-22 03:54:28.000000 galaxy-tours-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-tours-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:32.043313 galaxy-tours-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-03 02:45:32.043313 galaxy-tours-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:32.039313 galaxy-tours-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:32.043313 galaxy-tours-24.0.0/galaxy/tours/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/galaxy/tours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/galaxy/tours/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/galaxy/tours/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/galaxy/tours/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/galaxy/tours/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:32.043313 galaxy-tours-24.0.0/galaxy_tours.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-03 02:45:32.000000 galaxy-tours-24.0.0/galaxy_tours.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-03 02:45:32.000000 galaxy-tours-24.0.0/galaxy_tours.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:32.000000 galaxy-tours-24.0.0/galaxy_tours.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:45:32.000000 galaxy-tours-24.0.0/galaxy_tours.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 02:45:32.000000 galaxy-tours-24.0.0/galaxy_tours.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:32.000000 galaxy-tours-24.0.0/galaxy_tours.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-03 02:45:32.043313 galaxy-tours-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-tours-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-tours-23.2.1/LICENSE.txt` & `galaxy-tours-24.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.2.1/PKG-INFO` & `galaxy-tours-24.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: galaxy-tours
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy tours backend framework
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
+Requires-Dist: galaxy-navigation
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: PyYAML
 
 
 .. image:: https://badge.fury.io/py/galaxy-tours.svg
    :target: https://pypi.org/project/galaxy-tours/
 
 
 Overview
@@ -44,14 +47,26 @@
 
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
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.1.4 (2024-01-04)
```

### Comparing `galaxy-tours-23.2.1/galaxy/tours/_impl.py` & `galaxy-tours-24.0.0/galaxy/tours/_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module manages loading/etc of Galaxy interactive tours.
 """
+
 import logging
 import os
 from typing import (
     List,
     Union,
 )
```

### Comparing `galaxy-tours-23.2.1/galaxy/tours/_schema.py` & `galaxy-tours-24.0.0/galaxy/tours/_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
     List,
     Optional,
     Union,
 )
 
 from pydantic import (
     BaseModel,
+    ConfigDict,
     Field,
+    RootModel,
 )
 
 
 class Requirement(str, Enum):
     """Available types of job sources (model classes) that produce dataset collections."""
 
     LOGGED_IN = "logged_in"
@@ -20,41 +22,41 @@
 
 
 class TourCore(BaseModel):
     name: str = Field(title="Name", description="Name of tour")
     description: str = Field(title="Description", description="Tour description")
     tags: List[str] = Field(title="Tags", description="Topic topic tags")
     requirements: List[Requirement] = Field(title="Requirements", description="Requirements to run the tour.")
-
-    class Config:
-        use_enum_values = True  # when using .dict()
+    model_config = ConfigDict(use_enum_values=True)
 
 
 class Tour(TourCore):
     id: str = Field(title="Identifier", description="Tour identifier")
 
 
-class TourList(BaseModel):
-    __root__: List[Tour] = Field(title="List of tours", default=[])
+class TourList(RootModel):
+    root: List[Tour] = Field(title="List of tours", default=[])
 
 
 class TourStep(BaseModel):
-    title: Optional[str] = Field(title="Title", description="Title displayed in the header of the step container")
-    content: Optional[str] = Field(title="Content", description="Text shown to the user")
-    element: Optional[str] = Field(title="Element", description="CSS selector for the element to be described/clicked")
+    title: Optional[str] = Field(None, title="Title", description="Title displayed in the header of the step container")
+    content: Optional[str] = Field(None, title="Content", description="Text shown to the user")
+    element: Optional[str] = Field(
+        None, title="Element", description="CSS selector for the element to be described/clicked"
+    )
     placement: Optional[str] = Field(
-        title="Placement", description="Placement of the text box relative to the selected element"
+        None, title="Placement", description="Placement of the text box relative to the selected element"
     )
     preclick: Optional[Union[bool, List[str]]] = Field(
-        title="Pre-click", description="Elements that receive a click() event before the step is shown"
+        None, title="Pre-click", description="Elements that receive a click() event before the step is shown"
     )
     postclick: Optional[Union[bool, List[str]]] = Field(
-        title="Post-click", description="Elements that receive a click() event after the step is shown"
+        None, title="Post-click", description="Elements that receive a click() event after the step is shown"
     )
     textinsert: Optional[str] = Field(
-        title="Text-insert", description="Text to insert if element is a text box (e.g. tool search or upload)"
+        None, title="Text-insert", description="Text to insert if element is a text box (e.g. tool search or upload)"
     )
 
 
 class TourDetails(TourCore):
-    title_default: Optional[str] = Field(title="Default title", description="Default title for each step")
+    title_default: Optional[str] = Field(None, title="Default title", description="Default title for each step")
     steps: List[TourStep] = Field(title="Steps", description="Tour steps")
```

### Comparing `galaxy-tours-23.2.1/galaxy/tours/validate.py` & `galaxy-tours-24.0.0/galaxy/tours/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import sys
 
 import yaml
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 
 from galaxy.navigation.data import load_root_component
 from ._impl import (
     get_tour_id_from_path,
     load_tour_from_path,
     tour_paths,
 )
```

### Comparing `galaxy-tours-23.2.1/galaxy_tours.egg-info/PKG-INFO` & `galaxy-tours-24.0.0/galaxy_tours.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: galaxy-tours
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy tours backend framework
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
+Requires-Dist: galaxy-navigation
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: PyYAML
 
 
 .. image:: https://badge.fury.io/py/galaxy-tours.svg
    :target: https://pypi.org/project/galaxy-tours/
 
 
 Overview
@@ -44,14 +47,26 @@
 
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
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.1.4 (2024-01-04)
```

### Comparing `galaxy-tours-23.2.1/setup.cfg` & `galaxy-tours-24.0.0/setup.cfg`

 * *Files 9% similar despite different names*

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
 description = Galaxy tours backend framework
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tours
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
-	pydantic<2
+	pydantic>=2,!=2.6.0,!=2.6.1
 	PyYAML
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	gx-validate-tours = galaxy.tours.validate:main
 
 [options.packages.find]
 exclude =
```

