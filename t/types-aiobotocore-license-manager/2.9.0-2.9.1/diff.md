# Comparing `tmp/types-aiobotocore-license-manager-2.9.0.tar.gz` & `tmp/types-aiobotocore-license-manager-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-license-manager-2.9.0.tar", last modified: Wed Dec 13 19:59:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-license-manager-2.9.1.tar", last modified: Thu Jan 18 01:21:08 2024, max compression
```

## Comparing `types-aiobotocore-license-manager-2.9.0.tar` & `types-aiobotocore-license-manager-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:45.565527 types-aiobotocore-license-manager-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:09.000000 types-aiobotocore-license-manager-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2023-12-13 19:59:45.565527 types-aiobotocore-license-manager-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2023-12-13 19:49:09.000000 types-aiobotocore-license-manager-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:45.565527 types-aiobotocore-license-manager-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-12-13 19:49:09.000000 types-aiobotocore-license-manager-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:45.561527 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2023-12-13 19:49:09.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2023-12-13 19:49:09.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-13 19:49:09.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43080 2023-12-13 19:49:11.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43076 2023-12-13 19:49:11.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-13 19:49:11.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13076 2023-12-13 19:49:11.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2023-12-13 19:49:11.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2023-12-13 19:49:11.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:09.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    47305 2023-12-13 19:49:12.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    47304 2023-12-13 19:49:11.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:09.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:45.565527 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.077218 types-aiobotocore-license-manager-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-01-18 01:21:08.077218 types-aiobotocore-license-manager-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:08.077218 types-aiobotocore-license-manager-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.073218 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43102 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43099 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13076 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13076 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    47304 2024-01-18 01:10:59.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47304 2024-01-18 01:10:57.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:56.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.073218 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-license-manager-2.9.0/LICENSE` & `types-aiobotocore-license-manager-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-license-manager-2.9.0/PKG-INFO` & `types-aiobotocore-license-manager-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LicenseManager 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LicenseManager 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/
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
 
 <a id="types-aiobotocore-license-manager"></a>
 
 # types-aiobotocore-license-manager
 
 [![PyPI - types-aiobotocore-license-manager](https://img.shields.io/pypi/v/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[aiobotocore.LicenseManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [types-aiobotocore-license-manager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-license-manager-2.9.0/README.md` & `types-aiobotocore-license-manager-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[aiobotocore.LicenseManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [types-aiobotocore-license-manager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-license-manager-2.9.0/setup.py` & `types-aiobotocore-license-manager-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-license-manager",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LicenseManager 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LicenseManager 2.9.1 service generated with"
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
     keywords="aiobotocore license-manager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_license_manager": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/__init__.py` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListLicenseSpecificationsForResourcePaginator,
     ListResourceInventoryPaginator,
     ListUsageForLicenseConfigurationPaginator,
 )
 
 Client = LicenseManagerClient
 
-
 __all__ = (
     "Client",
     "LicenseManagerClient",
     "ListAssociationsForLicenseConfigurationPaginator",
     "ListLicenseConfigurationsPaginator",
     "ListLicenseSpecificationsForResourcePaginator",
     "ListResourceInventoryPaginator",
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/__init__.pyi` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/__main__.py` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LicenseManager 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LicenseManager 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager\nOther"
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

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/client.py` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LicenseManagerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -181,15 +180,15 @@
         self,
         *,
         LicenseArn: str,
         Entitlements: Sequence[EntitlementDataTypeDef],
         DigitalSignatureMethod: Literal["JWT_PS384"],
         ClientToken: str,
         NodeId: str = ...,
-        CheckoutMetadata: Sequence[MetadataTypeDef] = ...
+        CheckoutMetadata: Sequence[MetadataTypeDef] = ...,
     ) -> CheckoutBorrowLicenseResponseTypeDef:
         """
         Checks out the specified license for offline use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.checkout_borrow_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#checkout_borrow_license)
         """
@@ -199,15 +198,15 @@
         *,
         ProductSKU: str,
         CheckoutType: CheckoutTypeType,
         KeyFingerprint: str,
         Entitlements: Sequence[EntitlementDataTypeDef],
         ClientToken: str,
         Beneficiary: str = ...,
-        NodeId: str = ...
+        NodeId: str = ...,
     ) -> CheckoutLicenseResponseTypeDef:
         """
         Checks out the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.checkout_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#checkout_license)
         """
