# Comparing `tmp/types-aiobotocore-sagemaker-geospatial-2.9.0.tar.gz` & `tmp/types-aiobotocore-sagemaker-geospatial-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-geospatial-2.9.0.tar", last modified: Wed Dec 13 20:00:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-geospatial-2.9.1.tar", last modified: Thu Jan 18 01:21:43 2024, max compression
```

## Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0.tar` & `types-aiobotocore-sagemaker-geospatial-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:24.889185 types-aiobotocore-sagemaker-geospatial-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:42.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14313 2023-12-13 20:00:24.889185 types-aiobotocore-sagemaker-geospatial-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12687 2023-12-13 19:55:42.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:24.889185 types-aiobotocore-sagemaker-geospatial-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-13 19:55:42.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:24.889185 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-12-13 19:55:42.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-13 19:55:42.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-13 19:55:42.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20213 2023-12-13 19:55:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20209 2023-12-13 19:55:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11638 2023-12-13 19:55:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2023-12-13 19:55:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2023-12-13 19:55:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2023-12-13 19:55:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:42.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2023-12-13 19:55:46.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29126 2023-12-13 19:55:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:42.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:24.889185 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14313 2023-12-13 20:00:24.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-12-13 20:00:24.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:24.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:24.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:24.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-13 20:00:24.000000 types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:43.785057 types-aiobotocore-sagemaker-geospatial-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-01-18 01:21:43.785057 types-aiobotocore-sagemaker-geospatial-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:43.785057 types-aiobotocore-sagemaker-geospatial-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:43.785057 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20217 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29126 2024-01-18 01:17:18.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29126 2024-01-18 01:17:18.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:17.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:43.785057 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-01-18 01:21:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-18 01:21:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-18 01:21:43.000000 types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/LICENSE` & `types-aiobotocore-sagemaker-geospatial-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/PKG-INFO` & `types-aiobotocore-sagemaker-geospatial-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-geospatial
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/
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
 
 <a id="types-aiobotocore-sagemaker-geospatial"></a>
 
 # types-aiobotocore-sagemaker-geospatial
 
 [![PyPI - types-aiobotocore-sagemaker-geospatial](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-geospatial)](https://pepy.tech/project/types-aiobotocore-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakergeospatialcapabilities 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[aiobotocore.SageMakergeospatialcapabilities 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [types-aiobotocore-sagemaker-geospatial docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/README.md` & `types-aiobotocore-sagemaker-geospatial-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-geospatial)](https://pepy.tech/project/types-aiobotocore-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakergeospatialcapabilities 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[aiobotocore.SageMakergeospatialcapabilities 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [types-aiobotocore-sagemaker-geospatial docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/setup.py` & `types-aiobotocore-sagemaker-geospatial-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-geospatial",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sagemaker_geospatial"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.9.0 service generated"
-        " with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.9.1 service generated"
+        " with mypy-boto3-builder 7.23.1"
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
     keywords=(
         "aiobotocore sagemaker-geospatial type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sagemaker_geospatial": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/__init__.py` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListEarthObservationJobsPaginator,
     ListRasterDataCollectionsPaginator,
     ListVectorEnrichmentJobsPaginator,
 )
 
 Client = SageMakergeospatialcapabilitiesClient
 
