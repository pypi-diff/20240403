# Comparing `tmp/types-aiobotocore-vpc-lattice-2.9.0.tar.gz` & `tmp/types-aiobotocore-vpc-lattice-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-vpc-lattice-2.9.0.tar", last modified: Wed Dec 13 20:00:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-vpc-lattice-2.9.1.tar", last modified: Thu Jan 18 01:22:01 2024, max compression
```

## Comparing `types-aiobotocore-vpc-lattice-2.9.0.tar` & `types-aiobotocore-vpc-lattice-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:44.113021 types-aiobotocore-vpc-lattice-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14508 2023-12-13 20:00:44.113021 types-aiobotocore-vpc-lattice-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12930 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:44.113021 types-aiobotocore-vpc-lattice-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:44.109021 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41347 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    41343 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11301 2023-12-13 19:57:35.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11893 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    43081 2023-12-13 19:57:35.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43080 2023-12-13 19:57:35.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:34.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:44.113021 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14508 2023-12-13 20:00:44.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 20:00:44.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:44.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:44.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:44.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 20:00:44.000000 types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:01.236978 types-aiobotocore-vpc-lattice-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-01-18 01:22:01.236978 types-aiobotocore-vpc-lattice-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12930 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:01.236978 types-aiobotocore-vpc-lattice-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:01.232978 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-01-18 01:19:04.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41357 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-01-18 01:19:04.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-01-18 01:19:04.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-01-18 01:19:04.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-01-18 01:19:04.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    43080 2024-01-18 01:19:05.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43080 2024-01-18 01:19:04.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:03.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:01.236978 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-01-18 01:22:01.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-18 01:22:01.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:01.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:01.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:01.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:22:01.000000 types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/LICENSE` & `types-aiobotocore-vpc-lattice-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/PKG-INFO` & `types-aiobotocore-vpc-lattice-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-vpc-lattice
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.VPCLattice 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.VPCLattice 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/
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
 
 <a id="types-aiobotocore-vpc-lattice"></a>
 
 # types-aiobotocore-vpc-lattice
 
 [![PyPI - types-aiobotocore-vpc-lattice](https://img.shields.io/pypi/v/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VPCLattice 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[aiobotocore.VPCLattice 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [types-aiobotocore-vpc-lattice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/README.md` & `types-aiobotocore-vpc-lattice-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VPCLattice 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[aiobotocore.VPCLattice 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [types-aiobotocore-vpc-lattice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/setup.py` & `types-aiobotocore-vpc-lattice-2.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-vpc-lattice",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.VPCLattice 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.VPCLattice 2.9.1 service generated with"
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
     keywords="aiobotocore vpc-lattice type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_vpc_lattice": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/__init__.py` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     ListServicesPaginator,
     ListTargetGroupsPaginator,
     ListTargetsPaginator,
 )
 
 Client = VPCLatticeClient
 
-
 __all__ = (
     "Client",
     "ListAccessLogSubscriptionsPaginator",
     "ListListenersPaginator",
     "ListRulesPaginator",
     "ListServiceNetworkServiceAssociationsPaginator",
     "ListServiceNetworkVpcAssociationsPaginator",
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/__init__.pyi` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/__main__.py` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VPCLattice 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.VPCLattice 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
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

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/client.py` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("VPCLatticeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -158,15 +157,15 @@
 
     async def create_access_log_subscription(
         self,
         *,
         destinationArn: str,
         resourceIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAccessLogSubscriptionResponseTypeDef:
         """
         Enables access logs to be sent to Amazon CloudWatch, Amazon S3, and Amazon
         Kinesis Data
         Firehose.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
@@ -178,15 +177,15 @@
         *,
         defaultAction: RuleActionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateListenerResponseTypeDef:
         """
         Creates a listener for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_listener)
         """
@@ -197,15 +196,15 @@
         action: RuleActionTypeDef,
         listenerIdentifier: str,
         match: RuleMatchTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a listener rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_rule)
         """
@@ -214,45 +213,45 @@
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         certificateArn: str = ...,
         clientToken: str = ...,
         customDomainName: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_service)
         """
 
     async def create_service_network(
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkResponseTypeDef:
         """
         Creates a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_service_network)
         """
 
     async def create_service_network_service_association(
         self,
         *,
         serviceIdentifier: str,
         serviceNetworkIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkServiceAssociationResponseTypeDef:
         """
         Associates a service with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_service_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_service_network_service_association)
         """
@@ -260,15 +259,15 @@
     async def create_service_network_vpc_association(
         self,
         *,
         serviceNetworkIdentifier: str,
         vpcIdentifier: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkVpcAssociationResponseTypeDef:
         """
         Associates a VPC with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_vpc_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_service_network_vpc_association)
         """
@@ -276,15 +275,15 @@
     async def create_target_group(
         self,
         *,
         name: str,
         type: TargetGroupTypeType,
         clientToken: str = ...,
         config: TargetGroupConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTargetGroupResponseTypeDef:
         """
         Creates a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_target_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_target_group)
         """
@@ -526,45 +525,45 @@
 
     async def list_rules(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRulesResponseTypeDef:
         """
         Lists the rules for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_rules)
         """
 
     async def list_service_network_service_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceIdentifier: str = ...,
-        serviceNetworkIdentifier: str = ...
+        serviceNetworkIdentifier: str = ...,
     ) -> ListServiceNetworkServiceAssociationsResponseTypeDef:
         """
         Lists the associations between the service network and the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_service_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_service_network_service_associations)
         """
 
     async def list_service_network_vpc_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceNetworkIdentifier: str = ...,
-        vpcIdentifier: str = ...
+        vpcIdentifier: str = ...,
     ) -> ListServiceNetworkVpcAssociationsResponseTypeDef:
         """
         Lists the service network and VPC associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_vpc_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_service_network_vpc_associations)
         """
@@ -604,30 +603,30 @@
 
     async def list_target_groups(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         targetGroupType: TargetGroupTypeType = ...,
-        vpcIdentifier: str = ...
+        vpcIdentifier: str = ...,
     ) -> ListTargetGroupsResponseTypeDef:
         """
         Lists your target groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_target_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_target_groups)
         """
 
     async def list_targets(
         self,
         *,
         targetGroupIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        targets: Sequence[TargetTypeDef] = ...
+        targets: Sequence[TargetTypeDef] = ...,
     ) -> ListTargetsResponseTypeDef:
         """
         Lists the targets for the target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_targets)
         """
@@ -700,15 +699,15 @@
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
         action: RuleActionTypeDef = ...,
         match: RuleMatchTypeDef = ...,
-        priority: int = ...
+        priority: int = ...,
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_rule)
         """
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/client.pyi` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
     async def create_access_log_subscription(
         self,
         *,
         destinationArn: str,
         resourceIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAccessLogSubscriptionResponseTypeDef:
         """
         Enables access logs to be sent to Amazon CloudWatch, Amazon S3, and Amazon
         Kinesis Data
         Firehose.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
@@ -174,15 +174,15 @@
         *,
         defaultAction: RuleActionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateListenerResponseTypeDef:
         """
         Creates a listener for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_listener)
         """
@@ -193,15 +193,15 @@
         action: RuleActionTypeDef,
         listenerIdentifier: str,
         match: RuleMatchTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a listener rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_rule)
         """
@@ -210,45 +210,45 @@
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         certificateArn: str = ...,
         clientToken: str = ...,
         customDomainName: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_service)
         """
 
     async def create_service_network(
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkResponseTypeDef:
         """
         Creates a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_service_network)
         """
 
     async def create_service_network_service_association(
         self,
         *,
         serviceIdentifier: str,
         serviceNetworkIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkServiceAssociationResponseTypeDef:
         """
         Associates a service with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_service_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_service_network_service_association)
         """
@@ -256,15 +256,15 @@
     async def create_service_network_vpc_association(
         self,
         *,
         serviceNetworkIdentifier: str,
         vpcIdentifier: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkVpcAssociationResponseTypeDef:
         """
         Associates a VPC with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_vpc_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_service_network_vpc_association)
         """
@@ -272,15 +272,15 @@
     async def create_target_group(
         self,
         *,
         name: str,
         type: TargetGroupTypeType,
         clientToken: str = ...,
         config: TargetGroupConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTargetGroupResponseTypeDef:
         """
         Creates a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_target_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_target_group)
         """
@@ -522,45 +522,45 @@
 
     async def list_rules(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRulesResponseTypeDef:
         """
         Lists the rules for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_rules)
         """
 
     async def list_service_network_service_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceIdentifier: str = ...,
-        serviceNetworkIdentifier: str = ...
+        serviceNetworkIdentifier: str = ...,
     ) -> ListServiceNetworkServiceAssociationsResponseTypeDef:
         """
         Lists the associations between the service network and the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_service_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_service_network_service_associations)
         """
 
     async def list_service_network_vpc_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceNetworkIdentifier: str = ...,
-        vpcIdentifier: str = ...
+        vpcIdentifier: str = ...,
     ) -> ListServiceNetworkVpcAssociationsResponseTypeDef:
         """
         Lists the service network and VPC associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_vpc_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_service_network_vpc_associations)
         """
@@ -600,30 +600,30 @@
 
     async def list_target_groups(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         targetGroupType: TargetGroupTypeType = ...,
-        vpcIdentifier: str = ...
+        vpcIdentifier: str = ...,
     ) -> ListTargetGroupsResponseTypeDef:
         """
         Lists your target groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_target_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_target_groups)
         """
 
     async def list_targets(
         self,
         *,
         targetGroupIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        targets: Sequence[TargetTypeDef] = ...
+        targets: Sequence[TargetTypeDef] = ...,
     ) -> ListTargetsResponseTypeDef:
         """
         Lists the targets for the target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#list_targets)
         """
@@ -696,15 +696,15 @@
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
         action: RuleActionTypeDef = ...,
         match: RuleMatchTypeDef = ...,
-        priority: int = ...
+        priority: int = ...,
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_rule)
         """
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/literals.py` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/literals.py`

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
     "AuthPolicyStateType",
     "AuthTypeType",
     "HealthCheckProtocolVersionType",
     "IpAddressTypeType",
     "LambdaEventStructureVersionType",
     "ListAccessLogSubscriptionsPaginatorName",
@@ -47,15 +46,14 @@
     "VPCLatticeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AuthPolicyStateType = Literal["Active", "Inactive"]
 AuthTypeType = Literal["AWS_IAM", "NONE"]
 HealthCheckProtocolVersionType = Literal["HTTP1", "HTTP2"]
 IpAddressTypeType = Literal["IPV4", "IPV6"]
 LambdaEventStructureVersionType = Literal["V1", "V2"]
 ListAccessLogSubscriptionsPaginatorName = Literal["list_access_log_subscriptions"]
 ListListenersPaginatorName = Literal["list_listeners"]
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/literals.pyi` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/paginator.py` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     "ListServiceNetworkVpcAssociationsPaginator",
     "ListServiceNetworksPaginator",
     "ListServicesPaginator",
     "ListTargetGroupsPaginator",
     "ListTargetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -117,15 +116,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listrulespaginator)
         """
 
 
@@ -136,15 +135,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 
@@ -155,15 +154,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 
@@ -204,15 +203,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 
@@ -223,13 +222,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/paginator.pyi` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listrulespaginator)
         """
 
 class ListServiceNetworkServiceAssociationsPaginator(AioPaginator):
@@ -130,15 +130,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 class ListServiceNetworkVpcAssociationsPaginator(AioPaginator):
@@ -148,15 +148,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 class ListServiceNetworksPaginator(AioPaginator):
@@ -194,15 +194,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 class ListTargetsPaginator(AioPaginator):
@@ -212,13 +212,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/type_defs.py` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessLogSubscriptionSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "RuleUpdateFailureTypeDef",
     "CreateAccessLogSubscriptionRequestRequestTypeDef",
     "CreateServiceNetworkRequestRequestTypeDef",
     "CreateServiceNetworkServiceAssociationRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice/type_defs.pyi` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-vpc-lattice
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.VPCLattice 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.VPCLattice 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/
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
 
 <a id="types-aiobotocore-vpc-lattice"></a>
 
 # types-aiobotocore-vpc-lattice
 
 [![PyPI - types-aiobotocore-vpc-lattice](https://img.shields.io/pypi/v/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VPCLattice 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[aiobotocore.VPCLattice 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [types-aiobotocore-vpc-lattice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-vpc-lattice-2.9.0/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt` & `types-aiobotocore-vpc-lattice-2.9.1/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