@@ -224,15 +223,15 @@
         self,
         *,
         ClientToken: str,
         GrantName: str,
         LicenseArn: str,
         Principals: Sequence[str],
         HomeRegion: str,
-        AllowedOperations: Sequence[AllowedOperationType]
+        AllowedOperations: Sequence[AllowedOperationType],
     ) -> CreateGrantResponseTypeDef:
         """
         Creates a grant for the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_grant)
         """
@@ -243,15 +242,15 @@
         ClientToken: str,
         GrantArn: str,
         GrantName: str = ...,
         AllowedOperations: Sequence[AllowedOperationType] = ...,
         Status: GrantStatusType = ...,
         StatusReason: str = ...,
         SourceVersion: str = ...,
-        Options: OptionsTypeDef = ...
+        Options: OptionsTypeDef = ...,
     ) -> CreateGrantVersionResponseTypeDef:
         """
         Creates a new version of the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_grant_version)
         """
@@ -265,15 +264,15 @@
         Issuer: IssuerTypeDef,
         HomeRegion: str,
         Validity: DatetimeRangeTypeDef,
         Entitlements: Sequence[EntitlementTypeDef],
         Beneficiary: str,
         ConsumptionConfiguration: ConsumptionConfigurationTypeDef,
         ClientToken: str,
-        LicenseMetadata: Sequence[MetadataTypeDef] = ...
+        LicenseMetadata: Sequence[MetadataTypeDef] = ...,
     ) -> CreateLicenseResponseTypeDef:
         """
         Creates a license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license)
         """
@@ -285,29 +284,29 @@
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...
+        ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_configuration)
         """
 
     async def create_license_conversion_task_for_resource(
         self,
         *,
         ResourceArn: str,
         SourceLicenseContext: LicenseConversionContextTypeDef,
-        DestinationLicenseContext: LicenseConversionContextTypeDef
+        DestinationLicenseContext: LicenseConversionContextTypeDef,
     ) -> CreateLicenseConversionTaskForResourceResponseTypeDef:
         """
         Creates a new license conversion task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_conversion_task_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_conversion_task_for_resource)
         """
@@ -317,15 +316,15 @@
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
         ReportContext: ReportContextTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_manager_report_generator)
         """
@@ -340,15 +339,15 @@
         HomeRegion: str,
         Validity: DatetimeRangeTypeDef,
         Entitlements: Sequence[EntitlementTypeDef],
         ConsumptionConfiguration: ConsumptionConfigurationTypeDef,
         Status: LicenseStatusType,
         ClientToken: str,
         LicenseMetadata: Sequence[MetadataTypeDef] = ...,
-        SourceVersion: str = ...
+        SourceVersion: str = ...,
     ) -> CreateLicenseVersionResponseTypeDef:
         """
         Creates a new version of the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_version)
         """
@@ -356,15 +355,15 @@
     async def create_token(
         self,
         *,
         LicenseArn: str,
         ClientToken: str,
         RoleArns: Sequence[str] = ...,
         ExpirationInDays: int = ...,
-        TokenProperties: Sequence[str] = ...
+        TokenProperties: Sequence[str] = ...,
     ) -> CreateTokenResponseTypeDef:
         """
         Creates a long-lived token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_token)
         """
