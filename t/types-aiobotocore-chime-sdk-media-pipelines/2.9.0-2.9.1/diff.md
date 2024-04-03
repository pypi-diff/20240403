# Comparing `tmp/types-aiobotocore-chime-sdk-media-pipelines-2.9.0.tar.gz` & `tmp/types-aiobotocore-chime-sdk-media-pipelines-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-media-pipelines-2.9.0.tar", last modified: Wed Dec 13 19:58:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-media-pipelines-2.9.1.tar", last modified: Thu Jan 18 01:20:12 2024, max compression
```

## Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0.tar` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.462004 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2023-12-13 19:58:45.462004 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:45.462004 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.462004 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28150 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28146 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    45531 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    45530 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.462004 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.577479 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-01-18 01:20:12.577479 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:12.577479 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.573479 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28160 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    45530 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45530 2024-01-18 01:03:59.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:58.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.577479 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/LICENSE` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/PKG-INFO` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-media-pipelines
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/
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
 
 <a id="types-aiobotocore-chime-sdk-media-pipelines"></a>
 
 # types-aiobotocore-chime-sdk-media-pipelines
 
 [![PyPI - types-aiobotocore-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMediaPipelines 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[aiobotocore.ChimeSDKMediaPipelines 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [types-aiobotocore-chime-sdk-media-pipelines docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/README.md` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMediaPipelines 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[aiobotocore.ChimeSDKMediaPipelines 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [types-aiobotocore-chime-sdk-media-pipelines docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/setup.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-media-pipelines",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.9.1 service generated with"
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
         "aiobotocore chime-sdk-media-pipelines type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime_sdk_media_pipelines": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/__init__.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import ChimeSDKMediaPipelinesClient
 
 Client = ChimeSDKMediaPipelinesClient
 
-
 __all__ = ("ChimeSDKMediaPipelinesClient", "Client")
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/__main__.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/client.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ChimeSDKMediaPipelinesClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -132,30 +131,30 @@
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
         ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
         """
 
     async def create_media_concatenation_pipeline(
         self,
         *,
         Sources: Sequence[ConcatenationSourceTypeDef],
         Sinks: Sequence[ConcatenationSinkTypeDef],
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaConcatenationPipelineResponseTypeDef:
         """
         Creates a media concatenation pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_concatenation_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
@@ -165,15 +164,15 @@
         *,
         MediaInsightsPipelineConfigurationArn: str,
         KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
         KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline)
         """
@@ -182,15 +181,15 @@
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
         Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
         RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
@@ -198,45 +197,45 @@
 
     async def create_media_live_connector_pipeline(
         self,
         *,
         Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_live_connector_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_live_connector_pipeline)
         """
 
     async def create_media_pipeline_kinesis_video_stream_pool(
         self,
         *,
         StreamConfiguration: KinesisVideoStreamConfigurationTypeDef,
         PoolName: str,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaPipelineKinesisVideoStreamPoolResponseTypeDef:
         """
         Creates an Kinesis video stream pool for the media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_pipeline_kinesis_video_stream_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_pipeline_kinesis_video_stream_pool)
         """
 
     async def create_media_stream_pipeline(
         self,
         *,
         Sources: Sequence[MediaStreamSourceTypeDef],
         Sinks: Sequence[MediaStreamSinkTypeDef],
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaStreamPipelineResponseTypeDef:
         """
         Creates a streaming media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_stream_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_stream_pipeline)
         """
@@ -403,30 +402,30 @@
 
     async def start_speaker_search_task(
         self,
         *,
         Identifier: str,
         VoiceProfileDomainArn: str,
         KinesisVideoStreamSourceTaskConfiguration: KinesisVideoStreamSourceTaskConfigurationTypeDef = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartSpeakerSearchTaskResponseTypeDef:
         """
         Starts a speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.start_speaker_search_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#start_speaker_search_task)
         """
 
     async def start_voice_tone_analysis_task(
         self,
         *,
         Identifier: str,
         LanguageCode: Literal["en-US"],
         KinesisVideoStreamSourceTaskConfiguration: KinesisVideoStreamSourceTaskConfigurationTypeDef = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartVoiceToneAnalysisTaskResponseTypeDef:
         """
         Starts a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.start_voice_tone_analysis_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#start_voice_tone_analysis_task)
         """
@@ -469,15 +468,15 @@
 
     async def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
         Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
@@ -492,15 +491,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_status)
         """
 
     async def update_media_pipeline_kinesis_video_stream_pool(
         self,
         *,
         Identifier: str,
-        StreamConfiguration: KinesisVideoStreamConfigurationUpdateTypeDef = ...
+        StreamConfiguration: KinesisVideoStreamConfigurationUpdateTypeDef = ...,
     ) -> UpdateMediaPipelineKinesisVideoStreamPoolResponseTypeDef:
         """
         Updates an Kinesis video stream pool in a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_pipeline_kinesis_video_stream_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_pipeline_kinesis_video_stream_pool)
         """
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/client.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -128,30 +128,30 @@
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
         ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
         """
 
     async def create_media_concatenation_pipeline(
         self,
         *,
         Sources: Sequence[ConcatenationSourceTypeDef],
         Sinks: Sequence[ConcatenationSinkTypeDef],
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaConcatenationPipelineResponseTypeDef:
         """
         Creates a media concatenation pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_concatenation_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
@@ -161,15 +161,15 @@
         *,
         MediaInsightsPipelineConfigurationArn: str,
         KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
         KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline)
         """
@@ -178,15 +178,15 @@
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
         Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
         RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
@@ -194,45 +194,45 @@
 
     async def create_media_live_connector_pipeline(
         self,
         *,
         Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_live_connector_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_live_connector_pipeline)
         """
 
     async def create_media_pipeline_kinesis_video_stream_pool(
         self,
         *,
         StreamConfiguration: KinesisVideoStreamConfigurationTypeDef,
         PoolName: str,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaPipelineKinesisVideoStreamPoolResponseTypeDef:
         """
         Creates an Kinesis video stream pool for the media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_pipeline_kinesis_video_stream_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_pipeline_kinesis_video_stream_pool)
         """
 
     async def create_media_stream_pipeline(
         self,
         *,
         Sources: Sequence[MediaStreamSourceTypeDef],
         Sinks: Sequence[MediaStreamSinkTypeDef],
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMediaStreamPipelineResponseTypeDef:
         """
         Creates a streaming media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_stream_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_stream_pipeline)
         """
@@ -399,30 +399,30 @@
 
     async def start_speaker_search_task(
         self,
         *,
         Identifier: str,
         VoiceProfileDomainArn: str,
         KinesisVideoStreamSourceTaskConfiguration: KinesisVideoStreamSourceTaskConfigurationTypeDef = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartSpeakerSearchTaskResponseTypeDef:
         """
         Starts a speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.start_speaker_search_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#start_speaker_search_task)
         """
 
     async def start_voice_tone_analysis_task(
         self,
         *,
         Identifier: str,
         LanguageCode: Literal["en-US"],
         KinesisVideoStreamSourceTaskConfiguration: KinesisVideoStreamSourceTaskConfigurationTypeDef = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartVoiceToneAnalysisTaskResponseTypeDef:
         """
         Starts a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.start_voice_tone_analysis_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#start_voice_tone_analysis_task)
         """
@@ -465,15 +465,15 @@
 
     async def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
         Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
@@ -488,15 +488,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_status)
         """
 
     async def update_media_pipeline_kinesis_video_stream_pool(
         self,
         *,
         Identifier: str,
-        StreamConfiguration: KinesisVideoStreamConfigurationUpdateTypeDef = ...
+        StreamConfiguration: KinesisVideoStreamConfigurationUpdateTypeDef = ...,
     ) -> UpdateMediaPipelineKinesisVideoStreamPoolResponseTypeDef:
         """
         Updates an Kinesis video stream pool in a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_pipeline_kinesis_video_stream_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_pipeline_kinesis_video_stream_pool)
         """
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/literals.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/literals.py`

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
     "ActiveSpeakerPositionType",
     "ArtifactsConcatenationStateType",
     "ArtifactsStateType",
     "AudioArtifactsConcatenationStateType",
     "AudioChannelsOptionType",
     "AudioMuxTypeType",
@@ -69,15 +68,14 @@
     "VoiceAnalyticsLanguageCodeType",
     "ChimeSDKMediaPipelinesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ActiveSpeakerPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 ArtifactsConcatenationStateType = Literal["Disabled", "Enabled"]
 ArtifactsStateType = Literal["Disabled", "Enabled"]
 AudioArtifactsConcatenationStateType = Literal["Enabled"]
 AudioChannelsOptionType = Literal["Mono", "Stereo"]
 AudioMuxTypeType = Literal["AudioOnly", "AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
 BorderColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveSpeakerOnlyConfigurationTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-media-pipelines
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/
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
 
 <a id="types-aiobotocore-chime-sdk-media-pipelines"></a>
 
 # types-aiobotocore-chime-sdk-media-pipelines
 
 [![PyPI - types-aiobotocore-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMediaPipelines 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[aiobotocore.ChimeSDKMediaPipelines 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [types-aiobotocore-chime-sdk-media-pipelines docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.9.0/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-media-pipelines-2.9.1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

