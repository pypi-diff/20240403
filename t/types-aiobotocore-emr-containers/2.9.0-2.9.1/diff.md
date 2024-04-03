# Comparing `tmp/types-aiobotocore-emr-containers-2.9.0.tar.gz` & `tmp/types-aiobotocore-emr-containers-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-containers-2.9.0.tar", last modified: Wed Dec 13 19:59:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-containers-2.9.1.tar", last modified: Thu Jan 18 01:20:40 2024, max compression
```

## Comparing `types-aiobotocore-emr-containers-2.9.0.tar` & `types-aiobotocore-emr-containers-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.065756 types-aiobotocore-emr-containers-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13857 2023-12-13 19:59:16.065756 types-aiobotocore-emr-containers-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:16.065756 types-aiobotocore-emr-containers-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.061756 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2023-12-13 19:45:58.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19923 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2023-12-13 19:45:58.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2023-12-13 19:45:58.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2023-12-13 19:45:58.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2023-12-13 19:45:58.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28162 2023-12-13 19:45:58.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28161 2023-12-13 19:45:58.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:56.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.061756 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13857 2023-12-13 19:59:16.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:59:16.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:16.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:16.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:16.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:59:16.000000 types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.797342 types-aiobotocore-emr-containers-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:51.000000 types-aiobotocore-emr-containers-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-01-18 01:20:40.797342 types-aiobotocore-emr-containers-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-01-18 01:07:51.000000 types-aiobotocore-emr-containers-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:40.797342 types-aiobotocore-emr-containers-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-18 01:07:51.000000 types-aiobotocore-emr-containers-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.793342 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-01-18 01:07:51.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-01-18 01:07:51.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:07:51.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19935 2024-01-18 01:07:52.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19932 2024-01-18 01:07:52.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-01-18 01:07:52.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-01-18 01:07:52.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-01-18 01:07:52.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-01-18 01:07:52.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:51.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28161 2024-01-18 01:07:52.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28161 2024-01-18 01:07:52.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:51.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.797342 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-01-18 01:20:40.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:20:40.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:40.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:40.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:40.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:20:40.000000 types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/LICENSE` & `types-aiobotocore-emr-containers-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-emr-containers-2.9.0/PKG-INFO` & `types-aiobotocore-emr-containers-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-containers
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EMRContainers 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EMRContainers 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
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
 
 <a id="types-aiobotocore-emr-containers"></a>
 
 # types-aiobotocore-emr-containers
 
 [![PyPI - types-aiobotocore-emr-containers](https://img.shields.io/pypi/v/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-containers)](https://pepy.tech/project/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [types-aiobotocore-emr-containers docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/README.md` & `types-aiobotocore-emr-containers-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-containers)](https://pepy.tech/project/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [types-aiobotocore-emr-containers docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/setup.py` & `types-aiobotocore-emr-containers-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr-containers",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EMRContainers 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.EMRContainers 2.9.1 service generated with"
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
     keywords="aiobotocore emr-containers type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_emr_containers": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/__init__.py` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
     ListVirtualClustersPaginator,
 )
 
 Client = EMRContainersClient
 
-
 __all__ = (
     "Client",
     "EMRContainersClient",
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
     "ListVirtualClustersPaginator",
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/__init__.pyi` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/__main__.py` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EMRContainers 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EMRContainers 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
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

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/client.py` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EMRContainersClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -126,15 +125,15 @@
     async def create_job_template(
         self,
         *,
         name: str,
         clientToken: str,
         jobTemplateData: JobTemplateDataTypeDef,
         tags: Mapping[str, str] = ...,
-        kmsKeyArn: str = ...
+        kmsKeyArn: str = ...,
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_job_template)
         """
@@ -146,30 +145,30 @@
         virtualClusterId: str,
         type: str,
         releaseLabel: str,
         executionRoleArn: str,
         clientToken: str,
         certificateArn: str = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateManagedEndpointResponseTypeDef:
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_managed_endpoint)
         """
 
     async def create_virtual_cluster(
         self,
         *,
         name: str,
         containerProvider: ContainerProviderTypeDef,
         clientToken: str,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateVirtualClusterResponseTypeDef:
         """
         Creates a virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_virtual_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_virtual_cluster)
         """
@@ -255,15 +254,15 @@
         *,
         endpointIdentifier: str,
         virtualClusterIdentifier: str,
         executionRoleArn: str,
         credentialType: str,
         durationInSeconds: int = ...,
         logContext: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> GetManagedEndpointSessionCredentialsResponseTypeDef:
         """
         Generate a session token to connect to a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_managed_endpoint_session_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_managed_endpoint_session_credentials)
         """
@@ -273,30 +272,30 @@
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_job_runs)
         """
 
     async def list_job_templates(
         self,
         *,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListJobTemplatesResponseTypeDef:
         """
         Lists job templates based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_job_templates)
         """
@@ -306,15 +305,15 @@
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListManagedEndpointsResponseTypeDef:
         """
         Lists managed endpoints based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_managed_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_managed_endpoints)
         """
@@ -334,15 +333,15 @@
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListVirtualClustersResponseTypeDef:
         """
         Lists information about the specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_virtual_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_virtual_clusters)
         """
@@ -356,15 +355,15 @@
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
         jobDriver: JobDriverTypeDef = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
         jobTemplateParameters: Mapping[str, str] = ...,
-        retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
+        retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...,
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.start_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#start_job_run)
         """
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/client.pyi` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     async def create_job_template(
         self,
         *,
         name: str,
         clientToken: str,
         jobTemplateData: JobTemplateDataTypeDef,
         tags: Mapping[str, str] = ...,
-        kmsKeyArn: str = ...
+        kmsKeyArn: str = ...,
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_job_template)
         """
@@ -142,30 +142,30 @@
         virtualClusterId: str,
         type: str,
         releaseLabel: str,
         executionRoleArn: str,
         clientToken: str,
         certificateArn: str = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateManagedEndpointResponseTypeDef:
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_managed_endpoint)
         """
 
     async def create_virtual_cluster(
         self,
         *,
         name: str,
         containerProvider: ContainerProviderTypeDef,
         clientToken: str,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateVirtualClusterResponseTypeDef:
         """
         Creates a virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_virtual_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_virtual_cluster)
         """
@@ -251,15 +251,15 @@
         *,
         endpointIdentifier: str,
         virtualClusterIdentifier: str,
         executionRoleArn: str,
         credentialType: str,
         durationInSeconds: int = ...,
         logContext: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> GetManagedEndpointSessionCredentialsResponseTypeDef:
         """
         Generate a session token to connect to a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_managed_endpoint_session_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_managed_endpoint_session_credentials)
         """
@@ -269,30 +269,30 @@
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_job_runs)
         """
 
     async def list_job_templates(
         self,
         *,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListJobTemplatesResponseTypeDef:
         """
         Lists job templates based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_job_templates)
         """
@@ -302,15 +302,15 @@
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListManagedEndpointsResponseTypeDef:
         """
         Lists managed endpoints based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_managed_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_managed_endpoints)
         """
@@ -330,15 +330,15 @@
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListVirtualClustersResponseTypeDef:
         """
         Lists information about the specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_virtual_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_virtual_clusters)
         """
@@ -352,15 +352,15 @@
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
         jobDriver: JobDriverTypeDef = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
         jobTemplateParameters: Mapping[str, str] = ...,
-        retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
+        retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...,
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.start_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#start_job_run)
         """
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/literals.py` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/literals.py`

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
     "ContainerProviderTypeType",
     "EndpointStateType",
     "FailureReasonType",
     "JobRunStateType",
     "ListJobRunsPaginatorName",
     "ListJobTemplatesPaginatorName",
@@ -35,15 +34,14 @@
     "EMRContainersServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ContainerProviderTypeType = Literal["EKS"]
 EndpointStateType = Literal[
     "ACTIVE", "CREATING", "TERMINATED", "TERMINATED_WITH_ERRORS", "TERMINATING"
 ]
 FailureReasonType = Literal[
     "CLUSTER_UNAVAILABLE", "INTERNAL_ERROR", "USER_ERROR", "VALIDATION_ERROR"
 ]
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/literals.pyi` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/paginator.py` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,23 +44,21 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
     "ListVirtualClustersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -77,15 +75,15 @@
         self,
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobRunsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/paginators/#listjobrunspaginator)
         """
 
 
@@ -96,15 +94,15 @@
     """
 
     def paginate(
         self,
         *,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobTemplatesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -118,15 +116,15 @@
         self,
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListManagedEndpointsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
 
@@ -140,13 +138,13 @@
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/paginator.pyi` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self,
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobRunsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/paginators/#listjobrunspaginator)
         """
 
 class ListJobTemplatesPaginator(AioPaginator):
@@ -91,15 +91,15 @@
     """
 
     def paginate(
         self,
         *,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobTemplatesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/paginators/#listjobtemplatespaginator)
         """
 
 class ListManagedEndpointsPaginator(AioPaginator):
@@ -112,15 +112,15 @@
         self,
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListManagedEndpointsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
 class ListVirtualClustersPaginator(AioPaginator):
@@ -133,13 +133,13 @@
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/type_defs.py` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CertificateTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
     "ConfigurationPaginatorTypeDef",
     "ConfigurationTypeDef",
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers/type_defs.pyi` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/PKG-INFO` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-containers
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EMRContainers 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EMRContainers 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
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
 
 <a id="types-aiobotocore-emr-containers"></a>
 
 # types-aiobotocore-emr-containers
 
 [![PyPI - types-aiobotocore-emr-containers](https://img.shields.io/pypi/v/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-containers)](https://pepy.tech/project/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [types-aiobotocore-emr-containers docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-containers-2.9.0/types_aiobotocore_emr_containers.egg-info/SOURCES.txt` & `types-aiobotocore-emr-containers-2.9.1/types_aiobotocore_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

