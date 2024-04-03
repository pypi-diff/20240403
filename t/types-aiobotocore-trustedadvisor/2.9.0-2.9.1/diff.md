# Comparing `tmp/types-aiobotocore-trustedadvisor-2.9.0.tar.gz` & `tmp/types-aiobotocore-trustedadvisor-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-trustedadvisor-2.9.0.tar", last modified: Wed Dec 13 20:00:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-trustedadvisor-2.9.1.tar", last modified: Thu Jan 18 01:22:00 2024, max compression
```

## Comparing `types-aiobotocore-trustedadvisor-2.9.0.tar` & `types-aiobotocore-trustedadvisor-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.001031 types-aiobotocore-trustedadvisor-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2023-12-13 20:00:43.001031 types-aiobotocore-trustedadvisor-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:43.001031 types-aiobotocore-trustedadvisor-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-12-13 19:57:30.000000 types-aiobotocore-trustedadvisor-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.001031 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16967 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10268 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18925 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18924 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:31.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.001031 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2023-12-13 20:00:42.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:42.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:42.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:42.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:42.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:42.000000 types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.220983 types-aiobotocore-trustedadvisor-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-01-18 01:22:00.220983 types-aiobotocore-trustedadvisor-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:00.220983 types-aiobotocore-trustedadvisor-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.216982 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16971 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-01-18 01:18:57.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-01-18 01:18:57.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:56.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.220983 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-01-18 01:22:00.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:22:00.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:00.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:00.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:00.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:22:00.000000 types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/LICENSE` & `types-aiobotocore-trustedadvisor-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/PKG-INFO` & `types-aiobotocore-trustedadvisor-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-trustedadvisor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TrustedAdvisorPublicAPI 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TrustedAdvisorPublicAPI 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/
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
 
 <a id="types-aiobotocore-trustedadvisor"></a>
 
 # types-aiobotocore-trustedadvisor
 
 [![PyPI - types-aiobotocore-trustedadvisor](https://img.shields.io/pypi/v/types-aiobotocore-trustedadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-trustedadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-trustedadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-trustedadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-trustedadvisor)](https://pepy.tech/project/types-aiobotocore-trustedadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TrustedAdvisorPublicAPI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
+[aiobotocore.TrustedAdvisorPublicAPI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
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
 [types-aiobotocore-trustedadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/README.md` & `types-aiobotocore-trustedadvisor-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-trustedadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-trustedadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-trustedadvisor)](https://pepy.tech/project/types-aiobotocore-trustedadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TrustedAdvisorPublicAPI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
+[aiobotocore.TrustedAdvisorPublicAPI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
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
 [types-aiobotocore-trustedadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/setup.py` & `types-aiobotocore-trustedadvisor-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-trustedadvisor",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_trustedadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.TrustedAdvisorPublicAPI 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.TrustedAdvisorPublicAPI 2.9.1 service generated with"
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
     keywords="aiobotocore trustedadvisor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_trustedadvisor": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/__init__.py` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListOrganizationRecommendationsPaginator,
     ListRecommendationResourcesPaginator,
     ListRecommendationsPaginator,
 )
 
 Client = TrustedAdvisorPublicAPIClient
 
-
 __all__ = (
     "Client",
     "ListChecksPaginator",
     "ListOrganizationRecommendationAccountsPaginator",
     "ListOrganizationRecommendationResourcesPaginator",
     "ListOrganizationRecommendationsPaginator",
     "ListRecommendationResourcesPaginator",
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/__init__.pyi` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/__main__.py` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TrustedAdvisorPublicAPI 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.TrustedAdvisorPublicAPI 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI\nOther"
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

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/client.py` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TrustedAdvisorPublicAPIClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -151,15 +150,15 @@
         self,
         *,
         awsService: str = ...,
         language: RecommendationLanguageType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
-        source: RecommendationSourceType = ...
+        source: RecommendationSourceType = ...,
     ) -> ListChecksResponseTypeDef:
         """
         List a filterable set of Checks See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListChecks).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_checks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_checks)
@@ -167,15 +166,15 @@
 
     async def list_organization_recommendation_accounts(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListOrganizationRecommendationAccountsResponseTypeDef:
         """
         Lists the accounts that own the resources for an organization aggregate
         recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendation_accounts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_organization_recommendation_accounts)
@@ -185,15 +184,15 @@
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regionCode: str = ...,
-        status: ResourceStatusType = ...
+        status: ResourceStatusType = ...,
     ) -> ListOrganizationRecommendationResourcesResponseTypeDef:
         """
         List Resources of a Recommendation within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendation_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_organization_recommendation_resources)
         """
@@ -206,15 +205,15 @@
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
-        type: RecommendationTypeType = ...
+        type: RecommendationTypeType = ...,
     ) -> ListOrganizationRecommendationsResponseTypeDef:
         """
         List a filterable set of Recommendations within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_organization_recommendations)
         """
@@ -222,15 +221,15 @@
     async def list_recommendation_resources(
         self,
         *,
         recommendationIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
         regionCode: str = ...,
-        status: ResourceStatusType = ...
+        status: ResourceStatusType = ...,
     ) -> ListRecommendationResourcesResponseTypeDef:
         """
         List Resources of a Recommendation See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListRecommendationResources).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_recommendation_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_recommendation_resources)
@@ -244,15 +243,15 @@
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
-        type: RecommendationTypeType = ...
+        type: RecommendationTypeType = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         List a filterable set of Recommendations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListRecommendations).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_recommendations)
@@ -260,30 +259,30 @@
 
     async def update_organization_recommendation_lifecycle(
         self,
         *,
         lifecycleStage: UpdateRecommendationLifecycleStageType,
         organizationRecommendationIdentifier: str,
         updateReason: str = ...,
-        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...
+        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update the lifecyle of a Recommendation within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.update_organization_recommendation_lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#update_organization_recommendation_lifecycle)
         """
 
     async def update_recommendation_lifecycle(
         self,
         *,
         lifecycleStage: UpdateRecommendationLifecycleStageType,
         recommendationIdentifier: str,
         updateReason: str = ...,
-        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...
+        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update the lifecyle of a Recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.update_recommendation_lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#update_recommendation_lifecycle)
         """
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/client.pyi` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         self,
         *,
         awsService: str = ...,
         language: RecommendationLanguageType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
-        source: RecommendationSourceType = ...
+        source: RecommendationSourceType = ...,
     ) -> ListChecksResponseTypeDef:
         """
         List a filterable set of Checks See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListChecks).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_checks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_checks)