@@ -525,15 +524,15 @@
 
     async def list_distributed_grants(
         self,
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDistributedGrantsResponseTypeDef:
         """
         Lists the grants distributed for the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_distributed_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_distributed_grants)
         """
@@ -550,15 +549,15 @@
 
     async def list_license_configurations(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListLicenseConfigurationsResponseTypeDef:
         """
         Lists the license configurations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_configurations)
         """
@@ -605,60 +604,60 @@
 
     async def list_licenses(
         self,
         *,
         LicenseArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLicensesResponseTypeDef:
         """
         Lists the licenses for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_licenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_licenses)
         """
 
     async def list_received_grants(
         self,
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReceivedGrantsResponseTypeDef:
         """
         Lists grants that are received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_grants)
         """
 
     async def list_received_grants_for_organization(
         self,
         *,
         LicenseArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReceivedGrantsForOrganizationResponseTypeDef:
         """
         Lists the grants received for all accounts in the organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_grants_for_organization)
         """
 
     async def list_received_licenses(
         self,
         *,
         LicenseArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReceivedLicensesResponseTypeDef:
         """
         Lists received licenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_licenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_licenses)
         """
@@ -674,15 +673,15 @@
         """
 
     async def list_resource_inventory(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[InventoryFilterTypeDef] = ...
+        Filters: Sequence[InventoryFilterTypeDef] = ...,
     ) -> ListResourceInventoryResponseTypeDef:
         """
         Lists resources managed using Systems Manager inventory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_resource_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_resource_inventory)
         """
@@ -699,30 +698,30 @@
 
     async def list_tokens(
         self,
         *,
         TokenIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTokensResponseTypeDef:
         """
         Lists your tokens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_tokens)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_tokens)
         """
 
     async def list_usage_for_license_configuration(
         self,
         *,
         LicenseConfigurationArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListUsageForLicenseConfigurationResponseTypeDef:
         """
         Lists all license usage records for a license configuration, displaying license
         consumption details by resource at a selected point in
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_usage_for_license_configuration)
@@ -760,15 +759,15 @@
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
         ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
-        DisassociateWhenNotFound: bool = ...
+        DisassociateWhenNotFound: bool = ...,
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_configuration)
         """
@@ -778,29 +777,29 @@
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
         ReportContext: ReportContextTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_manager_report_generator)
         """
 
     async def update_license_specifications_for_resource(
         self,
         *,
         ResourceArn: str,
         AddLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...,
-        RemoveLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...
+        RemoveLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Adds or removes the specified license configurations for the specified Amazon
         Web Services
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_specifications_for_resource)
@@ -809,15 +808,15 @@
 
     async def update_service_settings(
         self,
         *,
         S3BucketArn: str = ...,
         SnsTopicArn: str = ...,
         OrganizationConfiguration: OrganizationConfigurationTypeDef = ...,
-        EnableCrossAccountsDiscovery: bool = ...
+        EnableCrossAccountsDiscovery: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates License Manager settings for the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_service_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_service_settings)
         """
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/client.pyi` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         self,
         *,
         LicenseArn: str,
         Entitlements: Sequence[EntitlementDataTypeDef],
         DigitalSignatureMethod: Literal["JWT_PS384"],
         ClientToken: str,
         NodeId: str = ...,
-        CheckoutMetadata: Sequence[MetadataTypeDef] = ...
+        CheckoutMetadata: Sequence[MetadataTypeDef] = ...,
     ) -> CheckoutBorrowLicenseResponseTypeDef:
         """
         Checks out the specified license for offline use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.checkout_borrow_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#checkout_borrow_license)
         """
@@ -195,15 +195,15 @@
         *,
         ProductSKU: str,
         CheckoutType: CheckoutTypeType,
         KeyFingerprint: str,
         Entitlements: Sequence[EntitlementDataTypeDef],
         ClientToken: str,
         Beneficiary: str = ...,
-        NodeId: str = ...
+        NodeId: str = ...,
     ) -> CheckoutLicenseResponseTypeDef:
         """
         Checks out the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.checkout_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#checkout_license)
         """
@@ -220,15 +220,15 @@
         self,
         *,
         ClientToken: str,
         GrantName: str,
         LicenseArn: str,
         Principals: Sequence[str],
         HomeRegion: str,
-        AllowedOperations: Sequence[AllowedOperationType]
+        AllowedOperations: Sequence[AllowedOperationType],
     ) -> CreateGrantResponseTypeDef:
         """
         Creates a grant for the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_grant)
         """
@@ -239,15 +239,15 @@
         ClientToken: str,
         GrantArn: str,
         GrantName: str = ...,
         AllowedOperations: Sequence[AllowedOperationType] = ...,
         Status: GrantStatusType = ...,
         StatusReason: str = ...,
         SourceVersion: str = ...,
-        Options: OptionsTypeDef = ...
+        Options: OptionsTypeDef = ...,
     ) -> CreateGrantVersionResponseTypeDef:
         """
         Creates a new version of the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_grant_version)
         """
@@ -261,15 +261,15 @@
         Issuer: IssuerTypeDef,
         HomeRegion: str,
         Validity: DatetimeRangeTypeDef,
         Entitlements: Sequence[EntitlementTypeDef],
         Beneficiary: str,
         ConsumptionConfiguration: ConsumptionConfigurationTypeDef,
         ClientToken: str,
-        LicenseMetadata: Sequence[MetadataTypeDef] = ...
+        LicenseMetadata: Sequence[MetadataTypeDef] = ...,
     ) -> CreateLicenseResponseTypeDef:
         """
         Creates a license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license)
         """
@@ -281,29 +281,29 @@
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...
+        ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_configuration)
         """
 
     async def create_license_conversion_task_for_resource(
         self,
         *,
         ResourceArn: str,
         SourceLicenseContext: LicenseConversionContextTypeDef,
-        DestinationLicenseContext: LicenseConversionContextTypeDef
+        DestinationLicenseContext: LicenseConversionContextTypeDef,
     ) -> CreateLicenseConversionTaskForResourceResponseTypeDef:
         """
         Creates a new license conversion task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_conversion_task_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_conversion_task_for_resource)
         """
