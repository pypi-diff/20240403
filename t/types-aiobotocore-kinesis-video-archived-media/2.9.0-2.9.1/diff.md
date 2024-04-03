# Comparing `tmp/types-aiobotocore-kinesis-video-archived-media-2.9.0.tar.gz` & `tmp/types-aiobotocore-kinesis-video-archived-media-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-archived-media-2.9.0.tar", last modified: Wed Dec 13 19:59:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-archived-media-2.9.1.tar", last modified: Thu Jan 18 01:21:02 2024, max compression
```

## Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0.tar` & `types-aiobotocore-kinesis-video-archived-media-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:39.625575 types-aiobotocore-kinesis-video-archived-media-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14273 2023-12-13 19:59:39.625575 types-aiobotocore-kinesis-video-archived-media-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:39.625575 types-aiobotocore-kinesis-video-archived-media-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:39.625575 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:33.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:39.625575 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14273 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:02.513243 types-aiobotocore-kinesis-video-archived-media-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-01-18 01:21:02.509243 types-aiobotocore-kinesis-video-archived-media-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:02.513243 types-aiobotocore-kinesis-video-archived-media-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:02.509243 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-01-18 01:10:22.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-01-18 01:10:22.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-01-18 01:10:22.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-01-18 01:10:22.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:02.509243 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/LICENSE` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/PKG-INFO` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-archived-media
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/
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
 
 <a id="types-aiobotocore-kinesis-video-archived-media"></a>
 
 # types-aiobotocore-kinesis-video-archived-media
 
 [![PyPI - types-aiobotocore-kinesis-video-archived-media](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-archived-media)](https://pepy.tech/project/types-aiobotocore-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoArchivedMedia 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[aiobotocore.KinesisVideoArchivedMedia 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/README.md` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-archived-media)](https://pepy.tech/project/types-aiobotocore-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoArchivedMedia 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[aiobotocore.KinesisVideoArchivedMedia 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/setup.py` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,51 +7,50 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-archived-media",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kinesis_video_archived_media"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.9.1 service generated with"
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
         "aiobotocore kinesis-video-archived-media type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesis_video_archived_media": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/__init__.py` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,13 @@
 """
 
 from .client import KinesisVideoArchivedMediaClient
 from .paginator import GetImagesPaginator, ListFragmentsPaginator
 
 Client = KinesisVideoArchivedMediaClient
 
-
 __all__ = (
     "Client",
     "GetImagesPaginator",
     "KinesisVideoArchivedMediaClient",
     "ListFragmentsPaginator",
 )
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/__init__.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/__main__.py` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia\nOther"
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

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/client.py` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KinesisVideoArchivedMediaClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -125,15 +124,15 @@
         """
 
     async def get_clip(
         self,
         *,
         ClipFragmentSelector: ClipFragmentSelectorTypeDef,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> GetClipOutputTypeDef:
         """
         Downloads an MP4 file (clip) containing the archived, on-demand media from the
         specified video stream over the specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_clip)
@@ -146,15 +145,15 @@
         StreamName: str = ...,
         StreamARN: str = ...,
         PlaybackMode: DASHPlaybackModeType = ...,
         DisplayFragmentTimestamp: DASHDisplayFragmentTimestampType = ...,
         DisplayFragmentNumber: DASHDisplayFragmentNumberType = ...,
         DASHFragmentSelector: DASHFragmentSelectorTypeDef = ...,
         Expires: int = ...,
-        MaxManifestFragmentResults: int = ...
+        MaxManifestFragmentResults: int = ...,
     ) -> GetDASHStreamingSessionURLOutputTypeDef:
         """
         Retrieves an MPEG Dynamic Adaptive Streaming over HTTP (DASH) URL for the
         stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_dash_streaming_session_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/client/#get_dash_streaming_session_url)
@@ -167,15 +166,15 @@
         StreamARN: str = ...,
         PlaybackMode: HLSPlaybackModeType = ...,
         HLSFragmentSelector: HLSFragmentSelectorTypeDef = ...,
         ContainerFormat: ContainerFormatType = ...,
         DiscontinuityMode: HLSDiscontinuityModeType = ...,
         DisplayFragmentTimestamp: HLSDisplayFragmentTimestampType = ...,
         Expires: int = ...,
-        MaxMediaPlaylistFragmentResults: int = ...
+        MaxMediaPlaylistFragmentResults: int = ...,
     ) -> GetHLSStreamingSessionURLOutputTypeDef:
         """
         Retrieves an HTTP Live Streaming (HLS) URL for the stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_hls_streaming_session_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/client/#get_hls_streaming_session_url)
         """
@@ -190,15 +189,15 @@
         StreamName: str = ...,
         StreamARN: str = ...,
         SamplingInterval: int = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetImagesOutputTypeDef:
         """
         Retrieves a list of Images corresponding to each timestamp for a given time
         range, sampling interval, and image format
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_images)
@@ -220,15 +219,15 @@
     async def list_fragments(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        FragmentSelector: FragmentSelectorTypeDef = ...
+        FragmentSelector: FragmentSelectorTypeDef = ...,
     ) -> ListFragmentsOutputTypeDef:
         """
         Returns a list of  Fragment objects from the specified stream and timestamp
         range within the archived
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.list_fragments)
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/client.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         """
 
     async def get_clip(
         self,
         *,
         ClipFragmentSelector: ClipFragmentSelectorTypeDef,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> GetClipOutputTypeDef:
         """
         Downloads an MP4 file (clip) containing the archived, on-demand media from the
         specified video stream over the specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_clip)
@@ -142,15 +142,15 @@
         StreamName: str = ...,
         StreamARN: str = ...,
         PlaybackMode: DASHPlaybackModeType = ...,
         DisplayFragmentTimestamp: DASHDisplayFragmentTimestampType = ...,
         DisplayFragmentNumber: DASHDisplayFragmentNumberType = ...,
         DASHFragmentSelector: DASHFragmentSelectorTypeDef = ...,
         Expires: int = ...,
-        MaxManifestFragmentResults: int = ...
+        MaxManifestFragmentResults: int = ...,
     ) -> GetDASHStreamingSessionURLOutputTypeDef:
         """
         Retrieves an MPEG Dynamic Adaptive Streaming over HTTP (DASH) URL for the
         stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_dash_streaming_session_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/client/#get_dash_streaming_session_url)
@@ -163,15 +163,15 @@
         StreamARN: str = ...,
         PlaybackMode: HLSPlaybackModeType = ...,
         HLSFragmentSelector: HLSFragmentSelectorTypeDef = ...,
         ContainerFormat: ContainerFormatType = ...,
         DiscontinuityMode: HLSDiscontinuityModeType = ...,
         DisplayFragmentTimestamp: HLSDisplayFragmentTimestampType = ...,
         Expires: int = ...,
-        MaxMediaPlaylistFragmentResults: int = ...
+        MaxMediaPlaylistFragmentResults: int = ...,
     ) -> GetHLSStreamingSessionURLOutputTypeDef:
         """
         Retrieves an HTTP Live Streaming (HLS) URL for the stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_hls_streaming_session_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/client/#get_hls_streaming_session_url)
         """
@@ -186,15 +186,15 @@
         StreamName: str = ...,
         StreamARN: str = ...,
         SamplingInterval: int = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetImagesOutputTypeDef:
         """
         Retrieves a list of Images corresponding to each timestamp for a given time
         range, sampling interval, and image format
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_images)
@@ -216,15 +216,15 @@
     async def list_fragments(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        FragmentSelector: FragmentSelectorTypeDef = ...
+        FragmentSelector: FragmentSelectorTypeDef = ...,
     ) -> ListFragmentsOutputTypeDef:
         """
         Returns a list of  Fragment objects from the specified stream and timestamp
         range within the archived
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.list_fragments)
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/literals.py` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/literals.py`

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
     "ClipFragmentSelectorTypeType",
     "ContainerFormatType",
     "DASHDisplayFragmentNumberType",
     "DASHDisplayFragmentTimestampType",
     "DASHFragmentSelectorTypeType",
     "DASHPlaybackModeType",
@@ -41,15 +40,14 @@
     "KinesisVideoArchivedMediaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ClipFragmentSelectorTypeType = Literal["PRODUCER_TIMESTAMP", "SERVER_TIMESTAMP"]
 ContainerFormatType = Literal["FRAGMENTED_MP4", "MPEG_TS"]
 DASHDisplayFragmentNumberType = Literal["ALWAYS", "NEVER"]
 DASHDisplayFragmentTimestampType = Literal["ALWAYS", "NEVER"]
 DASHFragmentSelectorTypeType = Literal["PRODUCER_TIMESTAMP", "SERVER_TIMESTAMP"]
 DASHPlaybackModeType = Literal["LIVE", "LIVE_REPLAY", "ON_DEMAND"]
 FormatConfigKeyType = Literal["JPEGQuality"]
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/literals.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/paginator.py` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,18 +39,16 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GetImagesPaginator", "ListFragmentsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -72,15 +70,15 @@
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         SamplingInterval: int = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
 
@@ -92,13 +90,13 @@
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         FragmentSelector: FragmentSelectorTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFragmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#listfragmentspaginator)
         """
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/paginator.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         SamplingInterval: int = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
 class ListFragmentsPaginator(AioPaginator):
@@ -87,13 +87,13 @@
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         FragmentSelector: FragmentSelectorTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFragmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#listfragmentspaginator)
         """
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/type_defs.py` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/type_defs.py`

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
     "TimestampTypeDef",
     "FragmentTypeDef",
     "ResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ImageTypeDef",
     "GetMediaForFragmentListInputRequestTypeDef",
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-archived-media
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/
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
 
 <a id="types-aiobotocore-kinesis-video-archived-media"></a>
 
 # types-aiobotocore-kinesis-video-archived-media
 
 [![PyPI - types-aiobotocore-kinesis-video-archived-media](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-archived-media)](https://pepy.tech/project/types-aiobotocore-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoArchivedMedia 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[aiobotocore.KinesisVideoArchivedMedia 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.9.0/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-archived-media-2.9.1/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

