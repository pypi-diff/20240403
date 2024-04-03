# Comparing `tmp/types-aiobotocore-omics-2.9.0.tar.gz` & `tmp/types-aiobotocore-omics-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-omics-2.9.0.tar", last modified: Wed Dec 13 20:00:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-omics-2.9.1.tar", last modified: Thu Jan 18 01:21:23 2024, max compression
```

## Comparing `types-aiobotocore-omics-2.9.0.tar` & `types-aiobotocore-omics-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:02.893376 types-aiobotocore-omics-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19063 2023-12-13 20:00:02.893376 types-aiobotocore-omics-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17508 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:02.893376 types-aiobotocore-omics-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:02.893376 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72897 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    72893 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17547 2023-12-13 19:51:04.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    17545 2023-12-13 19:51:04.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25409 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25387 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    84786 2023-12-13 19:51:07.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    84785 2023-12-13 19:51:04.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    18159 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18141 2023-12-13 19:51:03.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:02.893376 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19063 2023-12-13 20:00:02.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-12-13 20:00:02.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:02.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:02.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:02.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 20:00:02.000000 types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:23.917146 types-aiobotocore-omics-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-01-18 01:21:23.917146 types-aiobotocore-omics-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:23.917146 types-aiobotocore-omics-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:23.917146 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72934 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72931 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17545 2024-01-18 01:12:45.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17545 2024-01-18 01:12:45.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25426 2024-01-18 01:12:45.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25405 2024-01-18 01:12:45.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    84785 2024-01-18 01:12:47.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84785 2024-01-18 01:12:46.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:44.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-01-18 01:12:45.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-01-18 01:12:45.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:23.917146 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-01-18 01:21:23.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-18 01:21:23.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:23.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:23.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:23.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:21:23.000000 types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-omics-2.9.0/LICENSE` & `types-aiobotocore-omics-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-omics-2.9.0/PKG-INFO` & `types-aiobotocore-omics-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-omics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Omics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Omics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/
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
 
 <a id="types-aiobotocore-omics"></a>
 
 # types-aiobotocore-omics
 
 [![PyPI - types-aiobotocore-omics](https://img.shields.io/pypi/v/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Omics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[aiobotocore.Omics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [types-aiobotocore-omics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-omics-2.9.0/README.md` & `types-aiobotocore-omics-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Omics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[aiobotocore.Omics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [types-aiobotocore-omics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-omics-2.9.0/setup.py` & `types-aiobotocore-omics-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-omics",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Omics 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Omics 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore omics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_omics": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/__init__.py` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,14 @@
     VariantStoreCreatedWaiter,
     VariantStoreDeletedWaiter,
     WorkflowActiveWaiter,
 )
 
 Client = OmicsClient
 
-
 __all__ = (
     "AnnotationImportJobCreatedWaiter",
     "AnnotationStoreCreatedWaiter",
     "AnnotationStoreDeletedWaiter",
     "AnnotationStoreVersionCreatedWaiter",
     "AnnotationStoreVersionDeletedWaiter",
     "Client",
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/__init__.pyi` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/__main__.py` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Omics 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Omics 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
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

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/client.py` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("OmicsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -294,15 +293,15 @@
         """
 
     async def complete_multipart_read_set_upload(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
-        parts: Sequence[CompleteReadSetUploadPartListItemTypeDef]
+        parts: Sequence[CompleteReadSetUploadPartListItemTypeDef],
     ) -> CompleteMultipartReadSetUploadResponseTypeDef:
         """
         Concludes a multipart upload once you have uploaded all the components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.complete_multipart_read_set_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#complete_multipart_read_set_upload)
         """
@@ -313,15 +312,15 @@
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         versionName: str = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: StoreOptionsTypeDef = ...
+        storeOptions: StoreOptionsTypeDef = ...,
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_annotation_store)
         """
@@ -329,15 +328,15 @@
     async def create_annotation_store_version(
         self,
         *,
         name: str,
         versionName: str,
         description: str = ...,
         versionOptions: VersionOptionsTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAnnotationStoreVersionResponseTypeDef:
         """
         Creates a new version of an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_annotation_store_version)
         """
@@ -350,15 +349,15 @@
         subjectId: str,
         sampleId: str,
         name: str,
         clientToken: str = ...,
         generatedFrom: str = ...,
         referenceArn: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateMultipartReadSetUploadResponseTypeDef:
         """
         Begins a multipart read set upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_multipart_read_set_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_multipart_read_set_upload)
         """
@@ -366,15 +365,15 @@
     async def create_reference_store(
         self,
         *,
         name: str,
         description: str = ...,
         sseConfig: SseConfigTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateReferenceStoreResponseTypeDef:
         """
         Creates a reference store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_reference_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_reference_store)
         """
@@ -384,15 +383,15 @@
         *,
         requestId: str,
         name: str = ...,
         maxCpus: int = ...,
         maxRuns: int = ...,
         maxDuration: int = ...,
         tags: Mapping[str, str] = ...,
-        maxGpus: int = ...
+        maxGpus: int = ...,
     ) -> CreateRunGroupResponseTypeDef:
         """
         Creates a run group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_run_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_run_group)
         """
@@ -401,15 +400,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         sseConfig: SseConfigTypeDef = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...,
-        fallbackLocation: str = ...
+        fallbackLocation: str = ...,
     ) -> CreateSequenceStoreResponseTypeDef:
         """
         Creates a sequence store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_sequence_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_sequence_store)
         """
@@ -427,15 +426,15 @@
     async def create_variant_store(
         self,
         *,
         reference: ReferenceItemTypeDef,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
-        sseConfig: SseConfigTypeDef = ...
+        sseConfig: SseConfigTypeDef = ...,
     ) -> CreateVariantStoreResponseTypeDef:
         """
         Creates a variant store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_variant_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_variant_store)
         """
@@ -449,15 +448,15 @@
         engine: WorkflowEngineType = ...,
         definitionZip: BlobTypeDef = ...,
         definitionUri: str = ...,
         main: str = ...,
         parameterTemplate: Mapping[str, WorkflowParameterTypeDef] = ...,
         storageCapacity: int = ...,
         tags: Mapping[str, str] = ...,
-        accelerators: Literal["GPU"] = ...
+        accelerators: Literal["GPU"] = ...,
     ) -> CreateWorkflowResponseTypeDef:
         """
         Creates a workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_workflow)
         """
@@ -641,15 +640,15 @@
     async def get_reference(
         self,
         *,
         id: str,
         referenceStoreId: str,
         partNumber: int,
         range: str = ...,
-        file: ReferenceFileType = ...
+        file: ReferenceFileType = ...,
     ) -> GetReferenceResponseTypeDef:
         """
         Gets a reference file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_reference)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#get_reference)
         """
@@ -741,60 +740,60 @@
         """
 
     async def get_workflow(
         self,
         *,
         id: str,
         type: WorkflowTypeType = ...,
-        export: Sequence[Literal["DEFINITION"]] = ...
+        export: Sequence[Literal["DEFINITION"]] = ...,
     ) -> GetWorkflowResponseTypeDef:
         """
         Gets information about a workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#get_workflow)
         """
 
     async def list_annotation_import_jobs(
         self,
         *,
         maxResults: int = ...,
         ids: Sequence[str] = ...,
         nextToken: str = ...,
-        filter: ListAnnotationImportJobsFilterTypeDef = ...
+        filter: ListAnnotationImportJobsFilterTypeDef = ...,
     ) -> ListAnnotationImportJobsResponseTypeDef:
         """
         Retrieves a list of annotation import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_annotation_import_jobs)
         """
 
     async def list_annotation_store_versions(
         self,
         *,
         name: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ListAnnotationStoreVersionsFilterTypeDef = ...
+        filter: ListAnnotationStoreVersionsFilterTypeDef = ...,
     ) -> ListAnnotationStoreVersionsResponseTypeDef:
         """
         Lists the versions of an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_store_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_annotation_store_versions)
         """
 
     async def list_annotation_stores(
         self,
         *,
         ids: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ListAnnotationStoresFilterTypeDef = ...
+        filter: ListAnnotationStoresFilterTypeDef = ...,
     ) -> ListAnnotationStoresResponseTypeDef:
         """
         Retrieves a list of annotation stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_annotation_stores)
         """
@@ -811,45 +810,45 @@
 
     async def list_read_set_activation_jobs(
         self,
         *,
         sequenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ActivateReadSetFilterTypeDef = ...
+        filter: ActivateReadSetFilterTypeDef = ...,
     ) -> ListReadSetActivationJobsResponseTypeDef:
         """
         Retrieves a list of read set activation jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_activation_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_read_set_activation_jobs)
         """
 
     async def list_read_set_export_jobs(
         self,
         *,
         sequenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ExportReadSetFilterTypeDef = ...
+        filter: ExportReadSetFilterTypeDef = ...,
     ) -> ListReadSetExportJobsResponseTypeDef:
         """
         Retrieves a list of read set export jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_read_set_export_jobs)
         """
 
     async def list_read_set_import_jobs(
         self,
         *,
         sequenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ImportReadSetFilterTypeDef = ...
+        filter: ImportReadSetFilterTypeDef = ...,
     ) -> ListReadSetImportJobsResponseTypeDef:
         """
         Retrieves a list of read set import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_read_set_import_jobs)
         """
@@ -858,15 +857,15 @@
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ReadSetUploadPartListFilterTypeDef = ...
+        filter: ReadSetUploadPartListFilterTypeDef = ...,
     ) -> ListReadSetUploadPartsResponseTypeDef:
         """
         This operation will list all parts in a requested multipart upload for a
         sequence
         store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_upload_parts)
@@ -875,59 +874,59 @@
 
     async def list_read_sets(
         self,
         *,
         sequenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ReadSetFilterTypeDef = ...
+        filter: ReadSetFilterTypeDef = ...,
     ) -> ListReadSetsResponseTypeDef:
         """
         Retrieves a list of read sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_read_sets)
         """
 
     async def list_reference_import_jobs(
         self,
         *,
         referenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ImportReferenceFilterTypeDef = ...
+        filter: ImportReferenceFilterTypeDef = ...,
     ) -> ListReferenceImportJobsResponseTypeDef:
         """
         Retrieves a list of reference import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_reference_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_reference_import_jobs)
         """
 
     async def list_reference_stores(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ReferenceStoreFilterTypeDef = ...
+        filter: ReferenceStoreFilterTypeDef = ...,
     ) -> ListReferenceStoresResponseTypeDef:
         """
         Retrieves a list of reference stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_reference_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_reference_stores)
         """
 
     async def list_references(
         self,
         *,
         referenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ReferenceFilterTypeDef = ...
+        filter: ReferenceFilterTypeDef = ...,
     ) -> ListReferencesResponseTypeDef:
         """
         Retrieves a list of references.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_references)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_references)
         """
@@ -944,15 +943,15 @@
 
     async def list_run_tasks(
         self,
         *,
         id: str,
         status: TaskStatusType = ...,
         startingToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListRunTasksResponseTypeDef:
         """
         Retrieves a list of tasks for a run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_run_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_run_tasks)
         """
@@ -960,44 +959,44 @@
     async def list_runs(
         self,
         *,
         name: str = ...,
         runGroupId: str = ...,
         startingToken: str = ...,
         maxResults: int = ...,
-        status: RunStatusType = ...
+        status: RunStatusType = ...,
     ) -> ListRunsResponseTypeDef:
         """
         Retrieves a list of runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_runs)
         """
 
     async def list_sequence_stores(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: SequenceStoreFilterTypeDef = ...
+        filter: SequenceStoreFilterTypeDef = ...,
     ) -> ListSequenceStoresResponseTypeDef:
         """
         Retrieves a list of sequence stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_sequence_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_sequence_stores)
         """
 
     async def list_shares(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         filter: FilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListSharesResponseTypeDef:
         """
         Lists all shares associated with an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_shares)
         """
@@ -1014,45 +1013,45 @@
 
     async def list_variant_import_jobs(
         self,
         *,
         maxResults: int = ...,
         ids: Sequence[str] = ...,
         nextToken: str = ...,
-        filter: ListVariantImportJobsFilterTypeDef = ...
+        filter: ListVariantImportJobsFilterTypeDef = ...,
     ) -> ListVariantImportJobsResponseTypeDef:
         """
         Retrieves a list of variant import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_variant_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_variant_import_jobs)
         """
 
     async def list_variant_stores(
         self,
         *,
         maxResults: int = ...,
         ids: Sequence[str] = ...,
         nextToken: str = ...,
-        filter: ListVariantStoresFilterTypeDef = ...
+        filter: ListVariantStoresFilterTypeDef = ...,
     ) -> ListVariantStoresResponseTypeDef:
         """
         Retrieves a list of variant stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_variant_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_variant_stores)
         """
 
     async def list_workflows(
         self,
         *,
         type: WorkflowTypeType = ...,
         name: str = ...,
         startingToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListWorkflowsResponseTypeDef:
         """
         Retrieves a list of workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_workflows)
         """
@@ -1062,29 +1061,29 @@
         *,
         destinationName: str,
         roleArn: str,
         items: Sequence[AnnotationImportItemSourceTypeDef],
         versionName: str = ...,
         formatOptions: FormatOptionsTypeDef = ...,
         runLeftNormalization: bool = ...,
-        annotationFields: Mapping[str, str] = ...
+        annotationFields: Mapping[str, str] = ...,
     ) -> StartAnnotationImportResponseTypeDef:
         """
         Starts an annotation import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_annotation_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_annotation_import_job)
         """
 
     async def start_read_set_activation_job(
         self,
         *,
         sequenceStoreId: str,
         sources: Sequence[StartReadSetActivationJobSourceItemTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartReadSetActivationJobResponseTypeDef:
         """
         Activates an archived read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_activation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_read_set_activation_job)
         """
@@ -1092,45 +1091,45 @@
     async def start_read_set_export_job(
         self,
         *,
         sequenceStoreId: str,
         destination: str,
         roleArn: str,
         sources: Sequence[ExportReadSetTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartReadSetExportJobResponseTypeDef:
         """
         Exports a read set to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_read_set_export_job)
         """
 
     async def start_read_set_import_job(
         self,
         *,
         sequenceStoreId: str,
         roleArn: str,
         sources: Sequence[StartReadSetImportJobSourceItemTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartReadSetImportJobResponseTypeDef:
         """
         Starts a read set import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_read_set_import_job)
         """
 
     async def start_reference_import_job(
         self,
         *,
         referenceStoreId: str,
         roleArn: str,
         sources: Sequence[StartReferenceImportJobSourceItemTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartReferenceImportJobResponseTypeDef:
         """
         Starts a reference import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_reference_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_reference_import_job)
         """
@@ -1147,15 +1146,15 @@
         runGroupId: str = ...,
         priority: int = ...,
         parameters: Mapping[str, Any] = ...,
         storageCapacity: int = ...,
         outputUri: str = ...,
         logLevel: RunLogLevelType = ...,
         tags: Mapping[str, str] = ...,
-        retentionMode: RunRetentionModeType = ...
+        retentionMode: RunRetentionModeType = ...,
     ) -> StartRunResponseTypeDef:
         """
         Starts a workflow run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_run)
         """
@@ -1163,15 +1162,15 @@
     async def start_variant_import_job(
         self,
         *,
         destinationName: str,
         roleArn: str,
         items: Sequence[VariantImportItemSourceTypeDef],
         runLeftNormalization: bool = ...,
-        annotationFields: Mapping[str, str] = ...
+        annotationFields: Mapping[str, str] = ...,
     ) -> StartVariantImportResponseTypeDef:
         """
         Starts a variant import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_variant_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_variant_import_job)
         """
@@ -1216,15 +1215,15 @@
         self,
         *,
         id: str,
         name: str = ...,
         maxCpus: int = ...,
         maxRuns: int = ...,
         maxDuration: int = ...,
-        maxGpus: int = ...
+        maxGpus: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a run group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.update_run_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#update_run_group)
         """
@@ -1252,15 +1251,15 @@
     async def upload_read_set_part(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         partNumber: int,
-        payload: BlobTypeDef
+        payload: BlobTypeDef,
     ) -> UploadReadSetPartResponseTypeDef:
         """
         This operation uploads a specific part of a read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.upload_read_set_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#upload_read_set_part)
         """
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/client.pyi` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         """
 
     async def complete_multipart_read_set_upload(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
-        parts: Sequence[CompleteReadSetUploadPartListItemTypeDef]
+        parts: Sequence[CompleteReadSetUploadPartListItemTypeDef],
     ) -> CompleteMultipartReadSetUploadResponseTypeDef:
         """
         Concludes a multipart upload once you have uploaded all the components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.complete_multipart_read_set_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#complete_multipart_read_set_upload)
         """
@@ -309,15 +309,15 @@
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         versionName: str = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: StoreOptionsTypeDef = ...
+        storeOptions: StoreOptionsTypeDef = ...,
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_annotation_store)
         """
@@ -325,15 +325,15 @@
     async def create_annotation_store_version(
         self,
         *,
         name: str,
         versionName: str,
         description: str = ...,
         versionOptions: VersionOptionsTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAnnotationStoreVersionResponseTypeDef:
         """
         Creates a new version of an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_annotation_store_version)
         """
@@ -346,15 +346,15 @@
         subjectId: str,
         sampleId: str,
         name: str,
         clientToken: str = ...,
         generatedFrom: str = ...,
         referenceArn: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateMultipartReadSetUploadResponseTypeDef:
         """
         Begins a multipart read set upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_multipart_read_set_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_multipart_read_set_upload)
         """
@@ -362,15 +362,15 @@
     async def create_reference_store(
         self,
         *,
         name: str,
         description: str = ...,
         sseConfig: SseConfigTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateReferenceStoreResponseTypeDef:
         """
         Creates a reference store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_reference_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_reference_store)
         """
@@ -380,15 +380,15 @@
         *,
         requestId: str,
         name: str = ...,
         maxCpus: int = ...,
         maxRuns: int = ...,
         maxDuration: int = ...,
         tags: Mapping[str, str] = ...,
-        maxGpus: int = ...
+        maxGpus: int = ...,
     ) -> CreateRunGroupResponseTypeDef:
         """
         Creates a run group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_run_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_run_group)
         """
@@ -397,15 +397,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         sseConfig: SseConfigTypeDef = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...,
-        fallbackLocation: str = ...
+        fallbackLocation: str = ...,
     ) -> CreateSequenceStoreResponseTypeDef:
         """
         Creates a sequence store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_sequence_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_sequence_store)
         """
@@ -423,15 +423,15 @@
     async def create_variant_store(
         self,
         *,
         reference: ReferenceItemTypeDef,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
-        sseConfig: SseConfigTypeDef = ...
+        sseConfig: SseConfigTypeDef = ...,
     ) -> CreateVariantStoreResponseTypeDef:
         """
         Creates a variant store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_variant_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_variant_store)
         """
@@ -445,15 +445,15 @@
         engine: WorkflowEngineType = ...,
         definitionZip: BlobTypeDef = ...,
         definitionUri: str = ...,
         main: str = ...,
         parameterTemplate: Mapping[str, WorkflowParameterTypeDef] = ...,
         storageCapacity: int = ...,
         tags: Mapping[str, str] = ...,
-        accelerators: Literal["GPU"] = ...
+        accelerators: Literal["GPU"] = ...,
     ) -> CreateWorkflowResponseTypeDef:
         """
         Creates a workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_workflow)
         """
@@ -637,15 +637,15 @@
     async def get_reference(
         self,
         *,
         id: str,
         referenceStoreId: str,
         partNumber: int,
         range: str = ...,
-        file: ReferenceFileType = ...
+        file: ReferenceFileType = ...,
     ) -> GetReferenceResponseTypeDef:
         """
         Gets a reference file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_reference)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#get_reference)
         """
@@ -737,60 +737,60 @@
         """
 
     async def get_workflow(
         self,
         *,
         id: str,
         type: WorkflowTypeType = ...,
-        export: Sequence[Literal["DEFINITION"]] = ...
+        export: Sequence[Literal["DEFINITION"]] = ...,
     ) -> GetWorkflowResponseTypeDef:
         """
         Gets information about a workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#get_workflow)
         """
 
     async def list_annotation_import_jobs(
         self,
         *,
         maxResults: int = ...,
         ids: Sequence[str] = ...,
         nextToken: str = ...,
-        filter: ListAnnotationImportJobsFilterTypeDef = ...
+        filter: ListAnnotationImportJobsFilterTypeDef = ...,
     ) -> ListAnnotationImportJobsResponseTypeDef:
         """
         Retrieves a list of annotation import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_annotation_import_jobs)
         """
 
     async def list_annotation_store_versions(
         self,
         *,
         name: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ListAnnotationStoreVersionsFilterTypeDef = ...
+        filter: ListAnnotationStoreVersionsFilterTypeDef = ...,
     ) -> ListAnnotationStoreVersionsResponseTypeDef:
         """
         Lists the versions of an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_store_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_annotation_store_versions)
         """
 
     async def list_annotation_stores(
         self,
         *,
         ids: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ListAnnotationStoresFilterTypeDef = ...
+        filter: ListAnnotationStoresFilterTypeDef = ...,
     ) -> ListAnnotationStoresResponseTypeDef:
         """
         Retrieves a list of annotation stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_annotation_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_annotation_stores)
         """
@@ -807,45 +807,45 @@
 
     async def list_read_set_activation_jobs(
         self,
         *,
         sequenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ActivateReadSetFilterTypeDef = ...
+        filter: ActivateReadSetFilterTypeDef = ...,
     ) -> ListReadSetActivationJobsResponseTypeDef:
         """
         Retrieves a list of read set activation jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_activation_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_read_set_activation_jobs)
         """
 
     async def list_read_set_export_jobs(
         self,
         *,
         sequenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ExportReadSetFilterTypeDef = ...
+        filter: ExportReadSetFilterTypeDef = ...,
     ) -> ListReadSetExportJobsResponseTypeDef:
         """
         Retrieves a list of read set export jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_read_set_export_jobs)
         """
 
     async def list_read_set_import_jobs(
         self,
         *,
         sequenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ImportReadSetFilterTypeDef = ...
+        filter: ImportReadSetFilterTypeDef = ...,
     ) -> ListReadSetImportJobsResponseTypeDef:
         """
         Retrieves a list of read set import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_read_set_import_jobs)
         """
@@ -854,15 +854,15 @@
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ReadSetUploadPartListFilterTypeDef = ...
+        filter: ReadSetUploadPartListFilterTypeDef = ...,
     ) -> ListReadSetUploadPartsResponseTypeDef:
         """
         This operation will list all parts in a requested multipart upload for a
         sequence
         store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_set_upload_parts)