@@ -313,15 +313,15 @@
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
         ReportContext: ReportContextTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_manager_report_generator)
         """
@@ -336,15 +336,15 @@
         HomeRegion: str,
         Validity: DatetimeRangeTypeDef,
         Entitlements: Sequence[EntitlementTypeDef],
         ConsumptionConfiguration: ConsumptionConfigurationTypeDef,
         Status: LicenseStatusType,
         ClientToken: str,
         LicenseMetadata: Sequence[MetadataTypeDef] = ...,
-        SourceVersion: str = ...
+        SourceVersion: str = ...,
     ) -> CreateLicenseVersionResponseTypeDef:
         """
         Creates a new version of the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_version)
         """
@@ -352,15 +352,15 @@
     async def create_token(
         self,
         *,
         LicenseArn: str,
         ClientToken: str,
         RoleArns: Sequence[str] = ...,
         ExpirationInDays: int = ...,
-        TokenProperties: Sequence[str] = ...
+        TokenProperties: Sequence[str] = ...,
     ) -> CreateTokenResponseTypeDef:
         """
         Creates a long-lived token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_token)
         """
@@ -521,15 +521,15 @@
 
     async def list_distributed_grants(
         self,
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDistributedGrantsResponseTypeDef:
         """
         Lists the grants distributed for the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_distributed_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_distributed_grants)
         """
@@ -546,15 +546,15 @@
 
     async def list_license_configurations(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListLicenseConfigurationsResponseTypeDef:
         """
         Lists the license configurations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_configurations)
         """
@@ -601,60 +601,60 @@
 
     async def list_licenses(
         self,
         *,
         LicenseArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLicensesResponseTypeDef:
         """
         Lists the licenses for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_licenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_licenses)
         """
 
     async def list_received_grants(
         self,
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReceivedGrantsResponseTypeDef:
         """
         Lists grants that are received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_grants)
         """
 
     async def list_received_grants_for_organization(
         self,
         *,
         LicenseArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReceivedGrantsForOrganizationResponseTypeDef:
         """
         Lists the grants received for all accounts in the organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_grants_for_organization)
         """
 
     async def list_received_licenses(
         self,
         *,
         LicenseArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReceivedLicensesResponseTypeDef:
         """
         Lists received licenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_licenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_licenses)
         """
@@ -670,15 +670,15 @@
         """
 
     async def list_resource_inventory(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[InventoryFilterTypeDef] = ...
+        Filters: Sequence[InventoryFilterTypeDef] = ...,
     ) -> ListResourceInventoryResponseTypeDef:
         """
         Lists resources managed using Systems Manager inventory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_resource_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_resource_inventory)
         """
