# Comparing `tmp/types-aiobotocore-bcm-data-exports-2.9.0.tar.gz` & `tmp/types-aiobotocore-bcm-data-exports-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-bcm-data-exports-2.9.0.tar", last modified: Wed Dec 13 19:58:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-bcm-data-exports-2.9.1.tar", last modified: Thu Jan 18 01:20:08 2024, max compression
```

## Comparing `types-aiobotocore-bcm-data-exports-2.9.0.tar` & `types-aiobotocore-bcm-data-exports-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:41.354039 types-aiobotocore-bcm-data-exports-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2023-12-13 19:58:41.354039 types-aiobotocore-bcm-data-exports-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12285 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:41.354039 types-aiobotocore-bcm-data-exports-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:41.354039 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13357 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13353 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:40.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:41.354039 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2023-12-13 19:58:41.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:58:41.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:41.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:41.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:41.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:58:41.000000 types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.857493 types-aiobotocore-bcm-data-exports-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-01-18 01:20:08.857493 types-aiobotocore-bcm-data-exports-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:08.857493 types-aiobotocore-bcm-data-exports-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.853493 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-01-18 01:03:39.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:38.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.857493 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-01-18 01:20:08.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:20:08.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:08.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:08.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:08.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:20:08.000000 types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/LICENSE` & `types-aiobotocore-bcm-data-exports-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/PKG-INFO` & `types-aiobotocore-bcm-data-exports-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-bcm-data-exports
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.BillingandCostManagementDataExports 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.BillingandCostManagementDataExports 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/
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
 
 <a id="types-aiobotocore-bcm-data-exports"></a>
 
 # types-aiobotocore-bcm-data-exports
 
 [![PyPI - types-aiobotocore-bcm-data-exports](https://img.shields.io/pypi/v/types-aiobotocore-bcm-data-exports.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bcm-data-exports)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bcm-data-exports.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bcm-data-exports)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bcm-data-exports)](https://pepy.tech/project/types-aiobotocore-bcm-data-exports)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingandCostManagementDataExports 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports)
+[aiobotocore.BillingandCostManagementDataExports 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports)
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
 [types-aiobotocore-bcm-data-exports docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/README.md` & `types-aiobotocore-bcm-data-exports-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bcm-data-exports.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bcm-data-exports)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bcm-data-exports)](https://pepy.tech/project/types-aiobotocore-bcm-data-exports)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingandCostManagementDataExports 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports)
+[aiobotocore.BillingandCostManagementDataExports 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports)
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
 [types-aiobotocore-bcm-data-exports docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/setup.py` & `types-aiobotocore-bcm-data-exports-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-bcm-data-exports",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_bcm_data_exports"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.BillingandCostManagementDataExports 2.9.0 service"
-        " generated with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.BillingandCostManagementDataExports 2.9.1 service"
+        " generated with mypy-boto3-builder 7.23.1"
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
     keywords="aiobotocore bcm-data-exports type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_bcm_data_exports": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/__init__.py` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import BillingandCostManagementDataExportsClient
 from .paginator import ListExecutionsPaginator, ListExportsPaginator, ListTablesPaginator
 
 Client = BillingandCostManagementDataExportsClient
 
-
 __all__ = (
     "BillingandCostManagementDataExportsClient",
     "Client",
     "ListExecutionsPaginator",
     "ListExportsPaginator",
     "ListTablesPaginator",
 )
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/__init__.pyi` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/__main__.py` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BillingandCostManagementDataExports 2.9.0\nVersion:      "
-        "   2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.BillingandCostManagementDataExports 2.9.1\nVersion:      "
+        "   2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports\nOther"
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

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/client.py` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BillingandCostManagementDataExportsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/client.pyi` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/literals.py` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/literals.py`

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
     "CompressionOptionType",
     "ExecutionStatusCodeType",
     "ExecutionStatusReasonType",
     "ExportStatusCodeType",
     "FormatOptionType",
     "FrequencyOptionType",
@@ -34,15 +33,14 @@
     "S3OutputTypeType",
     "BillingandCostManagementDataExportsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 CompressionOptionType = Literal["GZIP", "PARQUET"]
 ExecutionStatusCodeType = Literal[
     "DELIVERY_FAILURE",
     "DELIVERY_IN_PROCESS",
     "DELIVERY_SUCCESS",
     "INITIATION_IN_PROCESS",
     "QUERY_FAILURE",
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/literals.pyi` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/paginator.py` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListExportsResponseTypeDef,
     ListTablesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListExecutionsPaginator", "ListExportsPaginator", "ListTablesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/paginator.pyi` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/type_defs.py` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/type_defs.py`

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
     "ColumnTypeDef",
     "ResourceTagTypeDef",
     "ResponseMetadataTypeDef",
     "DataQueryTypeDef",
     "DeleteExportRequestRequestTypeDef",
     "ExecutionStatusTypeDef",
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports/type_defs.pyi` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/PKG-INFO` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-bcm-data-exports
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.BillingandCostManagementDataExports 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.BillingandCostManagementDataExports 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/
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
 
 <a id="types-aiobotocore-bcm-data-exports"></a>
 
 # types-aiobotocore-bcm-data-exports
 
 [![PyPI - types-aiobotocore-bcm-data-exports](https://img.shields.io/pypi/v/types-aiobotocore-bcm-data-exports.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bcm-data-exports)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bcm-data-exports.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bcm-data-exports)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bcm-data-exports)](https://pepy.tech/project/types-aiobotocore-bcm-data-exports)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingandCostManagementDataExports 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports)
+[aiobotocore.BillingandCostManagementDataExports 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports)
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
 [types-aiobotocore-bcm-data-exports docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bcm_data_exports/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bcm-data-exports-2.9.0/types_aiobotocore_bcm_data_exports.egg-info/SOURCES.txt` & `types-aiobotocore-bcm-data-exports-2.9.1/types_aiobotocore_bcm_data_exports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

