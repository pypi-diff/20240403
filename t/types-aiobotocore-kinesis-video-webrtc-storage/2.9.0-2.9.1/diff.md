# Comparing `tmp/types-aiobotocore-kinesis-video-webrtc-storage-2.9.0.tar.gz` & `tmp/types-aiobotocore-kinesis-video-webrtc-storage-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-webrtc-storage-2.9.0.tar", last modified: Wed Dec 13 19:59:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-webrtc-storage-2.9.1.tar", last modified: Thu Jan 18 01:21:03 2024, max compression
```

## Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0.tar` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:40.725566 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2023-12-13 19:59:40.725566 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11726 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:40.725566 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:40.725566 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8607 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8605 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:34.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:40.725566 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2023-12-13 19:59:40.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-13 19:59:40.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:40.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:40.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:40.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-13 19:59:40.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:03.525238 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-01-18 01:21:03.525238 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:03.525238 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:03.521238 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8605 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8605 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:23.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:03.525238 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-01-18 01:21:03.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-01-18 01:21:03.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:03.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:03.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:03.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-18 01:21:03.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/LICENSE` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/PKG-INFO` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-webrtc-storage
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/
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
 
 <a id="types-aiobotocore-kinesis-video-webrtc-storage"></a>
 
 # types-aiobotocore-kinesis-video-webrtc-storage
 
 [![PyPI - types-aiobotocore-kinesis-video-webrtc-storage](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoWebRTCStorage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[aiobotocore.KinesisVideoWebRTCStorage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/README.md` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoWebRTCStorage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[aiobotocore.KinesisVideoWebRTCStorage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/setup.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,51 +7,50 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-webrtc-storage",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kinesis_video_webrtc_storage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.9.1 service generated with"
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
         "aiobotocore kinesis-video-webrtc-storage type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesis_video_webrtc_storage": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import KinesisVideoWebRTCStorageClient
 
 Client = KinesisVideoWebRTCStorageClient
 
-
 __all__ = ("Client", "KinesisVideoWebRTCStorageClient")
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage\nOther"
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

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/client.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/literals.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,21 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "KinesisVideoWebRTCStorageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 KinesisVideoWebRTCStorageServiceName = Literal["kinesis-video-webrtc-storage"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from typing import Dict
 
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "JoinStorageSessionInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-webrtc-storage
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/
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
 
 <a id="types-aiobotocore-kinesis-video-webrtc-storage"></a>
 
 # types-aiobotocore-kinesis-video-webrtc-storage
 
 [![PyPI - types-aiobotocore-kinesis-video-webrtc-storage](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoWebRTCStorage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[aiobotocore.KinesisVideoWebRTCStorage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.9.0/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-webrtc-storage-2.9.1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*
