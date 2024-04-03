# Comparing `tmp/types-aiobotocore-robomaker-2.9.0.tar.gz` & `tmp/types-aiobotocore-robomaker-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-robomaker-2.9.0.tar", last modified: Wed Dec 13 20:00:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-robomaker-2.9.1.tar", last modified: Thu Jan 18 01:21:38 2024, max compression
```

## Comparing `types-aiobotocore-robomaker-2.9.0.tar` & `types-aiobotocore-robomaker-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.241234 types-aiobotocore-robomaker-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:42.000000 types-aiobotocore-robomaker-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2023-12-13 20:00:19.241234 types-aiobotocore-robomaker-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2023-12-13 19:54:42.000000 types-aiobotocore-robomaker-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:19.241234 types-aiobotocore-robomaker-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:54:42.000000 types-aiobotocore-robomaker-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.241234 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-12-13 19:54:42.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2023-12-13 19:54:42.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:54:42.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44854 2023-12-13 19:54:43.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    44850 2023-12-13 19:54:43.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2023-12-13 19:54:43.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2023-12-13 19:54:43.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14024 2023-12-13 19:54:43.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14011 2023-12-13 19:54:43.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:42.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    59385 2023-12-13 19:54:47.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    59384 2023-12-13 19:54:46.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:42.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.241234 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2023-12-13 20:00:19.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 20:00:19.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:19.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:19.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:19.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 20:00:19.000000 types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.677080 types-aiobotocore-robomaker-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-01-18 01:21:38.677080 types-aiobotocore-robomaker-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:38.681080 types-aiobotocore-robomaker-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.677080 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44869 2024-01-18 01:16:19.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44866 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-01-18 01:16:19.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-01-18 01:16:19.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-01-18 01:16:19.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-01-18 01:16:19.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    59384 2024-01-18 01:16:20.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59384 2024-01-18 01:16:20.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:18.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.677080 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-01-18 01:21:38.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:21:38.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:38.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:38.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:38.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:38.000000 types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-robomaker-2.9.0/LICENSE` & `types-aiobotocore-robomaker-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-robomaker-2.9.0/PKG-INFO` & `types-aiobotocore-robomaker-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-robomaker
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RoboMaker 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RoboMaker 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/
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
 
 <a id="types-aiobotocore-robomaker"></a>
 
 # types-aiobotocore-robomaker
 
 [![PyPI - types-aiobotocore-robomaker](https://img.shields.io/pypi/v/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RoboMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[aiobotocore.RoboMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [types-aiobotocore-robomaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-robomaker-2.9.0/README.md` & `types-aiobotocore-robomaker-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RoboMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[aiobotocore.RoboMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [types-aiobotocore-robomaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-robomaker-2.9.0/setup.py` & `types-aiobotocore-robomaker-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-robomaker",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RoboMaker 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.RoboMaker 2.9.1 service generated with mypy-boto3-builder"
+        " 7.23.1"
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
     keywords="aiobotocore robomaker type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_robomaker": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/__init__.py` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     ListWorldGenerationJobsPaginator,
     ListWorldsPaginator,
     ListWorldTemplatesPaginator,
 )
 
 Client = RoboMakerClient
 
-
 __all__ = (
     "Client",
     "ListDeploymentJobsPaginator",
     "ListFleetsPaginator",
     "ListRobotApplicationsPaginator",
     "ListRobotsPaginator",
     "ListSimulationApplicationsPaginator",
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/__init__.pyi` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/__main__.py` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RoboMaker 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.RoboMaker 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
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

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/client.py` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RoboMakerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -227,15 +226,15 @@
     async def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
         deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigTypeDef],
         deploymentConfig: DeploymentConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_deployment_job)
         """
@@ -252,15 +251,15 @@
 
     async def create_robot(
         self,
         *,
         name: str,
         architecture: ArchitectureType,
         greengrassGroupId: str,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRobotResponseTypeDef:
         """
         Creates a robot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_robot)
         """
@@ -268,30 +267,30 @@
     async def create_robot_application(
         self,
         *,
         name: str,
         robotSoftwareSuite: RobotSoftwareSuiteTypeDef,
         sources: Sequence[SourceConfigTypeDef] = ...,
         tags: Mapping[str, str] = ...,
-        environment: EnvironmentTypeDef = ...
+        environment: EnvironmentTypeDef = ...,
     ) -> CreateRobotApplicationResponseTypeDef:
         """
         Creates a robot application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_robot_application)
         """
 
     async def create_robot_application_version(
         self,
         *,
         application: str,
         currentRevisionId: str = ...,
         s3Etags: Sequence[str] = ...,
-        imageDigest: str = ...
+        imageDigest: str = ...,
     ) -> CreateRobotApplicationVersionResponseTypeDef:
         """
         Creates a version of a robot application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot_application_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_robot_application_version)
         """
@@ -301,30 +300,30 @@
         *,
         name: str,
         simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,
         robotSoftwareSuite: RobotSoftwareSuiteTypeDef,
         sources: Sequence[SourceConfigTypeDef] = ...,
         renderingEngine: RenderingEngineTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        environment: EnvironmentTypeDef = ...
+        environment: EnvironmentTypeDef = ...,
     ) -> CreateSimulationApplicationResponseTypeDef:
         """
         Creates a simulation application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_application)
         """
 
     async def create_simulation_application_version(
         self,
         *,
         application: str,
         currentRevisionId: str = ...,
         s3Etags: Sequence[str] = ...,
-        imageDigest: str = ...
+        imageDigest: str = ...,
     ) -> CreateSimulationApplicationVersionResponseTypeDef:
         """
         Creates a simulation application with a specific revision id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_application_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_application_version)
         """
@@ -339,15 +338,15 @@
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
         robotApplications: Sequence[RobotApplicationConfigTypeDef] = ...,
         simulationApplications: Sequence[SimulationApplicationConfigTypeDef] = ...,
         dataSources: Sequence[DataSourceConfigTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         vpcConfig: VPCConfigTypeDef = ...,
-        compute: ComputeTypeDef = ...
+        compute: ComputeTypeDef = ...,
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_job)
         """
