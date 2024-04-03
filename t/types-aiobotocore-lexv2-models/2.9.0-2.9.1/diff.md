# Comparing `tmp/types-aiobotocore-lexv2-models-2.9.0.tar.gz` & `tmp/types-aiobotocore-lexv2-models-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lexv2-models-2.9.0.tar", last modified: Wed Dec 13 19:59:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-lexv2-models-2.9.1.tar", last modified: Thu Jan 18 01:21:07 2024, max compression
```

## Comparing `types-aiobotocore-lexv2-models-2.9.0.tar` & `types-aiobotocore-lexv2-models-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:44.433536 types-aiobotocore-lexv2-models-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:02.000000 types-aiobotocore-lexv2-models-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14247 2023-12-13 19:59:44.433536 types-aiobotocore-lexv2-models-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12665 2023-12-13 19:49:02.000000 types-aiobotocore-lexv2-models-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:44.433536 types-aiobotocore-lexv2-models-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-13 19:49:02.000000 types-aiobotocore-lexv2-models-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:44.433536 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-12-13 19:49:02.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:49:02.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-13 19:49:02.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79766 2023-12-13 19:49:03.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    79762 2023-12-13 19:49:03.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20338 2023-12-13 19:49:05.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    20336 2023-12-13 19:49:03.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:02.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   148270 2023-12-13 19:49:08.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   148269 2023-12-13 19:49:06.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:02.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2023-12-13 19:49:03.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2023-12-13 19:49:03.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:44.433536 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14247 2023-12-13 19:59:44.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-12-13 19:59:44.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:44.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:44.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:44.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:44.000000 types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:07.025223 types-aiobotocore-lexv2-models-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:49.000000 types-aiobotocore-lexv2-models-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-01-18 01:21:07.025223 types-aiobotocore-lexv2-models-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-01-18 01:10:49.000000 types-aiobotocore-lexv2-models-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:07.025223 types-aiobotocore-lexv2-models-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-18 01:10:49.000000 types-aiobotocore-lexv2-models-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:07.021223 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-01-18 01:10:49.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-01-18 01:10:49.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 01:10:49.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79814 2024-01-18 01:10:52.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79811 2024-01-18 01:10:50.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-01-18 01:10:52.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-01-18 01:10:52.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:49.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   148269 2024-01-18 01:10:55.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148269 2024-01-18 01:10:54.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:49.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-01-18 01:10:52.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-01-18 01:10:52.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:07.025223 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-01-18 01:21:06.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-18 01:21:06.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:06.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:06.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:06.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:06.000000 types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/LICENSE` & `types-aiobotocore-lexv2-models-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lexv2-models-2.9.0/PKG-INFO` & `types-aiobotocore-lexv2-models-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lexv2-models
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LexModelsV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LexModelsV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/
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
 
 <a id="types-aiobotocore-lexv2-models"></a>
 
 # types-aiobotocore-lexv2-models
 
 [![PyPI - types-aiobotocore-lexv2-models](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-models)](https://pepy.tech/project/types-aiobotocore-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelsV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[aiobotocore.LexModelsV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
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
 [types-aiobotocore-lexv2-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/README.md` & `types-aiobotocore-lexv2-models-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-models)](https://pepy.tech/project/types-aiobotocore-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelsV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[aiobotocore.LexModelsV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
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
 [types-aiobotocore-lexv2-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/setup.py` & `types-aiobotocore-lexv2-models-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lexv2-models",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lexv2_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LexModelsV2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LexModelsV2 2.9.1 service generated with"
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
     keywords="aiobotocore lexv2-models type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lexv2_models": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/__init__.py` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     BotLocaleCreatedWaiter,
     BotLocaleExpressTestingAvailableWaiter,
     BotVersionAvailableWaiter,
 )
 
 Client = LexModelsV2Client
 
-
 __all__ = (
     "BotAliasAvailableWaiter",
     "BotAvailableWaiter",
     "BotExportCompletedWaiter",
     "BotImportCompletedWaiter",
     "BotLocaleBuiltWaiter",
     "BotLocaleCreatedWaiter",
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/__init__.pyi` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/__main__.py` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexModelsV2 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LexModelsV2 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2\nOther"
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

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/client.py` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LexModelsV2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -261,15 +260,15 @@
 
     async def batch_create_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef]
+        customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef],
     ) -> BatchCreateCustomVocabularyItemResponseTypeDef:
         """
         Create a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_create_custom_vocabulary_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#batch_create_custom_vocabulary_item)
@@ -277,15 +276,15 @@
 
     async def batch_delete_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef]
+        customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef],
     ) -> BatchDeleteCustomVocabularyItemResponseTypeDef:
         """
         Delete a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_delete_custom_vocabulary_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#batch_delete_custom_vocabulary_item)