@@ -871,59 +871,59 @@
 
     async def list_read_sets(
         self,
         *,
         sequenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ReadSetFilterTypeDef = ...
+        filter: ReadSetFilterTypeDef = ...,
     ) -> ListReadSetsResponseTypeDef:
         """
         Retrieves a list of read sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_read_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_read_sets)
         """
 
     async def list_reference_import_jobs(
         self,
         *,
         referenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ImportReferenceFilterTypeDef = ...
+        filter: ImportReferenceFilterTypeDef = ...,
     ) -> ListReferenceImportJobsResponseTypeDef:
         """
         Retrieves a list of reference import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_reference_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_reference_import_jobs)
         """
 
     async def list_reference_stores(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ReferenceStoreFilterTypeDef = ...
+        filter: ReferenceStoreFilterTypeDef = ...,
     ) -> ListReferenceStoresResponseTypeDef:
         """
         Retrieves a list of reference stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_reference_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_reference_stores)
         """
 
     async def list_references(
         self,
         *,
         referenceStoreId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: ReferenceFilterTypeDef = ...
+        filter: ReferenceFilterTypeDef = ...,
     ) -> ListReferencesResponseTypeDef:
         """
         Retrieves a list of references.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_references)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_references)
         """
@@ -940,15 +940,15 @@
 
     async def list_run_tasks(
         self,
         *,
         id: str,
         status: TaskStatusType = ...,
         startingToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListRunTasksResponseTypeDef:
         """
         Retrieves a list of tasks for a run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_run_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_run_tasks)
         """
@@ -956,44 +956,44 @@
     async def list_runs(
         self,
         *,
         name: str = ...,
         runGroupId: str = ...,
         startingToken: str = ...,
         maxResults: int = ...,
-        status: RunStatusType = ...
+        status: RunStatusType = ...,
     ) -> ListRunsResponseTypeDef:
         """
         Retrieves a list of runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_runs)
         """
 
     async def list_sequence_stores(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        filter: SequenceStoreFilterTypeDef = ...
+        filter: SequenceStoreFilterTypeDef = ...,
     ) -> ListSequenceStoresResponseTypeDef:
         """
         Retrieves a list of sequence stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_sequence_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_sequence_stores)
         """
 
     async def list_shares(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         filter: FilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListSharesResponseTypeDef:
         """
         Lists all shares associated with an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_shares)
         """
@@ -1010,45 +1010,45 @@
 
     async def list_variant_import_jobs(
         self,
         *,
         maxResults: int = ...,
         ids: Sequence[str] = ...,
         nextToken: str = ...,
-        filter: ListVariantImportJobsFilterTypeDef = ...
+        filter: ListVariantImportJobsFilterTypeDef = ...,
     ) -> ListVariantImportJobsResponseTypeDef:
         """
         Retrieves a list of variant import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_variant_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_variant_import_jobs)
         """
 
     async def list_variant_stores(
         self,
         *,
         maxResults: int = ...,
         ids: Sequence[str] = ...,
         nextToken: str = ...,
-        filter: ListVariantStoresFilterTypeDef = ...
+        filter: ListVariantStoresFilterTypeDef = ...,
     ) -> ListVariantStoresResponseTypeDef:
         """
         Retrieves a list of variant stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_variant_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_variant_stores)
         """
 
     async def list_workflows(
         self,
         *,
         type: WorkflowTypeType = ...,
         name: str = ...,
         startingToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListWorkflowsResponseTypeDef:
         """
         Retrieves a list of workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#list_workflows)
         """
@@ -1058,29 +1058,29 @@
         *,
         destinationName: str,
         roleArn: str,
         items: Sequence[AnnotationImportItemSourceTypeDef],
         versionName: str = ...,
         formatOptions: FormatOptionsTypeDef = ...,
         runLeftNormalization: bool = ...,
-        annotationFields: Mapping[str, str] = ...
+        annotationFields: Mapping[str, str] = ...,
     ) -> StartAnnotationImportResponseTypeDef:
         """
         Starts an annotation import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_annotation_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_annotation_import_job)
         """
 
     async def start_read_set_activation_job(
         self,
         *,
         sequenceStoreId: str,
         sources: Sequence[StartReadSetActivationJobSourceItemTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartReadSetActivationJobResponseTypeDef:
         """
         Activates an archived read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_activation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_read_set_activation_job)
         """
@@ -1088,45 +1088,45 @@
     async def start_read_set_export_job(
         self,
         *,
         sequenceStoreId: str,
         destination: str,
         roleArn: str,
         sources: Sequence[ExportReadSetTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartReadSetExportJobResponseTypeDef:
         """
         Exports a read set to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_read_set_export_job)
         """
 
     async def start_read_set_import_job(
         self,
         *,
         sequenceStoreId: str,
         roleArn: str,
         sources: Sequence[StartReadSetImportJobSourceItemTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartReadSetImportJobResponseTypeDef:
         """
         Starts a read set import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_read_set_import_job)
         """
 
     async def start_reference_import_job(
         self,
         *,
         referenceStoreId: str,
         roleArn: str,
         sources: Sequence[StartReferenceImportJobSourceItemTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartReferenceImportJobResponseTypeDef:
         """
         Starts a reference import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_reference_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_reference_import_job)
         """
@@ -1143,15 +1143,15 @@
         runGroupId: str = ...,
         priority: int = ...,
         parameters: Mapping[str, Any] = ...,
         storageCapacity: int = ...,
         outputUri: str = ...,
         logLevel: RunLogLevelType = ...,
         tags: Mapping[str, str] = ...,
-        retentionMode: RunRetentionModeType = ...
+        retentionMode: RunRetentionModeType = ...,
     ) -> StartRunResponseTypeDef:
         """
         Starts a workflow run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_run)
         """
@@ -1159,15 +1159,15 @@
     async def start_variant_import_job(
         self,
         *,
         destinationName: str,
         roleArn: str,
         items: Sequence[VariantImportItemSourceTypeDef],
         runLeftNormalization: bool = ...,
-        annotationFields: Mapping[str, str] = ...
+        annotationFields: Mapping[str, str] = ...,
     ) -> StartVariantImportResponseTypeDef:
         """
         Starts a variant import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_variant_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#start_variant_import_job)
         """
@@ -1212,15 +1212,15 @@
         self,
         *,
         id: str,
         name: str = ...,
         maxCpus: int = ...,
         maxRuns: int = ...,
         maxDuration: int = ...,
-        maxGpus: int = ...
+        maxGpus: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a run group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.update_run_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#update_run_group)
         """
@@ -1248,15 +1248,15 @@
     async def upload_read_set_part(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         partNumber: int,
-        payload: BlobTypeDef
+        payload: BlobTypeDef,
     ) -> UploadReadSetPartResponseTypeDef:
         """
         This operation uploads a specific part of a read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.upload_read_set_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#upload_read_set_part)
         """
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/literals.py` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/literals.py`

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
     "AcceleratorsType",
     "AnnotationImportJobCreatedWaiterName",
     "AnnotationStoreCreatedWaiterName",
     "AnnotationStoreDeletedWaiterName",
     "AnnotationStoreVersionCreatedWaiterName",
     "AnnotationStoreVersionDeletedWaiterName",
@@ -98,15 +97,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AcceleratorsType = Literal["GPU"]
 AnnotationImportJobCreatedWaiterName = Literal["annotation_import_job_created"]
 AnnotationStoreCreatedWaiterName = Literal["annotation_store_created"]
 AnnotationStoreDeletedWaiterName = Literal["annotation_store_deleted"]
 AnnotationStoreVersionCreatedWaiterName = Literal["annotation_store_version_created"]
 AnnotationStoreVersionDeletedWaiterName = Literal["annotation_store_version_deleted"]
 AnnotationTypeType = Literal[
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/literals.pyi` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/paginator.py` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -129,389 +129,367 @@
     "ListSequenceStoresPaginator",
     "ListSharesPaginator",
     "ListVariantImportJobsPaginator",
     "ListVariantStoresPaginator",
     "ListWorkflowsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAnnotationImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationImportJobsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnnotationImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationimportjobspaginator)
         """
 
-
 class ListAnnotationStoreVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStoreVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstoreversionspaginator)
     """
 
     def paginate(
         self,
         *,
         name: str,
         filter: ListAnnotationStoreVersionsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnnotationStoreVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStoreVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstoreversionspaginator)
         """
 
-
 class ListAnnotationStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstorespaginator)
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationStoresFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnnotationStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstorespaginator)
         """
 
-
 class ListMultipartReadSetUploadsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listmultipartreadsetuploadspaginator)
     """
 
     def paginate(
         self, *, sequenceStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMultipartReadSetUploadsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listmultipartreadsetuploadspaginator)
         """
 
-
 class ListReadSetActivationJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetActivationJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetactivationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ActivateReadSetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetActivationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetActivationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetactivationjobspaginator)
         """
 
-
 class ListReadSetExportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetExportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ExportReadSetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetexportjobspaginator)
         """
 
-
 class ListReadSetImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ImportReadSetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetimportjobspaginator)
         """
 
-
 class ListReadSetUploadPartsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetUploadParts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetuploadpartspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         filter: ReadSetUploadPartListFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetUploadPartsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetUploadParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetuploadpartspaginator)
         """
 
-
 class ListReadSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ReadSetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetspaginator)
         """
 
-
 class ListReferenceImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferenceimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ImportReferenceFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReferenceImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferenceimportjobspaginator)
         """
 
-
 class ListReferenceStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ReferenceStoreFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReferenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencestorespaginator)
         """
 
-
 class ListReferencesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferences)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencespaginator)
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ReferenceFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencespaginator)
         """
 
-
 class ListRunGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrungroupspaginator)
     """
 
     def paginate(
         self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRunGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrungroupspaginator)
         """
 
-
 class ListRunTasksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listruntaskspaginator)
     """
 
     def paginate(
         self,
         *,
         id: str,
         status: TaskStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRunTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listruntaskspaginator)
         """
 
-
 class ListRunsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRuns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrunspaginator)
     """
 
     def paginate(
         self,
         *,
         name: str = ...,
         runGroupId: str = ...,
         status: RunStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrunspaginator)
         """
 
-
 class ListSequenceStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListSequenceStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsequencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: SequenceStoreFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSequenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListSequenceStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsequencestorespaginator)
         """
 