@@ -355,15 +354,15 @@
     async def create_world_export_job(
         self,
         *,
         worlds: Sequence[str],
         outputLocation: OutputLocationTypeDef,
         iamRole: str,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateWorldExportJobResponseTypeDef:
         """
         Creates a world export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_world_export_job)
         """
@@ -371,15 +370,15 @@
     async def create_world_generation_job(
         self,
         *,
         template: str,
         worldCount: WorldCountTypeDef,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        worldTags: Mapping[str, str] = ...
+        worldTags: Mapping[str, str] = ...,
     ) -> CreateWorldGenerationJobResponseTypeDef:
         """
         Creates worlds using the specified template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_generation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_world_generation_job)
         """
@@ -387,15 +386,15 @@
     async def create_world_template(
         self,
         *,
         clientRequestToken: str = ...,
         name: str = ...,
         templateBody: str = ...,
         templateLocation: TemplateLocationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateWorldTemplateResponseTypeDef:
         """
         Creates a world template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_world_template)
         """
@@ -596,15 +595,15 @@
 
     async def list_robot_applications(
         self,
         *,
         versionQualifier: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filters: Sequence[FilterTypeDef] = ...
+        filters: Sequence[FilterTypeDef] = ...,
     ) -> ListRobotApplicationsResponseTypeDef:
         """
         Returns a list of robot application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_robot_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#list_robot_applications)
         """
@@ -621,15 +620,15 @@
 
     async def list_simulation_applications(
         self,
         *,
         versionQualifier: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filters: Sequence[FilterTypeDef] = ...
+        filters: Sequence[FilterTypeDef] = ...,
     ) -> ListSimulationApplicationsResponseTypeDef:
         """
         Returns a list of simulation applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_simulation_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#list_simulation_applications)
         """
@@ -722,15 +721,15 @@
 
     async def start_simulation_job_batch(
         self,
         *,
         createSimulationJobRequests: Sequence[SimulationJobRequestTypeDef],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.start_simulation_job_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#start_simulation_job_batch)
         """
@@ -764,15 +763,15 @@
     async def update_robot_application(
         self,
         *,
         application: str,
         robotSoftwareSuite: RobotSoftwareSuiteTypeDef,
         sources: Sequence[SourceConfigTypeDef] = ...,
         currentRevisionId: str = ...,
-        environment: EnvironmentTypeDef = ...
+        environment: EnvironmentTypeDef = ...,
     ) -> UpdateRobotApplicationResponseTypeDef:
         """
         Updates a robot application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_robot_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#update_robot_application)
         """
@@ -782,30 +781,30 @@
         *,
         application: str,
         simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,
         robotSoftwareSuite: RobotSoftwareSuiteTypeDef,
         sources: Sequence[SourceConfigTypeDef] = ...,
         renderingEngine: RenderingEngineTypeDef = ...,
         currentRevisionId: str = ...,
-        environment: EnvironmentTypeDef = ...
+        environment: EnvironmentTypeDef = ...,
     ) -> UpdateSimulationApplicationResponseTypeDef:
         """
         Updates a simulation application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_simulation_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#update_simulation_application)
         """
 
     async def update_world_template(
         self,
         *,
         template: str,
         name: str = ...,
         templateBody: str = ...,
-        templateLocation: TemplateLocationTypeDef = ...
+        templateLocation: TemplateLocationTypeDef = ...,
     ) -> UpdateWorldTemplateResponseTypeDef:
         """
         Updates a world template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_world_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#update_world_template)
         """
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/client.pyi` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
     async def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
         deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigTypeDef],
         deploymentConfig: DeploymentConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_deployment_job)
         """
@@ -248,15 +248,15 @@
 
     async def create_robot(
         self,
         *,
         name: str,
         architecture: ArchitectureType,
         greengrassGroupId: str,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRobotResponseTypeDef:
         """
         Creates a robot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_robot)
         """
@@ -264,30 +264,30 @@
     async def create_robot_application(
         self,
         *,
         name: str,
         robotSoftwareSuite: RobotSoftwareSuiteTypeDef,
         sources: Sequence[SourceConfigTypeDef] = ...,
         tags: Mapping[str, str] = ...,
-        environment: EnvironmentTypeDef = ...
+        environment: EnvironmentTypeDef = ...,
     ) -> CreateRobotApplicationResponseTypeDef:
         """
         Creates a robot application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_robot_application)
         """
 
     async def create_robot_application_version(
         self,
         *,
         application: str,
         currentRevisionId: str = ...,
         s3Etags: Sequence[str] = ...,
-        imageDigest: str = ...
+        imageDigest: str = ...,
     ) -> CreateRobotApplicationVersionResponseTypeDef:
         """
         Creates a version of a robot application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot_application_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_robot_application_version)
         """
@@ -297,30 +297,30 @@
         *,
         name: str,
         simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,
         robotSoftwareSuite: RobotSoftwareSuiteTypeDef,
         sources: Sequence[SourceConfigTypeDef] = ...,
         renderingEngine: RenderingEngineTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        environment: EnvironmentTypeDef = ...
+        environment: EnvironmentTypeDef = ...,
     ) -> CreateSimulationApplicationResponseTypeDef:
         """
         Creates a simulation application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_application)
         """
 
     async def create_simulation_application_version(
         self,
         *,
         application: str,
         currentRevisionId: str = ...,
         s3Etags: Sequence[str] = ...,
-        imageDigest: str = ...
+        imageDigest: str = ...,
     ) -> CreateSimulationApplicationVersionResponseTypeDef:
         """
         Creates a simulation application with a specific revision id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_application_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_application_version)
         """
@@ -335,15 +335,15 @@
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
         robotApplications: Sequence[RobotApplicationConfigTypeDef] = ...,
         simulationApplications: Sequence[SimulationApplicationConfigTypeDef] = ...,
         dataSources: Sequence[DataSourceConfigTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         vpcConfig: VPCConfigTypeDef = ...,
-        compute: ComputeTypeDef = ...
+        compute: ComputeTypeDef = ...,
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_job)
         """
@@ -351,15 +351,15 @@
     async def create_world_export_job(
         self,
         *,
         worlds: Sequence[str],
         outputLocation: OutputLocationTypeDef,
         iamRole: str,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateWorldExportJobResponseTypeDef:
         """
         Creates a world export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_world_export_job)
         """
@@ -367,15 +367,15 @@
     async def create_world_generation_job(
         self,
         *,
         template: str,
         worldCount: WorldCountTypeDef,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        worldTags: Mapping[str, str] = ...
+        worldTags: Mapping[str, str] = ...,
     ) -> CreateWorldGenerationJobResponseTypeDef:
         """
         Creates worlds using the specified template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_generation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_world_generation_job)
         """
@@ -383,15 +383,15 @@
     async def create_world_template(
         self,
         *,
         clientRequestToken: str = ...,
         name: str = ...,
         templateBody: str = ...,
         templateLocation: TemplateLocationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateWorldTemplateResponseTypeDef:
         """
         Creates a world template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_world_template)
         """
@@ -592,15 +592,15 @@
 
     async def list_robot_applications(
         self,
         *,
         versionQualifier: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filters: Sequence[FilterTypeDef] = ...
+        filters: Sequence[FilterTypeDef] = ...,
     ) -> ListRobotApplicationsResponseTypeDef:
         """
         Returns a list of robot application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_robot_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#list_robot_applications)
         """
@@ -617,15 +617,15 @@
 
     async def list_simulation_applications(
         self,
         *,
         versionQualifier: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filters: Sequence[FilterTypeDef] = ...
+        filters: Sequence[FilterTypeDef] = ...,
     ) -> ListSimulationApplicationsResponseTypeDef:
         """
         Returns a list of simulation applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_simulation_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#list_simulation_applications)
         """
@@ -718,15 +718,15 @@
 
     async def start_simulation_job_batch(
         self,
         *,
         createSimulationJobRequests: Sequence[SimulationJobRequestTypeDef],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.start_simulation_job_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#start_simulation_job_batch)
         """
