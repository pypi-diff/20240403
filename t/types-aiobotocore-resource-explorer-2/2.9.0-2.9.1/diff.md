# Comparing `tmp/types-aiobotocore-resource-explorer-2-2.9.0.tar.gz` & `tmp/types-aiobotocore-resource-explorer-2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resource-explorer-2-2.9.0.tar", last modified: Wed Dec 13 20:00:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-resource-explorer-2-2.9.1.tar", last modified: Thu Jan 18 01:21:37 2024, max compression
```

## Comparing `types-aiobotocore-resource-explorer-2-2.9.0.tar` & `types-aiobotocore-resource-explorer-2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.133244 types-aiobotocore-resource-explorer-2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14228 2023-12-13 20:00:18.133244 types-aiobotocore-resource-explorer-2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:18.133244 types-aiobotocore-resource-explorer-2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-12-13 19:54:39.000000 types-aiobotocore-resource-explorer-2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.129244 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20909 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20905 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13899 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13898 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:40.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.133244 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14228 2023-12-13 20:00:18.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-13 20:00:18.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:18.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:18.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:18.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:18.000000 types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:37.681084 types-aiobotocore-resource-explorer-2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-01-18 01:21:37.681084 types-aiobotocore-resource-explorer-2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:37.681084 types-aiobotocore-resource-explorer-2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-01-18 01:16:15.000000 types-aiobotocore-resource-explorer-2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:37.681084 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20911 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20908 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:16.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:37.681084 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-01-18 01:21:37.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-01-18 01:21:37.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:37.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:37.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:37.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:37.000000 types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/LICENSE` & `types-aiobotocore-resource-explorer-2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/PKG-INFO` & `types-aiobotocore-resource-explorer-2-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-explorer-2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ResourceExplorer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ResourceExplorer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/
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
 
 <a id="types-aiobotocore-resource-explorer-2"></a>
 
 # types-aiobotocore-resource-explorer-2
 
 [![PyPI - types-aiobotocore-resource-explorer-2](https://img.shields.io/pypi/v/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-explorer-2)](https://pepy.tech/project/types-aiobotocore-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceExplorer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[aiobotocore.ResourceExplorer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/README.md` & `types-aiobotocore-resource-explorer-2-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-explorer-2)](https://pepy.tech/project/types-aiobotocore-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceExplorer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[aiobotocore.ResourceExplorer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/setup.py` & `types-aiobotocore-resource-explorer-2-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resource-explorer-2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_resource_explorer_2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ResourceExplorer 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ResourceExplorer 2.9.1 service generated with"
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
     keywords="aiobotocore resource-explorer-2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_resource_explorer_2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/__init__.py` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListSupportedResourceTypesPaginator,
     ListViewsPaginator,
     SearchPaginator,
 )
 
 Client = ResourceExplorerClient
 
-
 __all__ = (
     "Client",
     "ListIndexesForMembersPaginator",
     "ListIndexesPaginator",
     "ListSupportedResourceTypesPaginator",
     "ListViewsPaginator",
     "ResourceExplorerClient",
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/__init__.pyi` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/__main__.py` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResourceExplorer 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ResourceExplorer 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer\nOther"
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

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/client.py` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ResourceExplorerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -149,15 +148,15 @@
         self,
         *,
         ViewName: str,
         ClientToken: str = ...,
         Filters: SearchFilterTypeDef = ...,
         IncludedProperties: Sequence[IncludedPropertyTypeDef] = ...,
         Scope: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateViewOutputTypeDef:
         """
         Creates a view that users can query by using the  Search operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Client.create_view)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/client/#create_view)
         """
@@ -246,15 +245,15 @@
 
     async def list_indexes(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Regions: Sequence[str] = ...,
-        Type: IndexTypeType = ...
+        Type: IndexTypeType = ...,
     ) -> ListIndexesOutputTypeDef:
         """
         Retrieves a list of all of the indexes in Amazon Web Services Regions that are
         currently collecting resource information for Amazon Web Services Resource
         Explorer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Client.list_indexes)
@@ -351,15 +350,15 @@
         """
 
     async def update_view(
         self,
         *,
         ViewArn: str,
         Filters: SearchFilterTypeDef = ...,
-        IncludedProperties: Sequence[IncludedPropertyTypeDef] = ...
+        IncludedProperties: Sequence[IncludedPropertyTypeDef] = ...,
     ) -> UpdateViewOutputTypeDef:
         """
         Modifies some of the details of a view.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Client.update_view)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/client/#update_view)
         """
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/client.pyi` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         self,
         *,
         ViewName: str,
         ClientToken: str = ...,
         Filters: SearchFilterTypeDef = ...,
         IncludedProperties: Sequence[IncludedPropertyTypeDef] = ...,
         Scope: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateViewOutputTypeDef:
         """
         Creates a view that users can query by using the  Search operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Client.create_view)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/client/#create_view)
         """
@@ -242,15 +242,15 @@
 
     async def list_indexes(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Regions: Sequence[str] = ...,
-        Type: IndexTypeType = ...
+        Type: IndexTypeType = ...,
     ) -> ListIndexesOutputTypeDef:
         """
         Retrieves a list of all of the indexes in Amazon Web Services Regions that are
         currently collecting resource information for Amazon Web Services Resource
         Explorer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Client.list_indexes)
@@ -347,15 +347,15 @@
         """
 
     async def update_view(
         self,
         *,
         ViewArn: str,
         Filters: SearchFilterTypeDef = ...,
-        IncludedProperties: Sequence[IncludedPropertyTypeDef] = ...
+        IncludedProperties: Sequence[IncludedPropertyTypeDef] = ...,
     ) -> UpdateViewOutputTypeDef:
         """
         Modifies some of the details of a view.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Client.update_view)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/client/#update_view)
         """
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/literals.py` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/literals.py`

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
     "AWSServiceAccessStatusType",
     "IndexStateType",
     "IndexTypeType",
     "ListIndexesForMembersPaginatorName",
     "ListIndexesPaginatorName",
     "ListSupportedResourceTypesPaginatorName",
@@ -32,15 +31,14 @@
     "ResourceExplorerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AWSServiceAccessStatusType = Literal["DISABLED", "ENABLED"]
 IndexStateType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING", "UPDATING"]
 IndexTypeType = Literal["AGGREGATOR", "LOCAL"]
 ListIndexesForMembersPaginatorName = Literal["list_indexes_for_members"]
 ListIndexesPaginatorName = Literal["list_indexes"]
 ListSupportedResourceTypesPaginatorName = Literal["list_supported_resource_types"]
 ListViewsPaginatorName = Literal["list_views"]
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/literals.pyi` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/paginator.py` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     "ListIndexesPaginator",
     "ListIndexesForMembersPaginator",
     "ListSupportedResourceTypesPaginator",
     "ListViewsPaginator",
     "SearchPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -70,15 +69,15 @@
     """
 
     def paginate(
         self,
         *,
         Regions: Sequence[str] = ...,
         Type: IndexTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIndexesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listindexespaginator)
         """
 
 
@@ -134,13 +133,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ViewArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#searchpaginator)
         """
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/paginator.pyi` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     """
 
     def paginate(
         self,
         *,
         Regions: Sequence[str] = ...,
         Type: IndexTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIndexesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listindexespaginator)
         """
 
 class ListIndexesForMembersPaginator(AioPaginator):
@@ -127,13 +127,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ViewArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#searchpaginator)
         """
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/type_defs.py` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateDefaultViewInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetViewErrorTypeDef",
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
     "IncludedPropertyTypeDef",
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2/type_defs.pyi` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-explorer-2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ResourceExplorer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ResourceExplorer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/
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
 
 <a id="types-aiobotocore-resource-explorer-2"></a>
 
 # types-aiobotocore-resource-explorer-2
 
 [![PyPI - types-aiobotocore-resource-explorer-2](https://img.shields.io/pypi/v/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-explorer-2)](https://pepy.tech/project/types-aiobotocore-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceExplorer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[aiobotocore.ResourceExplorer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resource-explorer-2-2.9.0/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt` & `types-aiobotocore-resource-explorer-2-2.9.1/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

