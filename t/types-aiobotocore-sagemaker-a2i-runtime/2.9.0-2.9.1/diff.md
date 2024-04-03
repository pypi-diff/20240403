# Comparing `tmp/types-aiobotocore-sagemaker-a2i-runtime-2.9.0.tar.gz` & `tmp/types-aiobotocore-sagemaker-a2i-runtime-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-a2i-runtime-2.9.0.tar", last modified: Wed Dec 13 20:00:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-a2i-runtime-2.9.1.tar", last modified: Thu Jan 18 01:21:42 2024, max compression
```

## Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0.tar` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.789195 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13771 2023-12-13 20:00:23.789195 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12155 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:23.789195 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.789195 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:41.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.789195 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13771 2023-12-13 20:00:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-13 20:00:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-13 20:00:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.789062 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-01-18 01:21:42.789062 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:42.789062 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.789062 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-01-18 01:17:16.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-01-18 01:17:16.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-01-18 01:17:16.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-01-18 01:17:16.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.789062 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-01-18 01:21:42.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-18 01:21:42.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:42.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:42.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:42.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-18 01:21:42.000000 types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/LICENSE` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/PKG-INFO` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-a2i-runtime
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/
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
 
 <a id="types-aiobotocore-sagemaker-a2i-runtime"></a>
 
 # types-aiobotocore-sagemaker-a2i-runtime
 
 [![PyPI - types-aiobotocore-sagemaker-a2i-runtime](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-a2i-runtime)](https://pepy.tech/project/types-aiobotocore-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AugmentedAIRuntime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[aiobotocore.AugmentedAIRuntime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/README.md` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-a2i-runtime)](https://pepy.tech/project/types-aiobotocore-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AugmentedAIRuntime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[aiobotocore.AugmentedAIRuntime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/setup.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-a2i-runtime",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sagemaker_a2i_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AugmentedAIRuntime 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AugmentedAIRuntime 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore sagemaker-a2i-runtime type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sagemaker_a2i_runtime": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/__init__.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import AugmentedAIRuntimeClient
 from .paginator import ListHumanLoopsPaginator
 
 Client = AugmentedAIRuntimeClient
 
-
 __all__ = ("AugmentedAIRuntimeClient", "Client", "ListHumanLoopsPaginator")
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/__main__.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AugmentedAIRuntime 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AugmentedAIRuntime 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime\nOther"
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

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/client.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AugmentedAIRuntimeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -126,30 +125,30 @@
         self,
         *,
         FlowDefinitionArn: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListHumanLoopsResponseTypeDef:
         """
         Returns information about human loops, given the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#list_human_loops)
         """
 
     async def start_human_loop(
         self,
         *,
         HumanLoopName: str,
         FlowDefinitionArn: str,
         HumanLoopInput: HumanLoopInputTypeDef,
-        DataAttributes: HumanLoopDataAttributesTypeDef = ...
+        DataAttributes: HumanLoopDataAttributesTypeDef = ...,
     ) -> StartHumanLoopResponseTypeDef:
         """
         Starts a human loop, provided that at least one activation condition is met.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#start_human_loop)
         """
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/client.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -122,30 +122,30 @@
         self,
         *,
         FlowDefinitionArn: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListHumanLoopsResponseTypeDef:
         """
         Returns information about human loops, given the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#list_human_loops)
         """
 
     async def start_human_loop(
         self,
         *,
         HumanLoopName: str,
         FlowDefinitionArn: str,
         HumanLoopInput: HumanLoopInputTypeDef,
-        DataAttributes: HumanLoopDataAttributesTypeDef = ...
+        DataAttributes: HumanLoopDataAttributesTypeDef = ...,
     ) -> StartHumanLoopResponseTypeDef:
         """
         Starts a human loop, provided that at least one activation condition is met.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#start_human_loop)
         """
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/literals.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ContentClassifierType",
     "HumanLoopStatusType",
     "ListHumanLoopsPaginatorName",
     "SortOrderType",
     "AugmentedAIRuntimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ContentClassifierType = Literal["FreeOfAdultContent", "FreeOfPersonallyIdentifiableInformation"]
 HumanLoopStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 ListHumanLoopsPaginatorName = Literal["list_human_loops"]
 SortOrderType = Literal["Ascending", "Descending"]
 AugmentedAIRuntimeServiceName = Literal["sagemaker-a2i-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/paginator.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from botocore.paginate import PageIterator
 
 from .literals import SortOrderType
 from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListHumanLoopsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -51,13 +50,13 @@
     def paginate(
         self,
         *,
         FlowDefinitionArn: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHumanLoopsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     def paginate(
         self,
         *,
         FlowDefinitionArn: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHumanLoopsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py`

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
     "DeleteHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopRequestRequestTypeDef",
     "HumanLoopOutputTypeDef",
     "ResponseMetadataTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "HumanLoopInputTypeDef",
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-a2i-runtime
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/
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
 
 <a id="types-aiobotocore-sagemaker-a2i-runtime"></a>
 
 # types-aiobotocore-sagemaker-a2i-runtime
 
 [![PyPI - types-aiobotocore-sagemaker-a2i-runtime](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-a2i-runtime)](https://pepy.tech/project/types-aiobotocore-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AugmentedAIRuntime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[aiobotocore.AugmentedAIRuntime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.9.0/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-a2i-runtime-2.9.1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