@@ -760,15 +760,15 @@
     async def update_robot_application(
         self,
         *,
         application: str,
         robotSoftwareSuite: RobotSoftwareSuiteTypeDef,
         sources: Sequence[SourceConfigTypeDef] = ...,
         currentRevisionId: str = ...,
-        environment: EnvironmentTypeDef = ...
+        environment: EnvironmentTypeDef = ...,
     ) -> UpdateRobotApplicationResponseTypeDef:
         """
         Updates a robot application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_robot_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#update_robot_application)
         """
@@ -778,30 +778,30 @@
         *,
         application: str,
         simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,
         robotSoftwareSuite: RobotSoftwareSuiteTypeDef,
         sources: Sequence[SourceConfigTypeDef] = ...,
         renderingEngine: RenderingEngineTypeDef = ...,
         currentRevisionId: str = ...,
-        environment: EnvironmentTypeDef = ...
+        environment: EnvironmentTypeDef = ...,
     ) -> UpdateSimulationApplicationResponseTypeDef:
         """
         Updates a simulation application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_simulation_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#update_simulation_application)
         """
 
     async def update_world_template(
         self,
         *,
         template: str,
         name: str = ...,
         templateBody: str = ...,
-        templateLocation: TemplateLocationTypeDef = ...
+        templateLocation: TemplateLocationTypeDef = ...,
     ) -> UpdateWorldTemplateResponseTypeDef:
         """
         Updates a world template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_world_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#update_world_template)
         """
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/literals.py` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ArchitectureType",
     "ComputeTypeType",
     "DataSourceTypeType",
     "DeploymentJobErrorCodeType",
     "DeploymentStatusType",
     "ExitBehaviorType",
@@ -57,15 +56,14 @@
     "RoboMakerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ArchitectureType = Literal["ARM64", "ARMHF", "X86_64"]
 ComputeTypeType = Literal["CPU", "GPU_AND_CPU"]
 DataSourceTypeType = Literal["Archive", "File", "Prefix"]
 DeploymentJobErrorCodeType = Literal[
     "BadLambdaAssociated",
     "BadPermissionError",
     "DeploymentFleetDoesNotExist",
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/literals.pyi` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/paginator.py` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     "ListSimulationJobsPaginator",
     "ListWorldExportJobsPaginator",
     "ListWorldGenerationJobsPaginator",
     "ListWorldTemplatesPaginator",
     "ListWorldsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -93,15 +92,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listdeploymentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listdeploymentjobspaginator)
         """
 
 
@@ -111,15 +110,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listfleetspaginator)
         """
 
 
@@ -130,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRobotApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotapplicationspaginator)
         """
 
 
@@ -148,15 +147,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRobotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotspaginator)
         """
 
 
@@ -167,15 +166,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSimulationApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationapplicationspaginator)
         """
 
 
@@ -185,15 +184,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobbatchespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSimulationJobBatchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobbatchespaginator)
         """
 
 
@@ -203,15 +202,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSimulationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobspaginator)
         """
 
 
@@ -221,15 +220,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorldExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldexportjobspaginator)
         """
 
 
@@ -239,15 +238,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldgenerationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorldGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldgenerationjobspaginator)
         """
 
 
@@ -272,13 +271,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorldsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldspaginator)
         """
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/paginator.pyi` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listdeploymentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listdeploymentjobspaginator)
         """
 
 class ListFleetsPaginator(AioPaginator):
@@ -107,15 +107,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listfleetspaginator)
         """
 
 class ListRobotApplicationsPaginator(AioPaginator):
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRobotApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotapplicationspaginator)
         """
 
 class ListRobotsPaginator(AioPaginator):
@@ -142,15 +142,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRobotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotspaginator)
         """
 
 class ListSimulationApplicationsPaginator(AioPaginator):