@@ -293,15 +292,15 @@
 
     async def batch_update_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef]
+        customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef],
     ) -> BatchUpdateCustomVocabularyItemResponseTypeDef:
         """
         Update a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_update_custom_vocabulary_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#batch_update_custom_vocabulary_item)
@@ -340,15 +339,15 @@
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
         description: str = ...,
         botTags: Mapping[str, str] = ...,
         testBotAliasTags: Mapping[str, str] = ...,
         botType: BotTypeType = ...,
-        botMembers: Sequence[BotMemberTypeDef] = ...
+        botMembers: Sequence[BotMemberTypeDef] = ...,
     ) -> CreateBotResponseTypeDef:
         """
         Creates an Amazon Lex conversational bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_bot)
         """
@@ -359,15 +358,15 @@
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
         conversationLogSettings: ConversationLogSettingsTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_bot_alias)
         """
@@ -377,43 +376,43 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         nluIntentConfidenceThreshold: float,
         description: str = ...,
         voiceSettings: VoiceSettingsTypeDef = ...,
-        generativeAISettings: GenerativeAISettingsTypeDef = ...
+        generativeAISettings: GenerativeAISettingsTypeDef = ...,
     ) -> CreateBotLocaleResponseTypeDef:
         """
         Creates a locale in the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_locale)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_bot_locale)
         """
 
     async def create_bot_version(
         self,
         *,
         botId: str,
         botVersionLocaleSpecification: Mapping[str, BotVersionLocaleDetailsTypeDef],
-        description: str = ...
+        description: str = ...,
     ) -> CreateBotVersionResponseTypeDef:
         """
         Creates an immutable version of the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_bot_version)
         """
 
     async def create_export(
         self,
         *,
         resourceSpecification: ExportResourceSpecificationTypeDef,
         fileFormat: ImportExportFileFormatType,
-        filePassword: str = ...
+        filePassword: str = ...,
     ) -> CreateExportResponseTypeDef:
         """
         Creates a zip archive containing the contents of a bot or a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_export)
         """
@@ -431,15 +430,15 @@
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
         fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
         intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
         intentClosingSetting: IntentClosingSettingTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingTypeDef = ...
+        initialResponseSetting: InitialResponseSettingTypeDef = ...,
     ) -> CreateIntentResponseTypeDef:
         """
         Creates an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_intent)
         """
@@ -459,15 +458,15 @@
         *,
         resourceArn: str,
         statementId: str,
         effect: EffectType,
         principal: Sequence[PrincipalTypeDef],
         action: Sequence[str],
         condition: Mapping[str, Mapping[str, str]] = ...,
-        expectedRevisionId: str = ...
+        expectedRevisionId: str = ...,
     ) -> CreateResourcePolicyStatementResponseTypeDef:
         """
         Adds a new resource policy statement to a bot or bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_resource_policy_statement)
         """
@@ -481,15 +480,15 @@
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingTypeDef = ...
+        subSlotSetting: SubSlotSettingTypeDef = ...,
     ) -> CreateSlotResponseTypeDef:
         """
         Creates a slot in an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_slot)
         """
@@ -502,15 +501,15 @@
         botVersion: str,
         localeId: str,
         description: str = ...,
         slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...,
     ) -> CreateSlotTypeResponseTypeDef:
         """
         Creates a custom slot type To create a custom slot type, specify a name for the
         slot type and a set of enumeration values, the values that a slot of this type
         can
         assume.
 
@@ -647,15 +646,15 @@
     async def delete_slot_type(
         self,
         *,
         slotTypeId: str,
         botId: str,
         botVersion: str,
         localeId: str,
-        skipResourceInUseCheck: bool = ...
+        skipResourceInUseCheck: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a slot type from a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#delete_slot_type)
         """
