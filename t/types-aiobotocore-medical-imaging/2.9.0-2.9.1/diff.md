# Comparing `tmp/types-aiobotocore-medical-imaging-2.9.0.tar.gz` & `tmp/types-aiobotocore-medical-imaging-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-medical-imaging-2.9.0.tar", last modified: Wed Dec 13 19:59:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-medical-imaging-2.9.1.tar", last modified: Thu Jan 18 01:21:17 2024, max compression
```

## Comparing `types-aiobotocore-medical-imaging-2.9.0.tar` & `types-aiobotocore-medical-imaging-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:55.717439 types-aiobotocore-medical-imaging-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2023-12-13 19:59:55.717439 types-aiobotocore-medical-imaging-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:55.717439 types-aiobotocore-medical-imaging-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:55.717439 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17696 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17692 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18778 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:22.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:55.717439 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2023-12-13 19:59:55.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 19:59:55.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:55.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:55.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:55.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 19:59:55.000000 types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.433176 types-aiobotocore-medical-imaging-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-01-18 01:21:17.433176 types-aiobotocore-medical-imaging-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:17.433176 types-aiobotocore-medical-imaging-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.433176 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17700 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-01-18 01:12:06.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-01-18 01:12:06.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:05.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.433176 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-01-18 01:21:17.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:21:17.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:17.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:17.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:17.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:21:17.000000 types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/LICENSE` & `types-aiobotocore-medical-imaging-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-medical-imaging-2.9.0/PKG-INFO` & `types-aiobotocore-medical-imaging-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-medical-imaging
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.HealthImaging 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.HealthImaging 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/
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
 
 <a id="types-aiobotocore-medical-imaging"></a>
 
 # types-aiobotocore-medical-imaging
 
 [![PyPI - types-aiobotocore-medical-imaging](https://img.shields.io/pypi/v/types-aiobotocore-medical-imaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medical-imaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medical-imaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medical-imaging)](https://pepy.tech/project/types-aiobotocore-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthImaging 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[aiobotocore.HealthImaging 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [types-aiobotocore-medical-imaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/README.md` & `types-aiobotocore-medical-imaging-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medical-imaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medical-imaging)](https://pepy.tech/project/types-aiobotocore-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthImaging 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[aiobotocore.HealthImaging 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [types-aiobotocore-medical-imaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/setup.py` & `types-aiobotocore-medical-imaging-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-medical-imaging",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_medical_imaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.HealthImaging 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.HealthImaging 2.9.1 service generated with"
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
     keywords="aiobotocore medical-imaging type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_medical_imaging": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/__init__.py` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListDICOMImportJobsPaginator,
     ListImageSetVersionsPaginator,
     SearchImageSetsPaginator,
 )
 
 Client = HealthImagingClient
 
-
 __all__ = (
     "Client",
     "HealthImagingClient",
     "ListDICOMImportJobsPaginator",
     "ListDatastoresPaginator",
     "ListImageSetVersionsPaginator",
     "SearchImageSetsPaginator",
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/__init__.pyi` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/__main__.py` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.HealthImaging 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.HealthImaging 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging\nOther"
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

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/client.py` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("HealthImagingClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -113,30 +112,30 @@
         """
 
     async def copy_image_set(
         self,
         *,
         datastoreId: str,
         sourceImageSetId: str,
-        copyImageSetInformation: CopyImageSetInformationTypeDef
+        copyImageSetInformation: CopyImageSetInformationTypeDef,
     ) -> CopyImageSetResponseTypeDef:
         """
         Copy an image set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.copy_image_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#copy_image_set)
         """
 
     async def create_datastore(
         self,
         *,
         clientToken: str,
         datastoreName: str = ...,
         tags: Mapping[str, str] = ...,
-        kmsKeyArn: str = ...
+        kmsKeyArn: str = ...,
     ) -> CreateDatastoreResponseTypeDef:
         """
         Create a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.create_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#create_datastore)
         """
@@ -192,15 +191,15 @@
         """
 
     async def get_image_frame(
         self,
         *,
         datastoreId: str,
         imageSetId: str,
-        imageFrameInformation: ImageFrameInformationTypeDef
+        imageFrameInformation: ImageFrameInformationTypeDef,
     ) -> GetImageFrameResponseTypeDef:
         """
         Get an image frame (pixel data) for an image set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.get_image_frame)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#get_image_frame)
         """
@@ -226,30 +225,30 @@
         """
 
     async def list_datastores(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDatastoresResponseTypeDef:
         """
         List data stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.list_datastores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#list_datastores)
         """
 
     async def list_dicom_import_jobs(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDICOMImportJobsResponseTypeDef:
         """
         List import jobs created for a specific data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.list_dicom_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#list_dicom_import_jobs)
         """
@@ -276,15 +275,15 @@
 
     async def search_image_sets(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchImageSetsResponseTypeDef:
         """
         Search image sets based on defined input attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.search_image_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#search_image_sets)
         """
@@ -293,15 +292,15 @@
         self,
         *,
         dataAccessRoleArn: str,
         clientToken: str,
         datastoreId: str,
         inputS3Uri: str,
         outputS3Uri: str,
-        jobName: str = ...
+        jobName: str = ...,
     ) -> StartDICOMImportJobResponseTypeDef:
         """
         Start importing bulk data into an `ACTIVE` data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.start_dicom_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#start_dicom_import_job)
         """
@@ -324,15 +323,15 @@
 
     async def update_image_set_metadata(
         self,
         *,
         datastoreId: str,
         imageSetId: str,
         latestVersionId: str,
-        updateImageSetMetadataUpdates: MetadataUpdatesTypeDef
+        updateImageSetMetadataUpdates: MetadataUpdatesTypeDef,
     ) -> UpdateImageSetMetadataResponseTypeDef:
         """
         Update image set metadata attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.update_image_set_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#update_image_set_metadata)
         """
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/client.pyi` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -109,30 +109,30 @@
         """
 
     async def copy_image_set(
         self,
         *,
         datastoreId: str,
         sourceImageSetId: str,
-        copyImageSetInformation: CopyImageSetInformationTypeDef
+        copyImageSetInformation: CopyImageSetInformationTypeDef,
     ) -> CopyImageSetResponseTypeDef:
         """
         Copy an image set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.copy_image_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#copy_image_set)
         """
 
     async def create_datastore(
         self,
         *,
         clientToken: str,
         datastoreName: str = ...,
         tags: Mapping[str, str] = ...,
-        kmsKeyArn: str = ...
+        kmsKeyArn: str = ...,
     ) -> CreateDatastoreResponseTypeDef:
         """
         Create a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.create_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#create_datastore)
         """
@@ -188,15 +188,15 @@
         """
 
     async def get_image_frame(
         self,
         *,
         datastoreId: str,
         imageSetId: str,
-        imageFrameInformation: ImageFrameInformationTypeDef
+        imageFrameInformation: ImageFrameInformationTypeDef,
     ) -> GetImageFrameResponseTypeDef:
         """
         Get an image frame (pixel data) for an image set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.get_image_frame)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#get_image_frame)
         """
@@ -222,30 +222,30 @@
         """
 
     async def list_datastores(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDatastoresResponseTypeDef:
         """
         List data stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.list_datastores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#list_datastores)
         """
 
     async def list_dicom_import_jobs(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDICOMImportJobsResponseTypeDef:
         """
         List import jobs created for a specific data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.list_dicom_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#list_dicom_import_jobs)
         """
@@ -272,15 +272,15 @@
 
     async def search_image_sets(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchImageSetsResponseTypeDef:
         """
         Search image sets based on defined input attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.search_image_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#search_image_sets)
         """
@@ -289,15 +289,15 @@
         self,
         *,
         dataAccessRoleArn: str,
         clientToken: str,
         datastoreId: str,
         inputS3Uri: str,
         outputS3Uri: str,
-        jobName: str = ...
+        jobName: str = ...,
     ) -> StartDICOMImportJobResponseTypeDef:
         """
         Start importing bulk data into an `ACTIVE` data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.start_dicom_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#start_dicom_import_job)
         """
@@ -320,15 +320,15 @@
 
     async def update_image_set_metadata(
         self,
         *,
         datastoreId: str,
         imageSetId: str,
         latestVersionId: str,
-        updateImageSetMetadataUpdates: MetadataUpdatesTypeDef
+        updateImageSetMetadataUpdates: MetadataUpdatesTypeDef,
     ) -> UpdateImageSetMetadataResponseTypeDef:
         """
         Update image set metadata attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.update_image_set_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/client/#update_image_set_metadata)
         """
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/literals.py` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/literals.py`

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
     "DatastoreStatusType",
     "ImageSetStateType",
     "ImageSetWorkflowStatusType",
     "JobStatusType",
     "ListDICOMImportJobsPaginatorName",
     "ListDatastoresPaginatorName",
@@ -32,15 +31,14 @@
     "SearchImageSetsPaginatorName",
     "HealthImagingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 DatastoreStatusType = Literal["ACTIVE", "CREATE_FAILED", "CREATING", "DELETED", "DELETING"]
 ImageSetStateType = Literal["ACTIVE", "DELETED", "LOCKED"]
 ImageSetWorkflowStatusType = Literal[
     "COPIED",
     "COPYING",
     "COPYING_WITH_READ_ONLY_ACCESS",
     "COPY_FAILED",
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/literals.pyi` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/paginator.py` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 __all__ = (
     "ListDICOMImportJobsPaginator",
     "ListDatastoresPaginator",
     "ListImageSetVersionsPaginator",
     "SearchImageSetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -67,15 +66,15 @@
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDICOMImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/paginators/#listdicomimportjobspaginator)
         """
 
 
@@ -85,15 +84,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/paginators/#listdatastorespaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/paginators/#listdatastorespaginator)
         """
 
 
@@ -119,13 +118,13 @@
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchImageSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/paginators/#searchimagesetspaginator)
         """
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/paginator.pyi` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDICOMImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/paginators/#listdicomimportjobspaginator)
         """
 
 class ListDatastoresPaginator(AioPaginator):
@@ -81,15 +81,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/paginators/#listdatastorespaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/paginators/#listdatastorespaginator)
         """
 
 class ListImageSetVersionsPaginator(AioPaginator):
@@ -113,13 +113,13 @@
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchImageSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/paginators/#searchimagesetspaginator)
         """
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/type_defs.py` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "CopyDestinationImageSetPropertiesTypeDef",
     "CopyDestinationImageSetTypeDef",
     "CopySourceImageSetInformationTypeDef",
     "CopySourceImageSetPropertiesTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging/type_defs.pyi` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/PKG-INFO` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-medical-imaging
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.HealthImaging 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.HealthImaging 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/
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
 
 <a id="types-aiobotocore-medical-imaging"></a>
 
 # types-aiobotocore-medical-imaging
 
 [![PyPI - types-aiobotocore-medical-imaging](https://img.shields.io/pypi/v/types-aiobotocore-medical-imaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medical-imaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medical-imaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medical-imaging)](https://pepy.tech/project/types-aiobotocore-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthImaging 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[aiobotocore.HealthImaging 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [types-aiobotocore-medical-imaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-medical-imaging-2.9.0/types_aiobotocore_medical_imaging.egg-info/SOURCES.txt` & `types-aiobotocore-medical-imaging-2.9.1/types_aiobotocore_medical_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

