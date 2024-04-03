# Comparing `tmp/types-aiobotocore-personalize-events-2.9.0.tar.gz` & `tmp/types-aiobotocore-personalize-events-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-personalize-events-2.9.0.tar", last modified: Wed Dec 13 20:00:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-personalize-events-2.9.1.tar", last modified: Thu Jan 18 01:21:28 2024, max compression
```

## Comparing `types-aiobotocore-personalize-events-2.9.0.tar` & `types-aiobotocore-personalize-events-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.473337 types-aiobotocore-personalize-events-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2023-12-13 20:00:07.473337 types-aiobotocore-personalize-events-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:07.473337 types-aiobotocore-personalize-events-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.473337 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2023-12-13 19:51:34.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2023-12-13 19:51:34.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2023-12-13 19:51:34.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.473337 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:28.009127 types-aiobotocore-personalize-events-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-01-18 01:21:28.009127 types-aiobotocore-personalize-events-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:28.009127 types-aiobotocore-personalize-events-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:28.009127 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-01-18 01:13:12.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-01-18 01:13:12.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:28.009127 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-01-18 01:21:27.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-18 01:21:27.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:27.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:27.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:27.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 01:21:27.000000 types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/LICENSE` & `types-aiobotocore-personalize-events-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-personalize-events-2.9.0/PKG-INFO` & `types-aiobotocore-personalize-events-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-personalize-events
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PersonalizeEvents 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PersonalizeEvents 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/
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
 
 <a id="types-aiobotocore-personalize-events"></a>
 
 # types-aiobotocore-personalize-events
 
 [![PyPI - types-aiobotocore-personalize-events](https://img.shields.io/pypi/v/types-aiobotocore-personalize-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize-events)](https://pepy.tech/project/types-aiobotocore-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PersonalizeEvents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[aiobotocore.PersonalizeEvents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [types-aiobotocore-personalize-events docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/README.md` & `types-aiobotocore-personalize-events-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize-events)](https://pepy.tech/project/types-aiobotocore-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PersonalizeEvents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[aiobotocore.PersonalizeEvents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [types-aiobotocore-personalize-events docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/setup.py` & `types-aiobotocore-personalize-events-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-personalize-events",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_personalize_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PersonalizeEvents 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PersonalizeEvents 2.9.1 service generated with"
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
     keywords="aiobotocore personalize-events type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_personalize_events": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/__init__.py` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import PersonalizeEventsClient
 
 Client = PersonalizeEventsClient
 
-
 __all__ = ("Client", "PersonalizeEventsClient")
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/__init__.pyi` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/__main__.py` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PersonalizeEvents 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PersonalizeEvents 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents\nOther"
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

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/client.py` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     async def put_events(
         self,
         *,
         trackingId: str,
         sessionId: str,
         eventList: Sequence[EventTypeDef],
-        userId: str = ...
+        userId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Records item interaction event data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.put_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/client/#put_events)
         """
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/client.pyi` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     async def put_events(
         self,
         *,
         trackingId: str,
         sessionId: str,
         eventList: Sequence[EventTypeDef],
-        userId: str = ...
+        userId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Records item interaction event data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.put_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/client/#put_events)
         """
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/literals.py` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PersonalizeEventsServiceName", "ServiceName", "ResourceServiceName")
 
-
 PersonalizeEventsServiceName = Literal["personalize-events"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/literals.pyi` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/type_defs.py` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TimestampTypeDef",
     "ActionTypeDef",
     "ResponseMetadataTypeDef",
     "MetricAttributionTypeDef",
     "ItemTypeDef",
     "UserTypeDef",
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events/type_defs.pyi` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/PKG-INFO` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-personalize-events
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PersonalizeEvents 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PersonalizeEvents 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/
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
 
 <a id="types-aiobotocore-personalize-events"></a>
 
 # types-aiobotocore-personalize-events
 
 [![PyPI - types-aiobotocore-personalize-events](https://img.shields.io/pypi/v/types-aiobotocore-personalize-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize-events)](https://pepy.tech/project/types-aiobotocore-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PersonalizeEvents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[aiobotocore.PersonalizeEvents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [types-aiobotocore-personalize-events docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-personalize-events-2.9.0/types_aiobotocore_personalize_events.egg-info/SOURCES.txt` & `types-aiobotocore-personalize-events-2.9.1/types_aiobotocore_personalize_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