@@ -695,30 +695,30 @@
 
     async def list_tokens(
         self,
         *,
         TokenIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTokensResponseTypeDef:
         """
         Lists your tokens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_tokens)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_tokens)
         """
 
     async def list_usage_for_license_configuration(
         self,
         *,
         LicenseConfigurationArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListUsageForLicenseConfigurationResponseTypeDef:
         """
         Lists all license usage records for a license configuration, displaying license
         consumption details by resource at a selected point in
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_usage_for_license_configuration)
@@ -756,15 +756,15 @@
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
         ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
-        DisassociateWhenNotFound: bool = ...
+        DisassociateWhenNotFound: bool = ...,
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_configuration)
         """
@@ -774,29 +774,29 @@
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
         ReportContext: ReportContextTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_manager_report_generator)
         """
 
     async def update_license_specifications_for_resource(
         self,
         *,
         ResourceArn: str,
         AddLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...,
-        RemoveLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...
+        RemoveLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Adds or removes the specified license configurations for the specified Amazon
         Web Services
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_specifications_for_resource)
@@ -805,15 +805,15 @@
 
     async def update_service_settings(
         self,
         *,
         S3BucketArn: str = ...,
         SnsTopicArn: str = ...,
         OrganizationConfiguration: OrganizationConfigurationTypeDef = ...,
-        EnableCrossAccountsDiscovery: bool = ...
+        EnableCrossAccountsDiscovery: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates License Manager settings for the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_service_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_service_settings)
         """
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/literals.py` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/literals.py`

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
     "ActivationOverrideBehaviorType",
     "AllowedOperationType",
     "CheckoutTypeType",
     "DigitalSignatureMethodType",
     "EntitlementDataUnitType",
     "EntitlementUnitType",
@@ -48,15 +47,14 @@
     "LicenseManagerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActivationOverrideBehaviorType = Literal[
     "ALL_GRANTS_PERMITTED_BY_ISSUER", "DISTRIBUTED_GRANTS_ONLY"
 ]
 AllowedOperationType = Literal[
     "CheckInLicense",
     "CheckoutBorrowLicense",
     "CheckoutLicense",
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/literals.pyi` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/paginator.py` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     "ListAssociationsForLicenseConfigurationPaginator",
     "ListLicenseConfigurationsPaginator",
     "ListLicenseSpecificationsForResourcePaginator",
     "ListResourceInventoryPaginator",
     "ListUsageForLicenseConfigurationPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -86,15 +85,15 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLicenseConfigurationsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listlicenseconfigurationspaginator)
         """
 
 
@@ -119,15 +118,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listresourceinventorypaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceInventoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listresourceinventorypaginator)
         """
 
 
@@ -138,13 +137,13 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsageForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listusageforlicenseconfigurationpaginator)
         """
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/paginator.pyi` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLicenseConfigurationsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listlicenseconfigurationspaginator)
         """
 
 class ListLicenseSpecificationsForResourcePaginator(AioPaginator):
@@ -113,15 +113,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listresourceinventorypaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceInventoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listresourceinventorypaginator)
         """
 
 class ListUsageForLicenseConfigurationPaginator(AioPaginator):
@@ -131,13 +131,13 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsageForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listusageforlicenseconfigurationpaginator)
         """
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/type_defs.py` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager/type_defs.pyi` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/PKG-INFO` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LicenseManager 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LicenseManager 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/
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
 
 <a id="types-aiobotocore-license-manager"></a>
 
 # types-aiobotocore-license-manager
 
 [![PyPI - types-aiobotocore-license-manager](https://img.shields.io/pypi/v/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[aiobotocore.LicenseManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [types-aiobotocore-license-manager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-license-manager-2.9.0/types_aiobotocore_license_manager.egg-info/SOURCES.txt` & `types-aiobotocore-license-manager-2.9.1/types_aiobotocore_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

