# Comparing `tmp/types-aiobotocore-proton-2.9.0.tar.gz` & `tmp/types-aiobotocore-proton-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-proton-2.9.0.tar", last modified: Wed Dec 13 20:00:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-proton-2.9.1.tar", last modified: Thu Jan 18 01:21:32 2024, max compression
```

## Comparing `types-aiobotocore-proton-2.9.0.tar` & `types-aiobotocore-proton-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.977298 types-aiobotocore-proton-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:57.000000 types-aiobotocore-proton-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18762 2023-12-13 20:00:11.977298 types-aiobotocore-proton-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17203 2023-12-13 19:51:57.000000 types-aiobotocore-proton-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:11.977298 types-aiobotocore-proton-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:51:57.000000 types-aiobotocore-proton-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.977298 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2023-12-13 19:51:57.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2023-12-13 19:51:57.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:51:57.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78225 2023-12-13 19:51:58.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    78221 2023-12-13 19:51:58.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16426 2023-12-13 19:51:58.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16424 2023-12-13 19:51:58.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27544 2023-12-13 19:51:58.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27521 2023-12-13 19:51:58.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:57.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    83973 2023-12-13 19:52:02.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    83972 2023-12-13 19:52:01.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:57.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2023-12-13 19:51:58.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2023-12-13 19:51:58.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.977298 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18762 2023-12-13 20:00:11.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-13 20:00:11.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:11.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:11.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:11.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 20:00:11.000000 types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.073109 types-aiobotocore-proton-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18782 2024-01-18 01:21:32.073109 types-aiobotocore-proton-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:32.073109 types-aiobotocore-proton-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.069109 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78258 2024-01-18 01:13:35.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78255 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-01-18 01:13:35.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-01-18 01:13:35.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-01-18 01:13:35.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27534 2024-01-18 01:13:35.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    83972 2024-01-18 01:13:37.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83972 2024-01-18 01:13:36.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:34.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-01-18 01:13:35.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-01-18 01:13:35.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.073109 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18782 2024-01-18 01:21:32.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-18 01:21:32.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:32.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:32.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:32.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:21:32.000000 types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-proton-2.9.0/LICENSE` & `types-aiobotocore-proton-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-proton-2.9.0/PKG-INFO` & `types-aiobotocore-proton-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-proton
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Proton 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Proton 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/
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
 
 <a id="types-aiobotocore-proton"></a>
 
 # types-aiobotocore-proton
 
 [![PyPI - types-aiobotocore-proton](https://img.shields.io/pypi/v/types-aiobotocore-proton.svg?color=blue)](https://pypi.org/project/types-aiobotocore-proton)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-proton.svg?color=blue)](https://pypi.org/project/types-aiobotocore-proton)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-proton)](https://pepy.tech/project/types-aiobotocore-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Proton 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[aiobotocore.Proton 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [types-aiobotocore-proton docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-proton-2.9.0/README.md` & `types-aiobotocore-proton-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-proton.svg?color=blue)](https://pypi.org/project/types-aiobotocore-proton)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-proton)](https://pepy.tech/project/types-aiobotocore-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Proton 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[aiobotocore.Proton 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [types-aiobotocore-proton docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-proton-2.9.0/setup.py` & `types-aiobotocore-proton-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-proton",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_proton"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Proton 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Proton 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore proton type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_proton": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/__init__.py` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
     ServicePipelineDeployedWaiter,
     ServiceTemplateVersionRegisteredWaiter,
     ServiceUpdatedWaiter,
 )
 
 Client = ProtonClient
 
-
 __all__ = (
     "Client",
     "ComponentDeletedWaiter",
     "ComponentDeployedWaiter",
     "EnvironmentDeployedWaiter",
     "EnvironmentTemplateVersionRegisteredWaiter",
     "ListComponentOutputsPaginator",
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/__init__.pyi` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/__main__.py` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Proton 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Proton 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton\nOther"
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

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/client.py` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ProtonClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -290,15 +289,15 @@
         templateFile: str,
         clientToken: str = ...,
         description: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateComponentOutputTypeDef:
         """
         Create an Proton component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_component)
         """
@@ -313,15 +312,15 @@
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Deploy a new environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_environment)
         """
@@ -331,15 +330,15 @@
         *,
         environmentName: str,
         managementAccountId: str,
         clientToken: str = ...,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEnvironmentAccountConnectionOutputTypeDef:
         """
         Create an environment account connection in an environment account so that
         environment infrastructure resources can be provisioned in the environment
         account from a management
         account.
 
@@ -351,15 +350,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         provisioning: Literal["CUSTOMER_MANAGED"] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEnvironmentTemplateOutputTypeDef:
         """
         Create an environment template for Proton.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_environment_template)
         """
@@ -368,15 +367,15 @@
         self,
         *,
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEnvironmentTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_environment_template_version)
         """
@@ -384,15 +383,15 @@
     async def create_repository(
         self,
         *,
         connectionArn: str,
         name: str,
         provider: RepositoryProviderType,
         encryptionKey: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryOutputTypeDef:
         """
         Create and register a link to a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_repository)
         """
@@ -405,15 +404,15 @@
         templateMajorVersion: str,
         templateName: str,
         branchName: str = ...,
         description: str = ...,
         repositoryConnectionArn: str = ...,
         repositoryId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> CreateServiceOutputTypeDef:
         """
         Create an Proton service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service)
         """
@@ -423,15 +422,15 @@
         *,
         name: str,
         serviceName: str,
         spec: str,
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMajorVersion: str = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> CreateServiceInstanceOutputTypeDef:
         """
         Create a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service_instance)
         """
@@ -439,15 +438,15 @@
     async def create_service_sync_config(
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        serviceName: str
+        serviceName: str,
     ) -> CreateServiceSyncConfigOutputTypeDef:
         """
         Create the Proton Ops configuration file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service_sync_config)
         """
@@ -456,15 +455,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         pipelineProvisioning: Literal["CUSTOMER_MANAGED"] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateServiceTemplateOutputTypeDef:
         """
         Create a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service_template)
         """
@@ -475,15 +474,15 @@
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef],
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateServiceTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service_template_version)
         """
@@ -492,15 +491,15 @@
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
-        subdirectory: str = ...
+        subdirectory: str = ...,
     ) -> CreateTemplateSyncConfigOutputTypeDef:
         """
         Set up a template to create new template versions automatically by tracking a
         linked
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)
@@ -658,15 +657,15 @@
     async def get_deployment(
         self,
         *,
         id: str,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
-        serviceName: str = ...
+        serviceName: str = ...,
     ) -> GetDeploymentOutputTypeDef:
         """
         Get detailed data for a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_deployment)
         """
@@ -720,15 +719,15 @@
 
     async def get_repository_sync_status(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        syncType: SyncTypeType
+        syncType: SyncTypeType,
     ) -> GetRepositorySyncStatusOutputTypeDef:
         """
         Get the sync status of a repository used for Proton template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_repository_sync_status)
         """
@@ -850,15 +849,15 @@
     async def list_components(
         self,
         *,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
-        serviceName: str = ...
+        serviceName: str = ...,
     ) -> ListComponentsOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_components)
         """
@@ -867,15 +866,15 @@
         self,
         *,
         componentName: str = ...,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
-        serviceName: str = ...
+        serviceName: str = ...,
     ) -> ListDeploymentsOutputTypeDef:
         """
         List deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_deployments)
         """
@@ -883,15 +882,15 @@
     async def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...
+        statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
     ) -> ListEnvironmentAccountConnectionsOutputTypeDef:
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environment_account_connections)
         """
@@ -918,15 +917,15 @@
 
     async def list_environment_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of an environment template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environment_template_versions)
         """
@@ -942,15 +941,15 @@
         """
 
     async def list_environments(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentsOutputTypeDef:
         """
         List environments with detail data summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environments)
         """
@@ -967,30 +966,30 @@
 
     async def list_repository_sync_definitions(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRepositorySyncDefinitionsOutputTypeDef:
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_repository_sync_definitions)
         """
 
     async def list_service_instance_outputs(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_instance_outputs)
         """
@@ -1009,15 +1008,15 @@
         self,
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListServiceInstancesOutputTypeDef:
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_instances)
         """
@@ -1044,15 +1043,15 @@
 
     async def list_service_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListServiceTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of a service template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_template_versions)
         """
@@ -1090,15 +1089,15 @@
     async def notify_resource_deployment_status_change(
         self,
         *,
         resourceArn: str,
         deploymentId: str = ...,
         outputs: Sequence[OutputTypeDef] = ...,
         status: ResourceDeploymentStatusType = ...,
-        statusMessage: str = ...
+        statusMessage: str = ...,
     ) -> Dict[str, Any]:
         """
         Notify Proton of status changes to a provisioned resource when you use
         self-managed
         provisioning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)
@@ -1135,15 +1134,15 @@
 
     async def update_account_settings(
         self,
         *,
         deletePipelineProvisioningRepository: bool = ...,
         pipelineCodebuildRoleArn: str = ...,
         pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,
-        pipelineServiceRoleArn: str = ...
+        pipelineServiceRoleArn: str = ...,
     ) -> UpdateAccountSettingsOutputTypeDef:
         """
         Update Proton settings that are used for multiple services in the Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)
@@ -1156,15 +1155,15 @@
         deploymentType: ComponentDeploymentUpdateTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
-        templateFile: str = ...
+        templateFile: str = ...,
     ) -> UpdateComponentOutputTypeDef:
         """
         Update a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_component)
         """
@@ -1178,30 +1177,30 @@
         componentRoleArn: str = ...,
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Update an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_environment)
         """
 
     async def update_environment_account_connection(
         self,
         *,
         id: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> UpdateEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, update an environment account connection to use a
         new IAM
         role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)
@@ -1221,15 +1220,15 @@
     async def update_environment_template_version(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         description: str = ...,
-        status: TemplateVersionStatusType = ...
+        status: TemplateVersionStatusType = ...,
     ) -> UpdateEnvironmentTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_environment_template_version)
         """
@@ -1249,15 +1248,15 @@
         *,
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         serviceName: str,
         clientToken: str = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> UpdateServiceInstanceOutputTypeDef:
         """
         Update a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_service_instance)
         """
@@ -1265,15 +1264,15 @@
     async def update_service_pipeline(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         serviceName: str,
         spec: str,
         templateMajorVersion: str = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> UpdateServicePipelineOutputTypeDef:
         """
         Update the service pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_service_pipeline)
         """
@@ -1291,15 +1290,15 @@
     async def update_service_sync_config(
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        serviceName: str
+        serviceName: str,
     ) -> UpdateServiceSyncConfigOutputTypeDef:
         """
         Update the Proton Ops config file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_service_sync_config)
         """
@@ -1319,15 +1318,15 @@
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,
         description: str = ...,
         status: TemplateVersionStatusType = ...,
-        supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...
+        supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...,
     ) -> UpdateServiceTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_service_template_version)
         """
@@ -1336,15 +1335,15 @@
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
-        subdirectory: str = ...
+        subdirectory: str = ...,
     ) -> UpdateTemplateSyncConfigOutputTypeDef:
         """
         Update template sync configuration parameters, except for the `templateName`
         and
         `templateType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/client.pyi` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         templateFile: str,
         clientToken: str = ...,
         description: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateComponentOutputTypeDef:
         """
         Create an Proton component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_component)
         """
@@ -309,15 +309,15 @@
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Deploy a new environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_environment)
         """
@@ -327,15 +327,15 @@
         *,
         environmentName: str,
         managementAccountId: str,
         clientToken: str = ...,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEnvironmentAccountConnectionOutputTypeDef:
         """
         Create an environment account connection in an environment account so that
         environment infrastructure resources can be provisioned in the environment
         account from a management
         account.
 
@@ -347,15 +347,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         provisioning: Literal["CUSTOMER_MANAGED"] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEnvironmentTemplateOutputTypeDef:
         """
         Create an environment template for Proton.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_environment_template)
         """
@@ -364,15 +364,15 @@
         self,
         *,
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEnvironmentTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_environment_template_version)
         """
@@ -380,15 +380,15 @@
     async def create_repository(
         self,
         *,
         connectionArn: str,
         name: str,
         provider: RepositoryProviderType,
         encryptionKey: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryOutputTypeDef:
         """
         Create and register a link to a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_repository)
         """
@@ -401,15 +401,15 @@
         templateMajorVersion: str,
         templateName: str,
         branchName: str = ...,
         description: str = ...,
         repositoryConnectionArn: str = ...,
         repositoryId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> CreateServiceOutputTypeDef:
         """
         Create an Proton service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service)
         """
@@ -419,15 +419,15 @@
         *,
         name: str,
         serviceName: str,
         spec: str,
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMajorVersion: str = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> CreateServiceInstanceOutputTypeDef:
         """
         Create a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service_instance)
         """
@@ -435,15 +435,15 @@
     async def create_service_sync_config(
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        serviceName: str
+        serviceName: str,
     ) -> CreateServiceSyncConfigOutputTypeDef:
         """
         Create the Proton Ops configuration file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service_sync_config)
         """
@@ -452,15 +452,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         pipelineProvisioning: Literal["CUSTOMER_MANAGED"] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateServiceTemplateOutputTypeDef:
         """
         Create a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service_template)
         """
@@ -471,15 +471,15 @@
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef],
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateServiceTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#create_service_template_version)
         """
@@ -488,15 +488,15 @@
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
-        subdirectory: str = ...
+        subdirectory: str = ...,
     ) -> CreateTemplateSyncConfigOutputTypeDef:
         """
         Set up a template to create new template versions automatically by tracking a
         linked
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)
@@ -654,15 +654,15 @@
     async def get_deployment(
         self,
         *,
         id: str,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
-        serviceName: str = ...
+        serviceName: str = ...,
     ) -> GetDeploymentOutputTypeDef:
         """
         Get detailed data for a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_deployment)
         """
@@ -716,15 +716,15 @@
 
     async def get_repository_sync_status(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        syncType: SyncTypeType
+        syncType: SyncTypeType,
     ) -> GetRepositorySyncStatusOutputTypeDef:
         """
         Get the sync status of a repository used for Proton template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_repository_sync_status)
         """
@@ -846,15 +846,15 @@
     async def list_components(
         self,
         *,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
-        serviceName: str = ...
+        serviceName: str = ...,
     ) -> ListComponentsOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_components)
         """
@@ -863,15 +863,15 @@
         self,
         *,
         componentName: str = ...,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
-        serviceName: str = ...
+        serviceName: str = ...,
     ) -> ListDeploymentsOutputTypeDef:
         """
         List deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_deployments)
         """
@@ -879,15 +879,15 @@
     async def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...
+        statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
     ) -> ListEnvironmentAccountConnectionsOutputTypeDef:
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environment_account_connections)
         """
@@ -914,15 +914,15 @@
 
     async def list_environment_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of an environment template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environment_template_versions)
         """
@@ -938,15 +938,15 @@
         """
 
     async def list_environments(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentsOutputTypeDef:
         """
         List environments with detail data summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environments)
         """
@@ -963,30 +963,30 @@
 
     async def list_repository_sync_definitions(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRepositorySyncDefinitionsOutputTypeDef:
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_repository_sync_definitions)
         """
 
     async def list_service_instance_outputs(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_instance_outputs)
         """
@@ -1005,15 +1005,15 @@
         self,
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListServiceInstancesOutputTypeDef:
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_instances)
         """
@@ -1040,15 +1040,15 @@
 
     async def list_service_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListServiceTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of a service template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_template_versions)
         """
@@ -1086,15 +1086,15 @@
     async def notify_resource_deployment_status_change(
         self,
         *,
         resourceArn: str,
         deploymentId: str = ...,
         outputs: Sequence[OutputTypeDef] = ...,
         status: ResourceDeploymentStatusType = ...,
-        statusMessage: str = ...
+        statusMessage: str = ...,
     ) -> Dict[str, Any]:
         """
         Notify Proton of status changes to a provisioned resource when you use
         self-managed
         provisioning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)
@@ -1131,15 +1131,15 @@
 
     async def update_account_settings(
         self,
         *,
         deletePipelineProvisioningRepository: bool = ...,
         pipelineCodebuildRoleArn: str = ...,
         pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,
-        pipelineServiceRoleArn: str = ...
+        pipelineServiceRoleArn: str = ...,
     ) -> UpdateAccountSettingsOutputTypeDef:
         """
         Update Proton settings that are used for multiple services in the Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)
@@ -1152,15 +1152,15 @@
         deploymentType: ComponentDeploymentUpdateTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
-        templateFile: str = ...
+        templateFile: str = ...,
     ) -> UpdateComponentOutputTypeDef:
         """
         Update a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_component)
         """
@@ -1174,30 +1174,30 @@
         componentRoleArn: str = ...,
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Update an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_environment)
         """
 
     async def update_environment_account_connection(
         self,
         *,
         id: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> UpdateEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, update an environment account connection to use a
         new IAM
         role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)
@@ -1217,15 +1217,15 @@
     async def update_environment_template_version(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         description: str = ...,
-        status: TemplateVersionStatusType = ...
+        status: TemplateVersionStatusType = ...,
     ) -> UpdateEnvironmentTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_environment_template_version)
         """
@@ -1245,15 +1245,15 @@
         *,
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         serviceName: str,
         clientToken: str = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> UpdateServiceInstanceOutputTypeDef:
         """
         Update a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_service_instance)
         """
@@ -1261,15 +1261,15 @@
     async def update_service_pipeline(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         serviceName: str,
         spec: str,
         templateMajorVersion: str = ...,
-        templateMinorVersion: str = ...
+        templateMinorVersion: str = ...,
     ) -> UpdateServicePipelineOutputTypeDef:
         """
         Update the service pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_service_pipeline)
         """
@@ -1287,15 +1287,15 @@
     async def update_service_sync_config(
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        serviceName: str
+        serviceName: str,
     ) -> UpdateServiceSyncConfigOutputTypeDef:
         """
         Update the Proton Ops config file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_service_sync_config)
         """
@@ -1315,15 +1315,15 @@
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,
         description: str = ...,
         status: TemplateVersionStatusType = ...,
-        supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...
+        supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...,
     ) -> UpdateServiceTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#update_service_template_version)
         """
@@ -1332,15 +1332,15 @@
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
-        subdirectory: str = ...
+        subdirectory: str = ...,
     ) -> UpdateTemplateSyncConfigOutputTypeDef:
         """
         Update template sync configuration parameters, except for the `templateName`
         and
         `templateType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/literals.py` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/literals.py`

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
     "BlockerStatusType",
     "BlockerTypeType",
     "ComponentDeletedWaiterName",
     "ComponentDeployedWaiterName",
     "ComponentDeploymentUpdateTypeType",
     "DeploymentStatusType",
@@ -78,15 +77,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 BlockerStatusType = Literal["ACTIVE", "RESOLVED"]
 BlockerTypeType = Literal["AUTOMATED"]
 ComponentDeletedWaiterName = Literal["component_deleted"]
 ComponentDeployedWaiterName = Literal["component_deployed"]
 ComponentDeploymentUpdateTypeType = Literal["CURRENT_VERSION", "NONE"]
 DeploymentStatusType = Literal[
     "CANCELLED",
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/literals.pyi` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/paginator.py` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
     "ListServicePipelineProvisionedResourcesPaginator",
     "ListServiceTemplateVersionsPaginator",
     "ListServiceTemplatesPaginator",
     "ListServicesPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -143,15 +142,15 @@
     """
 
     def paginate(
         self,
         *,
         componentName: str,
         deploymentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentoutputspaginator)
         """
 
 
@@ -178,15 +177,15 @@
 
     def paginate(
         self,
         *,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentspaginator)
         """
 
 
@@ -199,15 +198,15 @@
     def paginate(
         self,
         *,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listdeploymentspaginator)
         """
 
 
@@ -219,15 +218,15 @@
 
     def paginate(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentAccountConnectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentaccountconnectionspaginator)
         """
 
 
@@ -238,15 +237,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentName: str,
         deploymentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentoutputspaginator)
         """
 
 
@@ -272,15 +271,15 @@
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmenttemplateversionspaginator)
         """
 
 
@@ -305,15 +304,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentspaginator)
         """
 
 
@@ -340,15 +339,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRepositorySyncDefinitionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listrepositorysyncdefinitionspaginator)
         """
 
 
@@ -360,15 +359,15 @@
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
 
@@ -379,15 +378,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceInstanceProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
         """
 
 
@@ -400,15 +399,15 @@
     def paginate(
         self,
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listserviceinstancespaginator)
         """
 
 
@@ -419,15 +418,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceName: str,
         deploymentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
 
@@ -453,15 +452,15 @@
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listservicetemplateversionspaginator)
         """
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/paginator.pyi` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     """
 
     def paginate(
         self,
         *,
         componentName: str,
         deploymentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentoutputspaginator)
         """
 
 class ListComponentProvisionedResourcesPaginator(AioPaginator):
@@ -173,15 +173,15 @@
 
     def paginate(
         self,
         *,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentspaginator)
         """
 
 class ListDeploymentsPaginator(AioPaginator):
@@ -193,15 +193,15 @@
     def paginate(
         self,
         *,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listdeploymentspaginator)
         """
 
 class ListEnvironmentAccountConnectionsPaginator(AioPaginator):
@@ -212,15 +212,15 @@
 
     def paginate(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentAccountConnectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentaccountconnectionspaginator)
         """
 
 class ListEnvironmentOutputsPaginator(AioPaginator):
@@ -230,15 +230,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentName: str,
         deploymentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentoutputspaginator)
         """
 
 class ListEnvironmentProvisionedResourcesPaginator(AioPaginator):
@@ -262,15 +262,15 @@
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmenttemplateversionspaginator)
         """
 
 class ListEnvironmentTemplatesPaginator(AioPaginator):
@@ -293,15 +293,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentspaginator)
         """
 
 class ListRepositoriesPaginator(AioPaginator):
@@ -326,15 +326,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRepositorySyncDefinitionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listrepositorysyncdefinitionspaginator)
         """
 
 class ListServiceInstanceOutputsPaginator(AioPaginator):
@@ -345,15 +345,15 @@
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
 class ListServiceInstanceProvisionedResourcesPaginator(AioPaginator):
@@ -363,15 +363,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceInstanceProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
         """
 
 class ListServiceInstancesPaginator(AioPaginator):
@@ -383,15 +383,15 @@
     def paginate(
         self,
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listserviceinstancespaginator)
         """
 
 class ListServicePipelineOutputsPaginator(AioPaginator):
@@ -401,15 +401,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceName: str,
         deploymentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
 class ListServicePipelineProvisionedResourcesPaginator(AioPaginator):
@@ -433,15 +433,15 @@
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listservicetemplateversionspaginator)
         """
 
 class ListServiceTemplatesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/type_defs.py` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     "EnvironmentAccountConnectionTypeDef",
     "ResponseMetadataTypeDef",
     "RepositoryBranchTypeDef",
     "CancelComponentDeploymentInputRequestTypeDef",
     "ComponentTypeDef",
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/type_defs.pyi` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/waiter.py` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     async def wait(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.EnvironmentTemplateVersionRegistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/waiters/#environmenttemplateversionregisteredwaiter)
         """
 
 
@@ -178,15 +178,15 @@
 
     async def wait(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.ServiceTemplateVersionRegistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/waiters/#servicetemplateversionregisteredwaiter)
         """
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton/waiter.pyi` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     async def wait(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.EnvironmentTemplateVersionRegistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/waiters/#environmenttemplateversionregisteredwaiter)
         """
 
 class ServiceCreatedWaiter(AIOWaiter):
@@ -169,15 +169,15 @@
 
     async def wait(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.ServiceTemplateVersionRegistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/waiters/#servicetemplateversionregisteredwaiter)
         """
 
 class ServiceUpdatedWaiter(AIOWaiter):
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/PKG-INFO` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-proton
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Proton 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Proton 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/
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
 
 <a id="types-aiobotocore-proton"></a>
 
 # types-aiobotocore-proton
 
 [![PyPI - types-aiobotocore-proton](https://img.shields.io/pypi/v/types-aiobotocore-proton.svg?color=blue)](https://pypi.org/project/types-aiobotocore-proton)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-proton.svg?color=blue)](https://pypi.org/project/types-aiobotocore-proton)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-proton)](https://pepy.tech/project/types-aiobotocore-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Proton 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[aiobotocore.Proton 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [types-aiobotocore-proton docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-proton-2.9.0/types_aiobotocore_proton.egg-info/SOURCES.txt` & `types-aiobotocore-proton-2.9.1/types_aiobotocore_proton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