-
 class ListSharesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListShares)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsharespaginator)
     """
 
     def paginate(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         filter: FilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsharespaginator)
         """
 
-
 class ListVariantImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantImportJobsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVariantImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantimportjobspaginator)
         """
 
-
 class ListVariantStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantstorespaginator)
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantStoresFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVariantStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantstorespaginator)
         """
 
-
 class ListWorkflowsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listworkflowspaginator)
     """
 
     def paginate(
         self,
         *,
         type: WorkflowTypeType = ...,
         name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/paginator.pyi` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,365 +131,386 @@
     "ListVariantImportJobsPaginator",
     "ListVariantStoresPaginator",
     "ListWorkflowsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAnnotationImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationImportJobsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnnotationImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationimportjobspaginator)
         """
 
+
 class ListAnnotationStoreVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStoreVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstoreversionspaginator)
     """
 
     def paginate(
         self,
         *,
         name: str,
         filter: ListAnnotationStoreVersionsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnnotationStoreVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStoreVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstoreversionspaginator)
         """
 
+
 class ListAnnotationStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstorespaginator)
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationStoresFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnnotationStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstorespaginator)
         """
 
+
 class ListMultipartReadSetUploadsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listmultipartreadsetuploadspaginator)
     """
 
     def paginate(
         self, *, sequenceStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMultipartReadSetUploadsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listmultipartreadsetuploadspaginator)
         """
 
+
 class ListReadSetActivationJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetActivationJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetactivationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ActivateReadSetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetActivationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetActivationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetactivationjobspaginator)
         """
 
