# Comparing `tmp/types-aiobotocore-iot1click-projects-2.9.0.tar.gz` & `tmp/types-aiobotocore-iot1click-projects-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot1click-projects-2.9.0.tar", last modified: Wed Dec 13 19:59:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot1click-projects-2.9.1.tar", last modified: Thu Jan 18 01:20:53 2024, max compression
```

## Comparing `types-aiobotocore-iot1click-projects-2.9.0.tar` & `types-aiobotocore-iot1click-projects-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:30.285670 types-aiobotocore-iot1click-projects-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13788 2023-12-13 19:59:30.285670 types-aiobotocore-iot1click-projects-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:30.285670 types-aiobotocore-iot1click-projects-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:30.285670 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14742 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8604 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2023-12-13 19:47:50.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8766 2023-12-13 19:47:50.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:30.285670 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13788 2023-12-13 19:59:30.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-13 19:59:30.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:30.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:30.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:30.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-13 19:59:30.000000 types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.937281 types-aiobotocore-iot1click-projects-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-01-18 01:20:53.937281 types-aiobotocore-iot1click-projects-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:53.937281 types-aiobotocore-iot1click-projects-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.933281 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.933281 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/LICENSE` & `types-aiobotocore-iot1click-projects-2.9.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/PKG-INFO` & `types-aiobotocore-iot1click-projects-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-projects
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-iot1click-projects"></a>
 
 # types-aiobotocore-iot1click-projects
 
 [![PyPI - types-aiobotocore-iot1click-projects](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickProjects 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[aiobotocore.IoT1ClickProjects 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/README.md` & `types-aiobotocore-iot1click-projects-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickProjects 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[aiobotocore.IoT1ClickProjects 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/setup.py` & `types-aiobotocore-iot1click-projects-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot1click-projects",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iot1click_projects"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoT1ClickProjects 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoT1ClickProjects 2.9.1 service generated with"
+        " mypy-boto3-builder 7.23.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="aiobotocore iot1click-projects type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot1click_projects": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/__init__.py` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import IoT1ClickProjectsClient
 from .paginator import ListPlacementsPaginator, ListProjectsPaginator
 
 Client = IoT1ClickProjectsClient
 
-
 __all__ = ("Client", "IoT1ClickProjectsClient", "ListPlacementsPaginator", "ListProjectsPaginator")
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/__init__.pyi` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/__main__.py` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoT1ClickProjects 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoT1ClickProjects 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.9.0")
+    print("2.9.1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/client.py` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoT1ClickProjectsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -113,15 +112,15 @@
 
     async def create_project(
         self,
         *,
         projectName: str,
         description: str = ...,
         placementTemplate: PlacementTemplateTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Creates an empty project with a placement template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#create_project)
         """
@@ -253,15 +252,15 @@
         """
 
     async def update_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateTypeDef = ...
+        placementTemplate: PlacementTemplateTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a project associated with your AWS account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#update_project)
         """
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/client.pyi` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     async def create_project(
         self,
         *,
         projectName: str,
         description: str = ...,
         placementTemplate: PlacementTemplateTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Creates an empty project with a placement template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#create_project)
         """
@@ -249,15 +249,15 @@
         """
 
     async def update_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateTypeDef = ...
+        placementTemplate: PlacementTemplateTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a project associated with your AWS account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#update_project)
         """
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/literals.py` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListPlacementsPaginatorName",
     "ListProjectsPaginatorName",
     "IoT1ClickProjectsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListPlacementsPaginatorName = Literal["list_placements"]
 ListProjectsPaginatorName = Literal["list_projects"]
 IoT1ClickProjectsServiceName = Literal["iot1click-projects"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/literals.pyi` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/paginator.py` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListPlacementsPaginator", "ListProjectsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/paginator.pyi` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/type_defs.py` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects/type_defs.pyi` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-projects
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-iot1click-projects"></a>
 
 # types-aiobotocore-iot1click-projects
 
 [![PyPI - types-aiobotocore-iot1click-projects](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickProjects 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[aiobotocore.IoT1ClickProjects 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot1click-projects-2.9.0/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt` & `types-aiobotocore-iot1click-projects-2.9.1/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