@@ -163,15 +163,15 @@
 
     async def list_organization_recommendation_accounts(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListOrganizationRecommendationAccountsResponseTypeDef:
         """
         Lists the accounts that own the resources for an organization aggregate
         recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendation_accounts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_organization_recommendation_accounts)
@@ -181,15 +181,15 @@
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regionCode: str = ...,
-        status: ResourceStatusType = ...
+        status: ResourceStatusType = ...,
     ) -> ListOrganizationRecommendationResourcesResponseTypeDef:
         """
         List Resources of a Recommendation within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendation_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_organization_recommendation_resources)
         """
@@ -202,15 +202,15 @@
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
-        type: RecommendationTypeType = ...
+        type: RecommendationTypeType = ...,
     ) -> ListOrganizationRecommendationsResponseTypeDef:
         """
         List a filterable set of Recommendations within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_organization_recommendations)
         """
@@ -218,15 +218,15 @@
     async def list_recommendation_resources(
         self,
         *,
         recommendationIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
         regionCode: str = ...,
-        status: ResourceStatusType = ...
+        status: ResourceStatusType = ...,
     ) -> ListRecommendationResourcesResponseTypeDef:
         """
         List Resources of a Recommendation See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListRecommendationResources).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_recommendation_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_recommendation_resources)
