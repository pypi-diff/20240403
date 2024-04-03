# Comparing `tmp/types-aiobotocore-medialive-2.9.0.tar.gz` & `tmp/types-aiobotocore-medialive-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-medialive-2.9.0.tar", last modified: Wed Dec 13 19:59:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-medialive-2.9.1.tar", last modified: Thu Jan 18 01:21:15 2024, max compression
```

## Comparing `types-aiobotocore-medialive-2.9.0.tar` & `types-aiobotocore-medialive-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.081463 types-aiobotocore-medialive-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16255 2023-12-13 19:59:53.081463 types-aiobotocore-medialive-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14684 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:53.081463 types-aiobotocore-medialive-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.081463 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56904 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    56900 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40803 2023-12-13 19:50:09.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    40801 2023-12-13 19:50:09.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   152647 2023-12-13 19:50:13.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   152646 2023-12-13 19:50:10.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11084 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11073 2023-12-13 19:50:08.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.081463 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16255 2023-12-13 19:59:53.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-13 19:59:53.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:53.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:53.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:53.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:53.000000 types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.005187 types-aiobotocore-medialive-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-01-18 01:21:15.005187 types-aiobotocore-medialive-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:15.005187 types-aiobotocore-medialive-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.005187 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56921 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56918 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40801 2024-01-18 01:11:52.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40801 2024-01-18 01:11:52.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12686 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   152646 2024-01-18 01:11:57.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152646 2024-01-18 01:11:56.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11084 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-01-18 01:11:51.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.005187 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-01-18 01:21:14.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-18 01:21:14.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:14.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:14.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:14.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:14.000000 types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-medialive-2.9.0/LICENSE` & `types-aiobotocore-medialive-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-medialive-2.9.0/PKG-INFO` & `types-aiobotocore-medialive-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-medialive
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaLive 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaLive 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/
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
 
 <a id="types-aiobotocore-medialive"></a>
 
 # types-aiobotocore-medialive
 
 [![PyPI - types-aiobotocore-medialive](https://img.shields.io/pypi/v/types-aiobotocore-medialive.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medialive.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medialive)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medialive)](https://pepy.tech/project/types-aiobotocore-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaLive 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[aiobotocore.MediaLive 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [types-aiobotocore-medialive docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-medialive-2.9.0/README.md` & `types-aiobotocore-medialive-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medialive.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medialive)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medialive)](https://pepy.tech/project/types-aiobotocore-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaLive 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[aiobotocore.MediaLive 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [types-aiobotocore-medialive docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-medialive-2.9.0/setup.py` & `types-aiobotocore-medialive-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-medialive",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaLive 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.MediaLive 2.9.1 service generated with mypy-boto3-builder"
+        " 7.23.1"
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
     keywords="aiobotocore medialive type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_medialive": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/__init__.py` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     MultiplexDeletedWaiter,
     MultiplexRunningWaiter,
     MultiplexStoppedWaiter,
 )
 
 Client = MediaLiveClient
 
-
 __all__ = (
     "ChannelCreatedWaiter",
     "ChannelDeletedWaiter",
     "ChannelRunningWaiter",
     "ChannelStoppedWaiter",
     "Client",
     "DescribeSchedulePaginator",
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/__init__.pyi` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/__main__.py` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaLive 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MediaLive 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
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

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/client.py` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaLiveClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -180,15 +179,15 @@
 
     async def batch_delete(
         self,
         *,
         ChannelIds: Sequence[str] = ...,
         InputIds: Sequence[str] = ...,
         InputSecurityGroupIds: Sequence[str] = ...,
-        MultiplexIds: Sequence[str] = ...
+        MultiplexIds: Sequence[str] = ...,
     ) -> BatchDeleteResponseTypeDef:
         """
         Starts delete of resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#batch_delete)
         """
@@ -216,15 +215,15 @@
         """
 
     async def batch_update_schedule(
         self,
         *,
         ChannelId: str,
         Creates: BatchScheduleActionCreateRequestTypeDef = ...,
-        Deletes: BatchScheduleActionDeleteRequestTypeDef = ...
+        Deletes: BatchScheduleActionDeleteRequestTypeDef = ...,
     ) -> BatchUpdateScheduleResponseTypeDef:
         """
         Update a channel schedule See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/BatchUpdateSchedule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_update_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#batch_update_schedule)
@@ -276,15 +275,15 @@
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
         Tags: Mapping[str, str] = ...,
-        Vpc: VpcOutputSettingsTypeDef = ...
+        Vpc: VpcOutputSettingsTypeDef = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a new channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_channel)
@@ -299,29 +298,29 @@
         MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,
         Name: str = ...,
         RequestId: str = ...,
         RoleArn: str = ...,
         Sources: Sequence[InputSourceRequestTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Type: InputTypeType = ...,
-        Vpc: InputVpcRequestTypeDef = ...
+        Vpc: InputVpcRequestTypeDef = ...,
     ) -> CreateInputResponseTypeDef:
         """
         Create an input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_input)
         """
 
     async def create_input_security_group(
         self,
         *,
         Tags: Mapping[str, str] = ...,
-        WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...
+        WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...,
     ) -> CreateInputSecurityGroupResponseTypeDef:
         """
         Creates a Input Security Group See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateInputSecurityGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_input_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_input_security_group)
@@ -330,30 +329,30 @@
     async def create_multiplex(
         self,
         *,
         AvailabilityZones: Sequence[str],
         MultiplexSettings: MultiplexSettingsTypeDef,
         Name: str,
         RequestId: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateMultiplexResponseTypeDef:
         """
         Create a new multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_multiplex)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_multiplex)
         """
 
     async def create_multiplex_program(
         self,
         *,
         MultiplexId: str,
         MultiplexProgramSettings: MultiplexProgramSettingsTypeDef,
         ProgramName: str,
-        RequestId: str
+        RequestId: str,
     ) -> CreateMultiplexProgramResponseTypeDef:
         """
         Create a new program in the multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_multiplex_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_multiplex_program)
         """
@@ -665,15 +664,15 @@
         MaxResults: int = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         NextToken: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
-        VideoQuality: str = ...
+        VideoQuality: str = ...,
     ) -> ListOfferingsResponseTypeDef:
         """
         List offerings available for purchase.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#list_offerings)
         """
@@ -686,15 +685,15 @@
         MaxResults: int = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         NextToken: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
-        VideoQuality: str = ...
+        VideoQuality: str = ...,
     ) -> ListReservationsResponseTypeDef:
         """
         List purchased reservations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_reservations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#list_reservations)
         """
@@ -715,15 +714,15 @@
         *,
         Count: int,
         OfferingId: str,
         Name: str = ...,
         RenewalSettings: RenewalSettingsTypeDef = ...,
         RequestId: str = ...,
         Start: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> PurchaseOfferingResponseTypeDef:
         """
         Purchase an offering and create a reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.purchase_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#purchase_offering)
         """
@@ -806,15 +805,15 @@
 
     async def transfer_input_device(
         self,
         *,
         InputDeviceId: str,
         TargetCustomerId: str = ...,
         TargetRegion: str = ...,
-        TransferMessage: str = ...
+        TransferMessage: str = ...,
     ) -> Dict[str, Any]:
         """
         Start an input device transfer to another AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.transfer_input_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#transfer_input_device)
         """
@@ -838,29 +837,29 @@
         Destinations: Sequence[OutputDestinationTypeDef] = ...,
         EncoderSettings: EncoderSettingsTypeDef = ...,
         InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_channel)
         """
 
     async def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...