-
 __all__ = (
     "Client",
     "ListEarthObservationJobsPaginator",
     "ListRasterDataCollectionsPaginator",
     "ListVectorEnrichmentJobsPaginator",
     "SageMakergeospatialcapabilitiesClient",
 )
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/__init__.pyi` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/__main__.py` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities\nOther"
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

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/client.py` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,37 +56,33 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SageMakergeospatialcapabilitiesClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class SageMakergeospatialcapabilitiesClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/)
     """
 
     meta: ClientMeta
@@ -135,15 +131,15 @@
     async def export_earth_observation_job(
         self,
         *,
         Arn: str,
         ExecutionRoleArn: str,
         OutputConfig: OutputConfigInputTypeDef,
         ClientToken: str = ...,
-        ExportSourceImages: bool = ...
+        ExportSourceImages: bool = ...,
     ) -> ExportEarthObservationJobOutputTypeDef:
         """
         Use this operation to export results of an Earth Observation job and optionally
         source images used as input to the EOJ to an Amazon S3
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_earth_observation_job)
@@ -152,15 +148,15 @@
 
     async def export_vector_enrichment_job(
         self,
         *,
         Arn: str,
         ExecutionRoleArn: str,
         OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> ExportVectorEnrichmentJobOutputTypeDef:
         """
         Use this operation to copy results of a Vector Enrichment job to an Amazon S3
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_vector_enrichment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#export_vector_enrichment_job)
@@ -206,15 +202,15 @@
         y: int,
         z: int,
         ExecutionRoleArn: str = ...,
         ImageMask: bool = ...,
         OutputDataType: OutputTypeType = ...,
         OutputFormat: str = ...,
         PropertyFilters: str = ...,
-        TimeRangeFilter: str = ...
+        TimeRangeFilter: str = ...,
     ) -> GetTileOutputTypeDef:
         """
         Gets a web mercator tile for the given Earth Observation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.get_tile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#get_tile)
         """
@@ -232,15 +228,15 @@
     async def list_earth_observation_jobs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        StatusEquals: EarthObservationJobStatusType = ...
+        StatusEquals: EarthObservationJobStatusType = ...,
     ) -> ListEarthObservationJobOutputTypeDef:
         """
         Use this operation to get a list of the Earth Observation jobs associated with
         the calling Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.list_earth_observation_jobs)
@@ -270,29 +266,29 @@
     async def list_vector_enrichment_jobs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        StatusEquals: str = ...
+        StatusEquals: str = ...,
     ) -> ListVectorEnrichmentJobOutputTypeDef:
         """
         Retrieves a list of vector enrichment jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.list_vector_enrichment_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#list_vector_enrichment_jobs)
         """
 
     async def search_raster_data_collection(
         self,
         *,
         Arn: str,
         RasterDataCollectionQuery: RasterDataCollectionQueryWithBandFilterInputTypeDef,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchRasterDataCollectionOutputTypeDef:
         """
         Allows you run image query on a specific raster data collection to get a list
         of the satellite imagery matching the selected
         filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.search_raster_data_collection)
@@ -304,15 +300,15 @@
         *,
         ExecutionRoleArn: str,
         InputConfig: InputConfigInputTypeDef,
         JobConfig: JobConfigInputTypeDef,
         Name: str,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> StartEarthObservationJobOutputTypeDef:
         """
         Use this operation to create an Earth observation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.start_earth_observation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#start_earth_observation_job)
         """
@@ -322,15 +318,15 @@
         *,
         ExecutionRoleArn: str,
         InputConfig: VectorEnrichmentJobInputConfigTypeDef,
         JobConfig: VectorEnrichmentJobConfigTypeDef,
         Name: str,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> StartVectorEnrichmentJobOutputTypeDef:
         """
         Creates a Vector Enrichment job for the supplied job type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.start_vector_enrichment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#start_vector_enrichment_job)
         """
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/client.pyi` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,31 +58,34 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("SageMakergeospatialcapabilitiesClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class SageMakergeospatialcapabilitiesClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/)
     """
 
     meta: ClientMeta
@@ -131,15 +134,15 @@
     async def export_earth_observation_job(
         self,
         *,
         Arn: str,
         ExecutionRoleArn: str,
         OutputConfig: OutputConfigInputTypeDef,
         ClientToken: str = ...,
-        ExportSourceImages: bool = ...
+        ExportSourceImages: bool = ...,
     ) -> ExportEarthObservationJobOutputTypeDef:
         """
         Use this operation to export results of an Earth Observation job and optionally
         source images used as input to the EOJ to an Amazon S3
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_earth_observation_job)
@@ -148,15 +151,15 @@
 
     async def export_vector_enrichment_job(
         self,
         *,
         Arn: str,
         ExecutionRoleArn: str,
         OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> ExportVectorEnrichmentJobOutputTypeDef:
         """
         Use this operation to copy results of a Vector Enrichment job to an Amazon S3
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_vector_enrichment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#export_vector_enrichment_job)
@@ -202,15 +205,15 @@
         y: int,
         z: int,
         ExecutionRoleArn: str = ...,
         ImageMask: bool = ...,
         OutputDataType: OutputTypeType = ...,
         OutputFormat: str = ...,
         PropertyFilters: str = ...,
-        TimeRangeFilter: str = ...
+        TimeRangeFilter: str = ...,
     ) -> GetTileOutputTypeDef:
         """
         Gets a web mercator tile for the given Earth Observation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.get_tile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#get_tile)
         """
@@ -228,15 +231,15 @@
     async def list_earth_observation_jobs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        StatusEquals: EarthObservationJobStatusType = ...
+        StatusEquals: EarthObservationJobStatusType = ...,
     ) -> ListEarthObservationJobOutputTypeDef:
         """
         Use this operation to get a list of the Earth Observation jobs associated with
         the calling Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.list_earth_observation_jobs)