@@ -240,15 +240,15 @@
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
-        type: RecommendationTypeType = ...
+        type: RecommendationTypeType = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         List a filterable set of Recommendations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListRecommendations).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#list_recommendations)
@@ -256,30 +256,30 @@
 
     async def update_organization_recommendation_lifecycle(
         self,
         *,
         lifecycleStage: UpdateRecommendationLifecycleStageType,
         organizationRecommendationIdentifier: str,
         updateReason: str = ...,
-        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...
+        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update the lifecyle of a Recommendation within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.update_organization_recommendation_lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#update_organization_recommendation_lifecycle)
         """
 
     async def update_recommendation_lifecycle(
         self,
         *,
         lifecycleStage: UpdateRecommendationLifecycleStageType,
         recommendationIdentifier: str,
         updateReason: str = ...,
-        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...
+        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update the lifecyle of a Recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.update_recommendation_lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/client/#update_recommendation_lifecycle)
         """
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/literals.py` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/literals.py`

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
     "ListChecksPaginatorName",
     "ListOrganizationRecommendationAccountsPaginatorName",
     "ListOrganizationRecommendationResourcesPaginatorName",
     "ListOrganizationRecommendationsPaginatorName",
     "ListRecommendationResourcesPaginatorName",
     "ListRecommendationsPaginatorName",
@@ -38,15 +37,14 @@
     "UpdateRecommendationLifecycleStageType",
     "TrustedAdvisorPublicAPIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ListChecksPaginatorName = Literal["list_checks"]
 ListOrganizationRecommendationAccountsPaginatorName = Literal[
     "list_organization_recommendation_accounts"
 ]
 ListOrganizationRecommendationResourcesPaginatorName = Literal[
     "list_organization_recommendation_resources"
 ]
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/literals.pyi` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/paginator.py` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     "ListOrganizationRecommendationAccountsPaginator",
     "ListOrganizationRecommendationResourcesPaginator",
     "ListOrganizationRecommendationsPaginator",
     "ListRecommendationResourcesPaginator",
     "ListRecommendationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -84,15 +83,15 @@
     def paginate(
         self,
         *,
         awsService: str = ...,
         language: RecommendationLanguageType = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListChecks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listcheckspaginator)
         """
 
 
@@ -103,15 +102,15 @@
     """
 
     def paginate(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationRecommendationAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listorganizationrecommendationaccountspaginator)
         """
 
 
@@ -124,15 +123,15 @@
     def paginate(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
         regionCode: str = ...,
         status: ResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationRecommendationResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listorganizationrecommendationresourcespaginator)
         """
 
 
@@ -149,15 +148,15 @@
         awsService: str = ...,
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
         type: RecommendationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listorganizationrecommendationspaginator)
         """
 
 
@@ -169,15 +168,15 @@
 
     def paginate(
         self,
         *,
         recommendationIdentifier: str,
         regionCode: str = ...,
         status: ResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendationResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listrecommendationresourcespaginator)
         """
 
 
@@ -194,13 +193,13 @@
         awsService: str = ...,
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
         type: RecommendationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listrecommendationspaginator)
         """
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/paginator.pyi` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     def paginate(
         self,
         *,
         awsService: str = ...,
         language: RecommendationLanguageType = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListChecks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listcheckspaginator)
         """
 
 class ListOrganizationRecommendationAccountsPaginator(AioPaginator):
@@ -99,15 +99,15 @@
     """
 
     def paginate(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationRecommendationAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listorganizationrecommendationaccountspaginator)
         """
 
 class ListOrganizationRecommendationResourcesPaginator(AioPaginator):
@@ -119,15 +119,15 @@
     def paginate(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
         regionCode: str = ...,
         status: ResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationRecommendationResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listorganizationrecommendationresourcespaginator)
         """
 
 class ListOrganizationRecommendationsPaginator(AioPaginator):
@@ -143,15 +143,15 @@
         awsService: str = ...,
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
         type: RecommendationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listorganizationrecommendationspaginator)
         """
 
 class ListRecommendationResourcesPaginator(AioPaginator):
@@ -162,15 +162,15 @@
 
     def paginate(
         self,
         *,
         recommendationIdentifier: str,
         regionCode: str = ...,
         status: ResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendationResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listrecommendationresourcespaginator)
         """
 
 class ListRecommendationsPaginator(AioPaginator):
@@ -186,13 +186,13 @@
         awsService: str = ...,
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
         type: RecommendationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/paginators/#listrecommendationspaginator)
         """
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/type_defs.py` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountRecommendationLifecycleSummaryTypeDef",
     "CheckSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "GetOrganizationRecommendationRequestRequestTypeDef",
     "GetRecommendationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor/type_defs.pyi` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/PKG-INFO` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-trustedadvisor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TrustedAdvisorPublicAPI 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TrustedAdvisorPublicAPI 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/
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
 
 <a id="types-aiobotocore-trustedadvisor"></a>
 
 # types-aiobotocore-trustedadvisor
 
 [![PyPI - types-aiobotocore-trustedadvisor](https://img.shields.io/pypi/v/types-aiobotocore-trustedadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-trustedadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-trustedadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-trustedadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-trustedadvisor)](https://pepy.tech/project/types-aiobotocore-trustedadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TrustedAdvisorPublicAPI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
+[aiobotocore.TrustedAdvisorPublicAPI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
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
 [types-aiobotocore-trustedadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_trustedadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-trustedadvisor-2.9.0/types_aiobotocore_trustedadvisor.egg-info/SOURCES.txt` & `types-aiobotocore-trustedadvisor-2.9.1/types_aiobotocore_trustedadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