+        Destinations: Sequence[OutputDestinationTypeDef] = ...,
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_channel_class)
         """
@@ -871,15 +870,15 @@
         InputId: str,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceRequestTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
         MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,
         Name: str = ...,
         RoleArn: str = ...,
-        Sources: Sequence[InputSourceRequestTypeDef] = ...
+        Sources: Sequence[InputSourceRequestTypeDef] = ...,
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_input)
         """
@@ -887,57 +886,57 @@
     async def update_input_device(
         self,
         *,
         InputDeviceId: str,
         HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
         Name: str = ...,
         UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
-        AvailabilityZone: str = ...
+        AvailabilityZone: str = ...,
     ) -> UpdateInputDeviceResponseTypeDef:
         """
         Updates the parameters for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_input_device)
         """
 
     async def update_input_security_group(
         self,
         *,
         InputSecurityGroupId: str,
         Tags: Mapping[str, str] = ...,
-        WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...
+        WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...,
     ) -> UpdateInputSecurityGroupResponseTypeDef:
         """
         Update an Input Security Group's Whilelists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_input_security_group)
         """
 
     async def update_multiplex(
         self,
         *,
         MultiplexId: str,
         MultiplexSettings: MultiplexSettingsTypeDef = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateMultiplexResponseTypeDef:
         """
         Updates a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_multiplex)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_multiplex)
         """
 
     async def update_multiplex_program(
         self,
         *,
         MultiplexId: str,
         ProgramName: str,
-        MultiplexProgramSettings: MultiplexProgramSettingsTypeDef = ...
+        MultiplexProgramSettings: MultiplexProgramSettingsTypeDef = ...,
     ) -> UpdateMultiplexProgramResponseTypeDef:
         """
         Update a program in a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_multiplex_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_multiplex_program)
         """
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/client.pyi` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     async def batch_delete(
         self,
         *,
         ChannelIds: Sequence[str] = ...,
         InputIds: Sequence[str] = ...,
         InputSecurityGroupIds: Sequence[str] = ...,
-        MultiplexIds: Sequence[str] = ...
+        MultiplexIds: Sequence[str] = ...,
     ) -> BatchDeleteResponseTypeDef:
         """
         Starts delete of resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#batch_delete)
         """
@@ -212,15 +212,15 @@
         """
 
     async def batch_update_schedule(
         self,
         *,
         ChannelId: str,
         Creates: BatchScheduleActionCreateRequestTypeDef = ...,
-        Deletes: BatchScheduleActionDeleteRequestTypeDef = ...
+        Deletes: BatchScheduleActionDeleteRequestTypeDef = ...,
     ) -> BatchUpdateScheduleResponseTypeDef:
         """
         Update a channel schedule See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/BatchUpdateSchedule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_update_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#batch_update_schedule)
@@ -272,15 +272,15 @@
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
         Tags: Mapping[str, str] = ...,
-        Vpc: VpcOutputSettingsTypeDef = ...
+        Vpc: VpcOutputSettingsTypeDef = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a new channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_channel)
@@ -295,29 +295,29 @@
         MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,
         Name: str = ...,
         RequestId: str = ...,
         RoleArn: str = ...,
         Sources: Sequence[InputSourceRequestTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Type: InputTypeType = ...,
-        Vpc: InputVpcRequestTypeDef = ...
+        Vpc: InputVpcRequestTypeDef = ...,
     ) -> CreateInputResponseTypeDef:
         """
         Create an input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_input)
         """
 
     async def create_input_security_group(
         self,
         *,
         Tags: Mapping[str, str] = ...,
-        WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...
+        WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...,
     ) -> CreateInputSecurityGroupResponseTypeDef:
         """
         Creates a Input Security Group See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateInputSecurityGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_input_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_input_security_group)
@@ -326,30 +326,30 @@
     async def create_multiplex(
         self,
         *,
         AvailabilityZones: Sequence[str],
         MultiplexSettings: MultiplexSettingsTypeDef,
         Name: str,
         RequestId: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateMultiplexResponseTypeDef:
         """
         Create a new multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_multiplex)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_multiplex)
         """
 
     async def create_multiplex_program(
         self,
         *,
         MultiplexId: str,
         MultiplexProgramSettings: MultiplexProgramSettingsTypeDef,
         ProgramName: str,
-        RequestId: str
+        RequestId: str,
     ) -> CreateMultiplexProgramResponseTypeDef:
         """
         Create a new program in the multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_multiplex_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#create_multiplex_program)
         """
@@ -661,15 +661,15 @@
         MaxResults: int = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         NextToken: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
-        VideoQuality: str = ...
+        VideoQuality: str = ...,
     ) -> ListOfferingsResponseTypeDef:
         """
         List offerings available for purchase.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#list_offerings)
         """
@@ -682,15 +682,15 @@
         MaxResults: int = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         NextToken: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
-        VideoQuality: str = ...
+        VideoQuality: str = ...,
     ) -> ListReservationsResponseTypeDef:
         """
         List purchased reservations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_reservations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#list_reservations)
         """
@@ -711,15 +711,15 @@
         *,
         Count: int,
         OfferingId: str,
         Name: str = ...,
         RenewalSettings: RenewalSettingsTypeDef = ...,
         RequestId: str = ...,
         Start: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> PurchaseOfferingResponseTypeDef:
         """
         Purchase an offering and create a reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.purchase_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#purchase_offering)
         """
@@ -802,15 +802,15 @@
 
     async def transfer_input_device(
         self,
         *,
         InputDeviceId: str,
         TargetCustomerId: str = ...,
         TargetRegion: str = ...,
-        TransferMessage: str = ...
+        TransferMessage: str = ...,
     ) -> Dict[str, Any]:
         """
         Start an input device transfer to another AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.transfer_input_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#transfer_input_device)
         """
@@ -834,29 +834,29 @@
         Destinations: Sequence[OutputDestinationTypeDef] = ...,
         EncoderSettings: EncoderSettingsTypeDef = ...,
         InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_channel)
         """
 
     async def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...
+        Destinations: Sequence[OutputDestinationTypeDef] = ...,
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_channel_class)
         """
@@ -867,15 +867,15 @@
         InputId: str,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceRequestTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
         MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,
         Name: str = ...,
         RoleArn: str = ...,
-        Sources: Sequence[InputSourceRequestTypeDef] = ...
+        Sources: Sequence[InputSourceRequestTypeDef] = ...,
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_input)
         """
@@ -883,57 +883,57 @@
     async def update_input_device(
         self,
         *,
         InputDeviceId: str,
         HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
         Name: str = ...,
         UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
-        AvailabilityZone: str = ...
+        AvailabilityZone: str = ...,
     ) -> UpdateInputDeviceResponseTypeDef:
         """
         Updates the parameters for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_input_device)
         """
 
     async def update_input_security_group(
         self,
         *,
         InputSecurityGroupId: str,
         Tags: Mapping[str, str] = ...,
-        WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...
+        WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...,
     ) -> UpdateInputSecurityGroupResponseTypeDef:
         """
         Update an Input Security Group's Whilelists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_input_security_group)
         """
 
     async def update_multiplex(
         self,
         *,
         MultiplexId: str,
         MultiplexSettings: MultiplexSettingsTypeDef = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateMultiplexResponseTypeDef:
         """
         Updates a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_multiplex)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_multiplex)
         """
 
     async def update_multiplex_program(
         self,
         *,
         MultiplexId: str,
         ProgramName: str,
-        MultiplexProgramSettings: MultiplexProgramSettingsTypeDef = ...
+        MultiplexProgramSettings: MultiplexProgramSettingsTypeDef = ...,
     ) -> UpdateMultiplexProgramResponseTypeDef:
         """
         Update a program in a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_multiplex_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_multiplex_program)
         """
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/literals.py` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/literals.py`

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
     "AacCodingModeType",
     "AacInputTypeType",
     "AacProfileType",
     "AacRateControlModeType",
     "AacRawFormatType",
     "AacSpecType",
@@ -320,15 +319,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AacCodingModeType = Literal[
     "AD_RECEIVER_MIX", "CODING_MODE_1_0", "CODING_MODE_1_1", "CODING_MODE_2_0", "CODING_MODE_5_1"
 ]
 AacInputTypeType = Literal["BROADCASTER_MIXED_AD", "NORMAL"]
 AacProfileType = Literal["HEV1", "HEV2", "LC"]
 AacRateControlModeType = Literal["CBR", "VBR"]
 AacRawFormatType = Literal["LATM_LOAS", "NONE"]
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/literals.pyi` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/paginator.py` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     "ListInputsPaginator",
     "ListMultiplexProgramsPaginator",
     "ListMultiplexesPaginator",
     "ListOfferingsPaginator",
     "ListReservationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -217,15 +216,15 @@
         Duration: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/paginators/#listofferingspaginator)
         """
 
 
@@ -242,13 +241,13 @@
         Codec: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/paginators/#listreservationspaginator)
         """
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/paginator.pyi` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         Duration: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/paginators/#listofferingspaginator)
         """
 
 class ListReservationsPaginator(AioPaginator):
@@ -230,13 +230,13 @@
         Codec: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/paginators/#listreservationspaginator)
         """
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/type_defs.py` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AacSettingsTypeDef",
     "Ac3SettingsTypeDef",
     "AcceptInputDeviceTransferRequestRequestTypeDef",
     "AccountConfigurationTypeDef",
     "AncillarySourceSettingsTypeDef",
     "ArchiveS3SettingsTypeDef",
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/type_defs.pyi` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/waiter.py` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive/waiter.pyi` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/PKG-INFO` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-medialive
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaLive 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaLive 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/
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
 
 <a id="types-aiobotocore-medialive"></a>
 
 # types-aiobotocore-medialive
 
 [![PyPI - types-aiobotocore-medialive](https://img.shields.io/pypi/v/types-aiobotocore-medialive.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medialive.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medialive)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medialive)](https://pepy.tech/project/types-aiobotocore-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaLive 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[aiobotocore.MediaLive 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [types-aiobotocore-medialive docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-medialive-2.9.0/types_aiobotocore_medialive.egg-info/SOURCES.txt` & `types-aiobotocore-medialive-2.9.1/types_aiobotocore_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