@@ -160,15 +160,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSimulationApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationapplicationspaginator)
         """
 
 class ListSimulationJobBatchesPaginator(AioPaginator):
@@ -177,15 +177,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobbatchespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSimulationJobBatchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobbatchespaginator)
         """
 
 class ListSimulationJobsPaginator(AioPaginator):
@@ -194,15 +194,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSimulationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobspaginator)
         """
 
 class ListWorldExportJobsPaginator(AioPaginator):
@@ -211,15 +211,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorldExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldexportjobspaginator)
         """
 
 class ListWorldGenerationJobsPaginator(AioPaginator):
@@ -228,15 +228,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldgenerationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorldGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldgenerationjobspaginator)
         """
 
 class ListWorldTemplatesPaginator(AioPaginator):
@@ -259,13 +259,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorldsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldspaginator)
         """
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/type_defs.py` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker/type_defs.pyi` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/PKG-INFO` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-robomaker
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RoboMaker 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RoboMaker 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/
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
 
 <a id="types-aiobotocore-robomaker"></a>
 
 # types-aiobotocore-robomaker
 
 [![PyPI - types-aiobotocore-robomaker](https://img.shields.io/pypi/v/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RoboMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[aiobotocore.RoboMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [types-aiobotocore-robomaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-robomaker-2.9.0/types_aiobotocore_robomaker.egg-info/SOURCES.txt` & `types-aiobotocore-robomaker-2.9.1/types_aiobotocore_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