+
 class ListReadSetExportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetExportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ExportReadSetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetexportjobspaginator)
         """
 
+
 class ListReadSetImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ImportReadSetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetimportjobspaginator)
         """
 
+
 class ListReadSetUploadPartsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetUploadParts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetuploadpartspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         filter: ReadSetUploadPartListFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetUploadPartsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetUploadParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetuploadpartspaginator)
         """
 
+
 class ListReadSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetspaginator)
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ReadSetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReadSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetspaginator)
         """
 
+
 class ListReferenceImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferenceimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ImportReferenceFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReferenceImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferenceimportjobspaginator)
         """
 
+
 class ListReferenceStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ReferenceStoreFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReferenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencestorespaginator)
         """
 
+
 class ListReferencesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferences)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencespaginator)
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ReferenceFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencespaginator)
         """
 
+
 class ListRunGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrungroupspaginator)
     """
 
     def paginate(
         self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRunGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrungroupspaginator)
         """
 
+
 class ListRunTasksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listruntaskspaginator)
     """
 
     def paginate(
         self,
         *,
         id: str,
         status: TaskStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRunTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listruntaskspaginator)
         """
 
+
 class ListRunsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRuns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrunspaginator)
     """
 
     def paginate(
         self,
         *,
         name: str = ...,
         runGroupId: str = ...,
         status: RunStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrunspaginator)
         """
 
+
 class ListSequenceStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListSequenceStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsequencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: SequenceStoreFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSequenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListSequenceStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsequencestorespaginator)
         """
 