@@ -883,15 +882,15 @@
         localeId: str,
         aggregationDuration: UtteranceAggregationDurationTypeDef,
         botAliasId: str = ...,
         botVersion: str = ...,
         sortBy: AggregatedUtterancesSortByTypeDef = ...,
         filters: Sequence[AggregatedUtterancesFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAggregatedUtterancesResponseTypeDef:
         """
         Provides a list of utterances that users have sent to the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_aggregated_utterances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_aggregated_utterances)
         """
@@ -910,15 +909,15 @@
         self,
         *,
         botId: str,
         botVersion: str,
         sortBy: BotLocaleSortByTypeDef = ...,
         filters: Sequence[BotLocaleFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotLocalesResponseTypeDef:
         """
         Gets a list of locales for the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_locales)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bot_locales)
         """
@@ -926,15 +925,15 @@
     async def list_bot_recommendations(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotRecommendationsResponseTypeDef:
         """
         Get a list of bot recommendations that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bot_recommendations)
         """
@@ -943,60 +942,60 @@
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: GenerationSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotResourceGenerationsResponseTypeDef:
         """
         Lists the generation requests made for a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_resource_generations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bot_resource_generations)
         """
 
     async def list_bot_versions(
         self,
         *,
         botId: str,
         sortBy: BotVersionSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotVersionsResponseTypeDef:
         """
         Gets information about all of the versions of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bot_versions)
         """
 
     async def list_bots(
         self,
         *,
         sortBy: BotSortByTypeDef = ...,
         filters: Sequence[BotFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotsResponseTypeDef:
         """
         Gets a list of available bots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bots)
         """
 
     async def list_built_in_intents(
         self,
         *,
         localeId: str,
         sortBy: BuiltInIntentSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBuiltInIntentsResponseTypeDef:
         """
         Gets a list of built-in intents provided by Amazon Lex that you can use in your
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_intents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_built_in_intents)
@@ -1004,15 +1003,15 @@
 
     async def list_built_in_slot_types(
         self,
         *,
         localeId: str,
         sortBy: BuiltInSlotTypeSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBuiltInSlotTypesResponseTypeDef:
         """
         Gets a list of built-in slot types that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_slot_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_built_in_slot_types)
         """
@@ -1020,15 +1019,15 @@
     async def list_custom_vocabulary_items(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCustomVocabularyItemsResponseTypeDef:
         """
         Paginated list of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_custom_vocabulary_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_custom_vocabulary_items)
@@ -1039,15 +1038,15 @@
         *,
         botId: str = ...,
         botVersion: str = ...,
         sortBy: ExportSortByTypeDef = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        localeId: str = ...
+        localeId: str = ...,
     ) -> ListExportsResponseTypeDef:
         """
         Lists the exports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_exports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_exports)
         """
@@ -1057,15 +1056,15 @@
         *,
         botId: str = ...,
         botVersion: str = ...,
         sortBy: ImportSortByTypeDef = ...,
         filters: Sequence[ImportFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        localeId: str = ...
+        localeId: str = ...,
     ) -> ListImportsResponseTypeDef:
         """
         Lists the imports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_imports)
         """
@@ -1077,15 +1076,15 @@
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         metrics: Sequence[AnalyticsIntentMetricTypeDef],
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsIntentGroupBySpecificationTypeDef] = ...,
         filters: Sequence[AnalyticsIntentFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIntentMetricsResponseTypeDef:
         """
         Retrieves summary metrics for the intents in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_metrics)
         """
@@ -1093,15 +1092,15 @@
     async def list_intent_paths(
         self,
         *,
         botId: str,
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         intentPath: str,
-        filters: Sequence[AnalyticsPathFilterTypeDef] = ...
+        filters: Sequence[AnalyticsPathFilterTypeDef] = ...,
     ) -> ListIntentPathsResponseTypeDef:
         """
         Retrieves summary statistics for a path of intents that users take over
         sessions with your
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_paths)
@@ -1115,15 +1114,15 @@
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         metrics: Sequence[AnalyticsIntentStageMetricTypeDef],
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,
         filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIntentStageMetricsResponseTypeDef:
         """
         Retrieves summary metrics for the stages within intents in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_stage_metrics)
         """
@@ -1133,15 +1132,15 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: IntentSortByTypeDef = ...,
         filters: Sequence[IntentFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIntentsResponseTypeDef:
         """
         Get a list of intents that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intents)
         """
@@ -1150,15 +1149,15 @@
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListRecommendedIntentsResponseTypeDef:
         """
         Gets a list of recommended intents provided by the bot recommendation that you
         can use in your
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_recommended_intents)
@@ -1170,15 +1169,15 @@
         *,
         botId: str,
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         sortBy: SessionDataSortByTypeDef = ...,
         filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSessionAnalyticsDataResponseTypeDef:
         """
         Retrieves a list of metadata for individual user sessions with your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_analytics_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_session_analytics_data)
         """
@@ -1190,15 +1189,15 @@
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         metrics: Sequence[AnalyticsSessionMetricTypeDef],
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsSessionGroupBySpecificationTypeDef] = ...,
         filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSessionMetricsResponseTypeDef:
         """
         Retrieves summary metrics for the user sessions with your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_session_metrics)
         """