@@ -266,29 +269,29 @@
     async def list_vector_enrichment_jobs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        StatusEquals: str = ...
+        StatusEquals: str = ...,
     ) -> ListVectorEnrichmentJobOutputTypeDef:
         """
         Retrieves a list of vector enrichment jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.list_vector_enrichment_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#list_vector_enrichment_jobs)
         """
 
     async def search_raster_data_collection(
         self,
         *,
         Arn: str,
         RasterDataCollectionQuery: RasterDataCollectionQueryWithBandFilterInputTypeDef,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchRasterDataCollectionOutputTypeDef:
         """
         Allows you run image query on a specific raster data collection to get a list
         of the satellite imagery matching the selected
         filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.search_raster_data_collection)
@@ -300,15 +303,15 @@
         *,
         ExecutionRoleArn: str,
         InputConfig: InputConfigInputTypeDef,
         JobConfig: JobConfigInputTypeDef,
         Name: str,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> StartEarthObservationJobOutputTypeDef:
         """
         Use this operation to create an Earth observation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.start_earth_observation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#start_earth_observation_job)
         """
@@ -318,15 +321,15 @@
         *,
         ExecutionRoleArn: str,
         InputConfig: VectorEnrichmentJobInputConfigTypeDef,
         JobConfig: VectorEnrichmentJobConfigTypeDef,
         Name: str,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> StartVectorEnrichmentJobOutputTypeDef:
         """
         Creates a Vector Enrichment job for the supplied job type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.start_vector_enrichment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#start_vector_enrichment_job)
         """
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/literals.py` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlgorithmNameCloudRemovalType",
     "AlgorithmNameGeoMosaicType",
     "AlgorithmNameResamplingType",
     "ComparisonOperatorType",
     "DataCollectionTypeType",
     "EarthObservationJobErrorTypeType",
@@ -51,15 +50,14 @@
     "SageMakergeospatialcapabilitiesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AlgorithmNameCloudRemovalType = Literal["INTERPOLATION"]
 AlgorithmNameGeoMosaicType = Literal[
     "AVERAGE",
     "BILINEAR",
     "CUBIC",
     "CUBICSPLINE",
     "LANCZOS",
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/literals.pyi` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/paginator.py` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
 __all__ = (
     "ListEarthObservationJobsPaginator",
     "ListRasterDataCollectionsPaginator",
     "ListVectorEnrichmentJobsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -63,15 +62,15 @@
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: EarthObservationJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEarthObservationJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/paginators/#listearthobservationjobspaginator)
         """
 
 
@@ -98,13 +97,13 @@
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVectorEnrichmentJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/paginators/#listvectorenrichmentjobspaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/paginator.pyi` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: EarthObservationJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEarthObservationJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/paginators/#listearthobservationjobspaginator)
         """
 
 class ListRasterDataCollectionsPaginator(AioPaginator):
@@ -93,13 +93,13 @@
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVectorEnrichmentJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/paginators/#listvectorenrichmentjobspaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/type_defs.py` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "MultiPolygonGeometryInputTypeDef",
     "PolygonGeometryInputTypeDef",
     "AssetValueTypeDef",
     "CloudRemovalConfigInputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial/type_defs.pyi` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-geospatial
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/
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
 
 <a id="types-aiobotocore-sagemaker-geospatial"></a>
 
 # types-aiobotocore-sagemaker-geospatial
 
 [![PyPI - types-aiobotocore-sagemaker-geospatial](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-geospatial)](https://pepy.tech/project/types-aiobotocore-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakergeospatialcapabilities 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[aiobotocore.SageMakergeospatialcapabilities 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [types-aiobotocore-sagemaker-geospatial docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.9.0/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-geospatial-2.9.1/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