+
 class ListSharesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListShares)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsharespaginator)
     """
 
     def paginate(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         filter: FilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsharespaginator)
         """
 
+
 class ListVariantImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantImportJobsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVariantImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantimportjobspaginator)
         """
 
+
 class ListVariantStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantstorespaginator)
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantStoresFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVariantStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantstorespaginator)
         """
 
+
 class ListWorkflowsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listworkflowspaginator)
     """
 
     def paginate(
         self,
         *,
         type: WorkflowTypeType = ...,
         name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/type_defs.py` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     "AcceptShareRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TimestampTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/type_defs.pyi` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/waiter.py` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 from .type_defs import WaiterConfigTypeDef
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnnotationImportJobCreatedWaiter",
     "AnnotationStoreCreatedWaiter",
     "AnnotationStoreDeletedWaiter",
     "AnnotationStoreVersionCreatedWaiter",
     "AnnotationStoreVersionDeletedWaiter",
     "ReadSetActivationJobCompletedWaiter",
@@ -224,15 +223,15 @@
     """
 
     async def wait(
         self,
         *,
         id: str,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.RunCompleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/waiters/#runcompletedwaiter)
         """
 
 
@@ -243,15 +242,15 @@
     """
 
     async def wait(
         self,
         *,
         id: str,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.RunRunning.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/waiters/#runrunningwaiter)
         """
 
 
@@ -328,13 +327,13 @@
 
     async def wait(
         self,
         *,
         id: str,
         type: WorkflowTypeType = ...,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.WorkflowActive.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/waiters/#workflowactivewaiter)
         """
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics/waiter.pyi` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     """
 
     async def wait(
         self,
         *,
         id: str,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.RunCompleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/waiters/#runcompletedwaiter)
         """
 
 class RunRunningWaiter(AIOWaiter):
@@ -231,15 +231,15 @@
     """
 
     async def wait(
         self,
         *,
         id: str,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.RunRunning.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/waiters/#runrunningwaiter)
         """
 
 class TaskCompletedWaiter(AIOWaiter):
@@ -310,13 +310,13 @@
 
     async def wait(
         self,
         *,
         id: str,
         type: WorkflowTypeType = ...,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.WorkflowActive.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/waiters/#workflowactivewaiter)
         """
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/PKG-INFO` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-omics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Omics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Omics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/
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
 
 <a id="types-aiobotocore-omics"></a>
 
 # types-aiobotocore-omics
 
 [![PyPI - types-aiobotocore-omics](https://img.shields.io/pypi/v/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Omics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[aiobotocore.Omics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [types-aiobotocore-omics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-omics-2.9.0/types_aiobotocore_omics.egg-info/SOURCES.txt` & `types-aiobotocore-omics-2.9.1/types_aiobotocore_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