@@ -1208,15 +1207,15 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: SlotTypeSortByTypeDef = ...,
         filters: Sequence[SlotTypeFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSlotTypesResponseTypeDef:
         """
         Gets a list of slot types that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slot_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_slot_types)
         """
@@ -1227,15 +1226,15 @@
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         sortBy: SlotSortByTypeDef = ...,
         filters: Sequence[SlotFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSlotsResponseTypeDef:
         """
         Gets a list of slots that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_slots)
         """
@@ -1252,29 +1251,29 @@
 
     async def list_test_execution_result_items(
         self,
         *,
         testExecutionId: str,
         resultFilterBy: TestExecutionResultFilterByTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTestExecutionResultItemsResponseTypeDef:
         """
         Gets a list of test execution result items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_execution_result_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_test_execution_result_items)
         """
 
     async def list_test_executions(
         self,
         *,
         sortBy: TestExecutionSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTestExecutionsResponseTypeDef:
         """
         The list of test set executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_test_executions)
         """
@@ -1305,15 +1304,15 @@
         *,
         botId: str,
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         sortBy: UtteranceDataSortByTypeDef = ...,
         filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListUtteranceAnalyticsDataResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_utterance_analytics_data)
         """
@@ -1326,15 +1325,15 @@
         endDateTime: TimestampTypeDef,
         metrics: Sequence[AnalyticsUtteranceMetricTypeDef],
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,
         attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,
         filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListUtteranceMetricsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_utterance_metrics)
         """
@@ -1345,15 +1344,15 @@
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
         filters: Sequence[AssociatedTranscriptFilterTypeDef],
         searchOrder: SearchOrderType = ...,
         maxResults: int = ...,
-        nextIndex: int = ...
+        nextIndex: int = ...,
     ) -> SearchAssociatedTranscriptsResponseTypeDef:
         """
         Search for associated transcripts that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.search_associated_transcripts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#search_associated_transcripts)
         """
@@ -1361,15 +1360,15 @@
     async def start_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         transcriptSourceSetting: TranscriptSourceSettingTypeDef,
-        encryptionSetting: EncryptionSettingTypeDef = ...
+        encryptionSetting: EncryptionSettingTypeDef = ...,
     ) -> StartBotRecommendationResponseTypeDef:
         """
         Use this to provide your transcript data, and to start the bot recommendation
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_bot_recommendation)
@@ -1389,15 +1388,15 @@
 
     async def start_import(
         self,
         *,
         importId: str,
         resourceSpecification: ImportResourceSpecificationTypeDef,
         mergeStrategy: MergeStrategyType,
-        filePassword: str = ...
+        filePassword: str = ...,
     ) -> StartImportResponseTypeDef:
         """
         Starts importing a bot, bot locale, or custom vocabulary from a zip archive
         that you uploaded to an S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_import)
@@ -1406,15 +1405,15 @@
 
     async def start_test_execution(
         self,
         *,
         testSetId: str,
         target: TestExecutionTargetTypeDef,
         apiMode: TestExecutionApiModeType,
-        testExecutionModality: TestExecutionModalityType = ...
+        testExecutionModality: TestExecutionModalityType = ...,
     ) -> StartTestExecutionResponseTypeDef:
         """
         The action to start test set execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_test_execution)
         """
@@ -1423,15 +1422,15 @@
         self,
         *,
         testSetName: str,
         storageLocation: TestSetStorageLocationTypeDef,
         generationDataSource: TestSetGenerationDataSourceTypeDef,
         roleArn: str,
         description: str = ...,
-        testSetTags: Mapping[str, str] = ...
+        testSetTags: Mapping[str, str] = ...,
     ) -> StartTestSetGenerationResponseTypeDef:
         """
         The action to start the generation of test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_set_generation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_test_set_generation)
         """
@@ -1468,15 +1467,15 @@
         botId: str,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
         description: str = ...,
         botType: BotTypeType = ...,
-        botMembers: Sequence[BotMemberTypeDef] = ...
+        botMembers: Sequence[BotMemberTypeDef] = ...,
     ) -> UpdateBotResponseTypeDef:
         """
         Updates the configuration of an existing bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot)
         """
@@ -1487,15 +1486,15 @@
         botAliasId: str,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
         conversationLogSettings: ConversationLogSettingsTypeDef = ...,
-        sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...
+        sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,
     ) -> UpdateBotAliasResponseTypeDef:
         """
         Updates the configuration of an existing bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_alias)
         """
@@ -1505,15 +1504,15 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         nluIntentConfidenceThreshold: float,
         description: str = ...,
         voiceSettings: VoiceSettingsTypeDef = ...,
-        generativeAISettings: GenerativeAISettingsTypeDef = ...
+        generativeAISettings: GenerativeAISettingsTypeDef = ...,
     ) -> UpdateBotLocaleResponseTypeDef:
         """
         Updates the settings that a bot has for a specific locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_locale)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_locale)
         """
@@ -1521,15 +1520,15 @@
     async def update_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
