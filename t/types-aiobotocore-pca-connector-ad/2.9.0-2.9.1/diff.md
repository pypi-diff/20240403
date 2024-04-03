# Comparing `tmp/types-aiobotocore-pca-connector-ad-2.9.0.tar.gz` & `tmp/types-aiobotocore-pca-connector-ad-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pca-connector-ad-2.9.0.tar", last modified: Wed Dec 13 20:00:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-pca-connector-ad-2.9.1.tar", last modified: Thu Jan 18 01:21:27 2024, max compression
```

## Comparing `types-aiobotocore-pca-connector-ad-2.9.0.tar` & `types-aiobotocore-pca-connector-ad-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.101340 types-aiobotocore-pca-connector-ad-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2023-12-13 20:00:07.101340 types-aiobotocore-pca-connector-ad-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:07.101340 types-aiobotocore-pca-connector-ad-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.097340 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24003 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13550 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35614 2023-12-13 19:51:29.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35613 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:28.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.101340 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2023-12-13 20:00:07.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 20:00:07.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:07.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:07.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:07.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 20:00:07.000000 types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.673129 types-aiobotocore-pca-connector-ad-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-01-18 01:21:27.673129 types-aiobotocore-pca-connector-ad-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:27.673129 types-aiobotocore-pca-connector-ad-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.669129 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24011 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24008 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    35613 2024-01-18 01:13:09.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35613 2024-01-18 01:13:09.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:08.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.673129 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-01-18 01:21:27.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:21:27.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:27.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:27.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:27.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:21:27.000000 types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/LICENSE` & `types-aiobotocore-pca-connector-ad-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/PKG-INFO` & `types-aiobotocore-pca-connector-ad-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pca-connector-ad
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PcaConnectorAd 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PcaConnectorAd 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/
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
 
 <a id="types-aiobotocore-pca-connector-ad"></a>
 
 # types-aiobotocore-pca-connector-ad
 
 [![PyPI - types-aiobotocore-pca-connector-ad](https://img.shields.io/pypi/v/types-aiobotocore-pca-connector-ad.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pca-connector-ad)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pca-connector-ad.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pca-connector-ad)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pca-connector-ad)](https://pepy.tech/project/types-aiobotocore-pca-connector-ad)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PcaConnectorAd 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd)
+[aiobotocore.PcaConnectorAd 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd)
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
 [types-aiobotocore-pca-connector-ad docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/README.md` & `types-aiobotocore-pca-connector-ad-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pca-connector-ad.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pca-connector-ad)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pca-connector-ad)](https://pepy.tech/project/types-aiobotocore-pca-connector-ad)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PcaConnectorAd 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd)
+[aiobotocore.PcaConnectorAd 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd)
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
 [types-aiobotocore-pca-connector-ad docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/setup.py` & `types-aiobotocore-pca-connector-ad-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pca-connector-ad",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_pca_connector_ad"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PcaConnectorAd 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PcaConnectorAd 2.9.1 service generated with"
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
     keywords="aiobotocore pca-connector-ad type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_pca_connector_ad": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/__init__.py` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListServicePrincipalNamesPaginator,
     ListTemplateGroupAccessControlEntriesPaginator,
     ListTemplatesPaginator,
 )
 
 Client = PcaConnectorAdClient
 
-
 __all__ = (
     "Client",
     "ListConnectorsPaginator",
     "ListDirectoryRegistrationsPaginator",
     "ListServicePrincipalNamesPaginator",
     "ListTemplateGroupAccessControlEntriesPaginator",
     "ListTemplatesPaginator",
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/__init__.pyi` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/__main__.py` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PcaConnectorAd 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PcaConnectorAd 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd\nOther"
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

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/client.py` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PcaConnectorAdClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -113,15 +112,15 @@
     async def create_connector(
         self,
         *,
         CertificateAuthorityArn: str,
         DirectoryId: str,
         VpcInformation: VpcInformationTypeDef,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates a connector between Amazon Web Services Private CA and an Active
         Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.create_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#create_connector)
@@ -153,15 +152,15 @@
     async def create_template(
         self,
         *,
         ConnectorArn: str,
         Definition: TemplateDefinitionTypeDef,
         Name: str,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates an Active Directory compatible certificate template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.create_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#create_template)
         """
@@ -169,15 +168,15 @@
     async def create_template_group_access_control_entry(
         self,
         *,
         AccessRights: AccessRightsTypeDef,
         GroupDisplayName: str,
         GroupSecurityIdentifier: str,
         TemplateArn: str,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Create a group access control entry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.create_template_group_access_control_entry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#create_template_group_access_control_entry)
         """
@@ -381,15 +380,15 @@
         """
 
     async def update_template(
         self,
         *,
         TemplateArn: str,
         Definition: TemplateDefinitionTypeDef = ...,
-        ReenrollAllCertificateHolders: bool = ...
+        ReenrollAllCertificateHolders: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update template configuration to define the information included in
         certificates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.update_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#update_template)
@@ -397,15 +396,15 @@
 
     async def update_template_group_access_control_entry(
         self,
         *,
         GroupSecurityIdentifier: str,
         TemplateArn: str,
         AccessRights: AccessRightsTypeDef = ...,
-        GroupDisplayName: str = ...
+        GroupDisplayName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update a group access control entry you created using
         [CreateTemplateGroupAccessControlEntry](https://docs.aws.amazon.com/pca-connector-ad/latest/APIReference/API_CreateTemplateGroupAccessControlEntry.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.update_template_group_access_control_entry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#update_template_group_access_control_entry)
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/client.pyi` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     async def create_connector(
         self,
         *,
         CertificateAuthorityArn: str,
         DirectoryId: str,
         VpcInformation: VpcInformationTypeDef,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates a connector between Amazon Web Services Private CA and an Active
         Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.create_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#create_connector)
@@ -149,15 +149,15 @@
     async def create_template(
         self,
         *,
         ConnectorArn: str,
         Definition: TemplateDefinitionTypeDef,
         Name: str,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates an Active Directory compatible certificate template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.create_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#create_template)
         """
@@ -165,15 +165,15 @@
     async def create_template_group_access_control_entry(
         self,
         *,
         AccessRights: AccessRightsTypeDef,
         GroupDisplayName: str,
         GroupSecurityIdentifier: str,
         TemplateArn: str,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Create a group access control entry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.create_template_group_access_control_entry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#create_template_group_access_control_entry)
         """
@@ -377,15 +377,15 @@
         """
 
     async def update_template(
         self,
         *,
         TemplateArn: str,
         Definition: TemplateDefinitionTypeDef = ...,
-        ReenrollAllCertificateHolders: bool = ...
+        ReenrollAllCertificateHolders: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update template configuration to define the information included in
         certificates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.update_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#update_template)
@@ -393,15 +393,15 @@
 
     async def update_template_group_access_control_entry(
         self,
         *,
         GroupSecurityIdentifier: str,
         TemplateArn: str,
         AccessRights: AccessRightsTypeDef = ...,
-        GroupDisplayName: str = ...
+        GroupDisplayName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update a group access control entry you created using
         [CreateTemplateGroupAccessControlEntry](https://docs.aws.amazon.com/pca-connector-ad/latest/APIReference/API_CreateTemplateGroupAccessControlEntry.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client.update_template_group_access_control_entry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/client/#update_template_group_access_control_entry)
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/literals.py` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/literals.py`

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
     "AccessRightType",
     "ApplicationPolicyTypeType",
     "ClientCompatibilityV2Type",
     "ClientCompatibilityV3Type",
     "ClientCompatibilityV4Type",
     "ConnectorStatusReasonType",
@@ -45,15 +44,14 @@
     "ValidityPeriodTypeType",
     "PcaConnectorAdServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AccessRightType = Literal["ALLOW", "DENY"]
 ApplicationPolicyTypeType = Literal[
     "ALL_APPLICATION_POLICIES",
     "ANY_PURPOSE",
     "ATTESTATION_IDENTITY_KEY_CERTIFICATE",
     "CERTIFICATE_REQUEST_AGENT",
     "CLIENT_AUTHENTICATION",
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/literals.pyi` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/paginator.py` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListConnectorsPaginator",
     "ListDirectoryRegistrationsPaginator",
     "ListServicePrincipalNamesPaginator",
     "ListTemplateGroupAccessControlEntriesPaginator",
     "ListTemplatesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/paginator.pyi` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/type_defs.py` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessRightsTypeDef",
     "ApplicationPolicyTypeDef",
     "ValidityPeriodTypeDef",
     "VpcInformationPaginatorTypeDef",
     "VpcInformationTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad/type_defs.pyi` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/PKG-INFO` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pca-connector-ad
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PcaConnectorAd 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PcaConnectorAd 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/
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
 
 <a id="types-aiobotocore-pca-connector-ad"></a>
 
 # types-aiobotocore-pca-connector-ad
 
 [![PyPI - types-aiobotocore-pca-connector-ad](https://img.shields.io/pypi/v/types-aiobotocore-pca-connector-ad.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pca-connector-ad)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pca-connector-ad.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pca-connector-ad)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pca-connector-ad)](https://pepy.tech/project/types-aiobotocore-pca-connector-ad)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PcaConnectorAd 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd)
+[aiobotocore.PcaConnectorAd 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd)
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
 [types-aiobotocore-pca-connector-ad docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pca_connector_ad/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pca-connector-ad-2.9.0/types_aiobotocore_pca_connector_ad.egg-info/SOURCES.txt` & `types-aiobotocore-pca-connector-ad-2.9.1/types_aiobotocore_pca_connector_ad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