-        encryptionSetting: EncryptionSettingTypeDef
+        encryptionSetting: EncryptionSettingTypeDef,
     ) -> UpdateBotRecommendationResponseTypeDef:
         """
         Updates an existing bot recommendation request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_recommendation)
         """
@@ -1559,15 +1558,15 @@
         fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
         slotPriorities: Sequence[SlotPriorityTypeDef] = ...,
         intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
         intentClosingSetting: IntentClosingSettingTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingTypeDef = ...
+        initialResponseSetting: InitialResponseSettingTypeDef = ...,
     ) -> UpdateIntentResponseTypeDef:
         """
         Updates the settings for an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_intent)
         """
@@ -1592,15 +1591,15 @@
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingTypeDef = ...
+        subSlotSetting: SubSlotSettingTypeDef = ...,
     ) -> UpdateSlotResponseTypeDef:
         """
         Updates the settings for a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot)
         """
@@ -1614,15 +1613,15 @@
         botVersion: str,
         localeId: str,
         description: str = ...,
         slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...,
     ) -> UpdateSlotTypeResponseTypeDef:
         """
         Updates the configuration of an existing slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot_type)
         """
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/client.pyi` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 
     async def batch_create_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef]
+        customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef],
     ) -> BatchCreateCustomVocabularyItemResponseTypeDef:
         """
         Create a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_create_custom_vocabulary_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#batch_create_custom_vocabulary_item)
@@ -273,15 +273,15 @@
 
     async def batch_delete_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef]
+        customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef],
     ) -> BatchDeleteCustomVocabularyItemResponseTypeDef:
         """
         Delete a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_delete_custom_vocabulary_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#batch_delete_custom_vocabulary_item)
@@ -289,15 +289,15 @@
 
     async def batch_update_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef]
+        customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef],
     ) -> BatchUpdateCustomVocabularyItemResponseTypeDef:
         """
         Update a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_update_custom_vocabulary_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#batch_update_custom_vocabulary_item)
@@ -336,15 +336,15 @@
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
         description: str = ...,
         botTags: Mapping[str, str] = ...,
         testBotAliasTags: Mapping[str, str] = ...,
         botType: BotTypeType = ...,
-        botMembers: Sequence[BotMemberTypeDef] = ...
+        botMembers: Sequence[BotMemberTypeDef] = ...,
     ) -> CreateBotResponseTypeDef:
         """
         Creates an Amazon Lex conversational bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_bot)
         """
@@ -355,15 +355,15 @@
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
         conversationLogSettings: ConversationLogSettingsTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_bot_alias)
         """
@@ -373,43 +373,43 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         nluIntentConfidenceThreshold: float,
         description: str = ...,
         voiceSettings: VoiceSettingsTypeDef = ...,
-        generativeAISettings: GenerativeAISettingsTypeDef = ...
+        generativeAISettings: GenerativeAISettingsTypeDef = ...,
     ) -> CreateBotLocaleResponseTypeDef:
         """
         Creates a locale in the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_locale)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_bot_locale)
         """
 
     async def create_bot_version(
         self,
         *,
         botId: str,
         botVersionLocaleSpecification: Mapping[str, BotVersionLocaleDetailsTypeDef],
-        description: str = ...
+        description: str = ...,
     ) -> CreateBotVersionResponseTypeDef:
         """
         Creates an immutable version of the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_bot_version)
         """
 
     async def create_export(
         self,
         *,
         resourceSpecification: ExportResourceSpecificationTypeDef,
         fileFormat: ImportExportFileFormatType,
-        filePassword: str = ...
+        filePassword: str = ...,
     ) -> CreateExportResponseTypeDef:
         """
         Creates a zip archive containing the contents of a bot or a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_export)
         """
@@ -427,15 +427,15 @@
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
         fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
         intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
         intentClosingSetting: IntentClosingSettingTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingTypeDef = ...
+        initialResponseSetting: InitialResponseSettingTypeDef = ...,
     ) -> CreateIntentResponseTypeDef:
         """
         Creates an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_intent)
         """
@@ -455,15 +455,15 @@
         *,
         resourceArn: str,
         statementId: str,
         effect: EffectType,
         principal: Sequence[PrincipalTypeDef],
         action: Sequence[str],
         condition: Mapping[str, Mapping[str, str]] = ...,
-        expectedRevisionId: str = ...
+        expectedRevisionId: str = ...,
     ) -> CreateResourcePolicyStatementResponseTypeDef:
         """
         Adds a new resource policy statement to a bot or bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_resource_policy_statement)
         """
@@ -477,15 +477,15 @@
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingTypeDef = ...
+        subSlotSetting: SubSlotSettingTypeDef = ...,
     ) -> CreateSlotResponseTypeDef:
         """
         Creates a slot in an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_slot)
         """
@@ -498,15 +498,15 @@
         botVersion: str,
         localeId: str,
         description: str = ...,
         slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...,
     ) -> CreateSlotTypeResponseTypeDef:
         """
         Creates a custom slot type To create a custom slot type, specify a name for the
         slot type and a set of enumeration values, the values that a slot of this type
         can
         assume.
 
@@ -643,15 +643,15 @@
     async def delete_slot_type(
         self,
         *,
         slotTypeId: str,
         botId: str,
         botVersion: str,
         localeId: str,
-        skipResourceInUseCheck: bool = ...
+        skipResourceInUseCheck: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a slot type from a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#delete_slot_type)
         """
@@ -879,15 +879,15 @@
         localeId: str,
         aggregationDuration: UtteranceAggregationDurationTypeDef,
         botAliasId: str = ...,
         botVersion: str = ...,
         sortBy: AggregatedUtterancesSortByTypeDef = ...,
         filters: Sequence[AggregatedUtterancesFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAggregatedUtterancesResponseTypeDef:
         """
         Provides a list of utterances that users have sent to the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_aggregated_utterances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_aggregated_utterances)
         """
@@ -906,15 +906,15 @@
         self,
         *,
         botId: str,
         botVersion: str,
         sortBy: BotLocaleSortByTypeDef = ...,
         filters: Sequence[BotLocaleFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotLocalesResponseTypeDef:
         """
         Gets a list of locales for the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_locales)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bot_locales)
         """
@@ -922,15 +922,15 @@
     async def list_bot_recommendations(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotRecommendationsResponseTypeDef:
         """
         Get a list of bot recommendations that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bot_recommendations)
         """
@@ -939,60 +939,60 @@
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: GenerationSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotResourceGenerationsResponseTypeDef:
         """
         Lists the generation requests made for a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_resource_generations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bot_resource_generations)
         """
 
     async def list_bot_versions(
         self,
         *,
         botId: str,
         sortBy: BotVersionSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotVersionsResponseTypeDef:
         """
         Gets information about all of the versions of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bot_versions)
         """
 
     async def list_bots(
         self,
         *,
         sortBy: BotSortByTypeDef = ...,
         filters: Sequence[BotFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBotsResponseTypeDef:
         """
         Gets a list of available bots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_bots)
         """
 
     async def list_built_in_intents(
         self,
         *,
         localeId: str,
         sortBy: BuiltInIntentSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBuiltInIntentsResponseTypeDef:
         """
         Gets a list of built-in intents provided by Amazon Lex that you can use in your
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_intents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_built_in_intents)
@@ -1000,15 +1000,15 @@
 
     async def list_built_in_slot_types(
         self,
         *,
         localeId: str,
         sortBy: BuiltInSlotTypeSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBuiltInSlotTypesResponseTypeDef:
         """
         Gets a list of built-in slot types that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_slot_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_built_in_slot_types)
         """
@@ -1016,15 +1016,15 @@
     async def list_custom_vocabulary_items(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCustomVocabularyItemsResponseTypeDef:
         """
         Paginated list of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_custom_vocabulary_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_custom_vocabulary_items)
@@ -1035,15 +1035,15 @@
         *,
         botId: str = ...,
         botVersion: str = ...,
         sortBy: ExportSortByTypeDef = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        localeId: str = ...
+        localeId: str = ...,
     ) -> ListExportsResponseTypeDef:
         """
         Lists the exports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_exports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_exports)
         """
@@ -1053,15 +1053,15 @@
         *,
         botId: str = ...,
         botVersion: str = ...,
         sortBy: ImportSortByTypeDef = ...,
         filters: Sequence[ImportFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        localeId: str = ...
+        localeId: str = ...,
     ) -> ListImportsResponseTypeDef:
         """
         Lists the imports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_imports)
         """
@@ -1073,15 +1073,15 @@
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         metrics: Sequence[AnalyticsIntentMetricTypeDef],
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsIntentGroupBySpecificationTypeDef] = ...,
         filters: Sequence[AnalyticsIntentFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIntentMetricsResponseTypeDef:
         """
         Retrieves summary metrics for the intents in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_metrics)
         """
@@ -1089,15 +1089,15 @@
     async def list_intent_paths(
         self,
         *,
         botId: str,
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         intentPath: str,
-        filters: Sequence[AnalyticsPathFilterTypeDef] = ...
+        filters: Sequence[AnalyticsPathFilterTypeDef] = ...,
     ) -> ListIntentPathsResponseTypeDef:
         """
         Retrieves summary statistics for a path of intents that users take over
         sessions with your
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_paths)
@@ -1111,15 +1111,15 @@
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         metrics: Sequence[AnalyticsIntentStageMetricTypeDef],
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,
         filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIntentStageMetricsResponseTypeDef:
         """
         Retrieves summary metrics for the stages within intents in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_stage_metrics)
         """
@@ -1129,15 +1129,15 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: IntentSortByTypeDef = ...,
         filters: Sequence[IntentFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIntentsResponseTypeDef:
         """
         Get a list of intents that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intents)
         """
@@ -1146,15 +1146,15 @@
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListRecommendedIntentsResponseTypeDef:
         """
         Gets a list of recommended intents provided by the bot recommendation that you
         can use in your
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_recommended_intents)
@@ -1166,15 +1166,15 @@
         *,
         botId: str,
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         sortBy: SessionDataSortByTypeDef = ...,
         filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSessionAnalyticsDataResponseTypeDef:
         """
         Retrieves a list of metadata for individual user sessions with your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_analytics_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_session_analytics_data)
         """
@@ -1186,15 +1186,15 @@
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         metrics: Sequence[AnalyticsSessionMetricTypeDef],
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsSessionGroupBySpecificationTypeDef] = ...,
         filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSessionMetricsResponseTypeDef:
         """
         Retrieves summary metrics for the user sessions with your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_session_metrics)
         """
@@ -1204,15 +1204,15 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: SlotTypeSortByTypeDef = ...,
         filters: Sequence[SlotTypeFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSlotTypesResponseTypeDef:
         """
         Gets a list of slot types that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slot_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_slot_types)
         """
@@ -1223,15 +1223,15 @@
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         sortBy: SlotSortByTypeDef = ...,
         filters: Sequence[SlotFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSlotsResponseTypeDef:
         """
         Gets a list of slots that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_slots)
         """
@@ -1248,29 +1248,29 @@
 
     async def list_test_execution_result_items(
         self,
         *,
         testExecutionId: str,
         resultFilterBy: TestExecutionResultFilterByTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTestExecutionResultItemsResponseTypeDef:
         """
         Gets a list of test execution result items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_execution_result_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_test_execution_result_items)
         """
 
     async def list_test_executions(
         self,
         *,
         sortBy: TestExecutionSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTestExecutionsResponseTypeDef:
         """
         The list of test set executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_test_executions)
         """
@@ -1301,15 +1301,15 @@
         *,
         botId: str,
         startDateTime: TimestampTypeDef,
         endDateTime: TimestampTypeDef,
         sortBy: UtteranceDataSortByTypeDef = ...,
         filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListUtteranceAnalyticsDataResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_utterance_analytics_data)
         """
@@ -1322,15 +1322,15 @@
         endDateTime: TimestampTypeDef,
         metrics: Sequence[AnalyticsUtteranceMetricTypeDef],
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,
         attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,
         filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListUtteranceMetricsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_utterance_metrics)
         """
@@ -1341,15 +1341,15 @@
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
         filters: Sequence[AssociatedTranscriptFilterTypeDef],
         searchOrder: SearchOrderType = ...,
         maxResults: int = ...,
-        nextIndex: int = ...
+        nextIndex: int = ...,
     ) -> SearchAssociatedTranscriptsResponseTypeDef:
         """
         Search for associated transcripts that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.search_associated_transcripts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#search_associated_transcripts)
         """
@@ -1357,15 +1357,15 @@
     async def start_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         transcriptSourceSetting: TranscriptSourceSettingTypeDef,
-        encryptionSetting: EncryptionSettingTypeDef = ...
+        encryptionSetting: EncryptionSettingTypeDef = ...,
     ) -> StartBotRecommendationResponseTypeDef:
         """
         Use this to provide your transcript data, and to start the bot recommendation
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_bot_recommendation)
@@ -1385,15 +1385,15 @@
 
     async def start_import(
         self,
         *,
         importId: str,
         resourceSpecification: ImportResourceSpecificationTypeDef,
         mergeStrategy: MergeStrategyType,
-        filePassword: str = ...
+        filePassword: str = ...,
     ) -> StartImportResponseTypeDef:
         """
         Starts importing a bot, bot locale, or custom vocabulary from a zip archive
         that you uploaded to an S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_import)
@@ -1402,15 +1402,15 @@
 
     async def start_test_execution(
         self,
         *,
         testSetId: str,
         target: TestExecutionTargetTypeDef,
         apiMode: TestExecutionApiModeType,
-        testExecutionModality: TestExecutionModalityType = ...
+        testExecutionModality: TestExecutionModalityType = ...,
     ) -> StartTestExecutionResponseTypeDef:
         """
         The action to start test set execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_test_execution)
         """
@@ -1419,15 +1419,15 @@
         self,
         *,
         testSetName: str,
         storageLocation: TestSetStorageLocationTypeDef,
         generationDataSource: TestSetGenerationDataSourceTypeDef,
         roleArn: str,
         description: str = ...,
-        testSetTags: Mapping[str, str] = ...
+        testSetTags: Mapping[str, str] = ...,
     ) -> StartTestSetGenerationResponseTypeDef:
         """
         The action to start the generation of test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_set_generation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_test_set_generation)
         """
@@ -1464,15 +1464,15 @@
         botId: str,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
         description: str = ...,
         botType: BotTypeType = ...,
-        botMembers: Sequence[BotMemberTypeDef] = ...
+        botMembers: Sequence[BotMemberTypeDef] = ...,
     ) -> UpdateBotResponseTypeDef:
         """
         Updates the configuration of an existing bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot)
         """
@@ -1483,15 +1483,15 @@
         botAliasId: str,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
         conversationLogSettings: ConversationLogSettingsTypeDef = ...,
-        sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...
+        sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,
     ) -> UpdateBotAliasResponseTypeDef:
         """
         Updates the configuration of an existing bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_alias)
         """
@@ -1501,15 +1501,15 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         nluIntentConfidenceThreshold: float,
         description: str = ...,
         voiceSettings: VoiceSettingsTypeDef = ...,
-        generativeAISettings: GenerativeAISettingsTypeDef = ...
+        generativeAISettings: GenerativeAISettingsTypeDef = ...,
     ) -> UpdateBotLocaleResponseTypeDef:
         """
         Updates the settings that a bot has for a specific locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_locale)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_locale)
         """
@@ -1517,15 +1517,15 @@
     async def update_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
-        encryptionSetting: EncryptionSettingTypeDef
+        encryptionSetting: EncryptionSettingTypeDef,
     ) -> UpdateBotRecommendationResponseTypeDef:
         """
         Updates an existing bot recommendation request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_recommendation)
         """
@@ -1555,15 +1555,15 @@
         fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
         slotPriorities: Sequence[SlotPriorityTypeDef] = ...,
         intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
         intentClosingSetting: IntentClosingSettingTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingTypeDef = ...
+        initialResponseSetting: InitialResponseSettingTypeDef = ...,
     ) -> UpdateIntentResponseTypeDef:
         """
         Updates the settings for an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_intent)
         """
@@ -1588,15 +1588,15 @@
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingTypeDef = ...
+        subSlotSetting: SubSlotSettingTypeDef = ...,
     ) -> UpdateSlotResponseTypeDef:
         """
         Updates the settings for a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot)
         """
@@ -1610,15 +1610,15 @@
         botVersion: str,
         localeId: str,
         description: str = ...,
         slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...,
     ) -> UpdateSlotTypeResponseTypeDef:
         """
         Updates the configuration of an existing slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot_type)
         """
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/literals.py` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/literals.py`

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
     "AggregatedUtterancesFilterNameType",
     "AggregatedUtterancesFilterOperatorType",
     "AggregatedUtterancesSortAttributeType",
     "AnalyticsBinByNameType",
     "AnalyticsCommonFilterNameType",
     "AnalyticsFilterOperatorType",
@@ -128,15 +127,14 @@
     "LexModelsV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "WaiterName",
     "RegionName",
 )
 
-
 AggregatedUtterancesFilterNameType = Literal["Utterance"]
 AggregatedUtterancesFilterOperatorType = Literal["CO", "EQ"]
 AggregatedUtterancesSortAttributeType = Literal["HitCount", "MissedCount"]
 AnalyticsBinByNameType = Literal["ConversationStartTime", "UtteranceTimestamp"]
 AnalyticsCommonFilterNameType = Literal[
     "BotAliasId", "BotVersion", "Channel", "LocaleId", "Modality"
 ]
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/literals.pyi` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/type_defs.py` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveContextTypeDef",
     "AdvancedRecognitionSettingTypeDef",
     "ExecutionErrorDetailsTypeDef",
     "AgentTurnSpecificationTypeDef",
     "AggregatedUtterancesFilterTypeDef",
     "AggregatedUtterancesSortByTypeDef",
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/type_defs.pyi` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/waiter.py` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models/waiter.pyi` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/PKG-INFO` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lexv2-models
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LexModelsV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LexModelsV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/
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
 
 <a id="types-aiobotocore-lexv2-models"></a>
 
 # types-aiobotocore-lexv2-models
 
 [![PyPI - types-aiobotocore-lexv2-models](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-models)](https://pepy.tech/project/types-aiobotocore-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelsV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[aiobotocore.LexModelsV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
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
 [types-aiobotocore-lexv2-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lexv2-models-2.9.0/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt` & `types-aiobotocore-lexv2-models-2.9.1/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

