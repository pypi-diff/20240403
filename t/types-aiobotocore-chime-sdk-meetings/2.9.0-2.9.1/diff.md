# Comparing `tmp/types-aiobotocore-chime-sdk-meetings-2.9.0.tar.gz` & `tmp/types-aiobotocore-chime-sdk-meetings-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-meetings-2.9.0.tar", last modified: Wed Dec 13 19:58:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-meetings-2.9.1.tar", last modified: Thu Jan 18 01:20:12 2024, max compression
```

## Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0.tar` & `types-aiobotocore-chime-sdk-meetings-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.838002 types-aiobotocore-chime-sdk-meetings-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2023-12-13 19:58:45.838002 types-aiobotocore-chime-sdk-meetings-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:45.838002 types-aiobotocore-chime-sdk-meetings-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.838002 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15529 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10247 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10245 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13114 2023-12-13 19:42:03.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13113 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:02.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.838002 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.913477 types-aiobotocore-chime-sdk-meetings-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-01-18 01:20:12.913477 types-aiobotocore-chime-sdk-meetings-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:12.913477 types-aiobotocore-chime-sdk-meetings-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.913477 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15536 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15533 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13113 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13113 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:00.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.913477 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/LICENSE` & `types-aiobotocore-chime-sdk-meetings-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/PKG-INFO` & `types-aiobotocore-chime-sdk-meetings-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-meetings
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/
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
 
 <a id="types-aiobotocore-chime-sdk-meetings"></a>
 
 # types-aiobotocore-chime-sdk-meetings
 
 [![PyPI - types-aiobotocore-chime-sdk-meetings](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-meetings)](https://pepy.tech/project/types-aiobotocore-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMeetings 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[aiobotocore.ChimeSDKMeetings 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [types-aiobotocore-chime-sdk-meetings docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/README.md` & `types-aiobotocore-chime-sdk-meetings-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-meetings)](https://pepy.tech/project/types-aiobotocore-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMeetings 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[aiobotocore.ChimeSDKMeetings 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [types-aiobotocore-chime-sdk-meetings docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/setup.py` & `types-aiobotocore-chime-sdk-meetings-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-meetings",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_chime_sdk_meetings"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ChimeSDKMeetings 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ChimeSDKMeetings 2.9.1 service generated with"
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
     keywords="aiobotocore chime-sdk-meetings type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime_sdk_meetings": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/__init__.py` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import ChimeSDKMeetingsClient
 
 Client = ChimeSDKMeetingsClient
 
-
 __all__ = ("ChimeSDKMeetingsClient", "Client")
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/__init__.pyi` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/client.py` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         """
 
     async def batch_update_attendee_capabilities_except(
         self,
         *,
         MeetingId: str,
         ExcludedAttendeeIds: Sequence[AttendeeIdItemTypeDef],
-        Capabilities: AttendeeCapabilitiesTypeDef
+        Capabilities: AttendeeCapabilitiesTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates `AttendeeCapabilities` except the capabilities listed in an
         `ExcludedAttendeeIds`
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.batch_update_attendee_capabilities_except)
@@ -127,15 +127,15 @@
         """
 
     async def create_attendee(
         self,
         *,
         MeetingId: str,
         ExternalUserId: str,
-        Capabilities: AttendeeCapabilitiesTypeDef = ...
+        Capabilities: AttendeeCapabilitiesTypeDef = ...,
     ) -> CreateAttendeeResponseTypeDef:
         """
         Creates a new attendee for an active Amazon Chime SDK meeting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_attendee)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/client/#create_attendee)
         """
@@ -147,15 +147,15 @@
         MediaRegion: str,
         ExternalMeetingId: str,
         MeetingHostId: str = ...,
         NotificationsConfiguration: NotificationsConfigurationTypeDef = ...,
         MeetingFeatures: MeetingFeaturesConfigurationTypeDef = ...,
         PrimaryMeetingId: str = ...,
         TenantIds: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMeetingResponseTypeDef:
         """
         Creates a new Amazon Chime SDK meeting in the specified media Region with no
         initial
         attendees.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_meeting)
@@ -170,15 +170,15 @@
         ExternalMeetingId: str,
         Attendees: Sequence[CreateAttendeeRequestItemTypeDef],
         MeetingHostId: str = ...,
         MeetingFeatures: MeetingFeaturesConfigurationTypeDef = ...,
         NotificationsConfiguration: NotificationsConfigurationTypeDef = ...,
         PrimaryMeetingId: str = ...,
         TenantIds: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMeetingWithAttendeesResponseTypeDef:
         """
         Creates a new Amazon Chime SDK meeting in the specified media Region, with
         attendees.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_meeting_with_attendees)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/client/#create_meeting_with_attendees)
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/client.pyi` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         """
 
     async def batch_update_attendee_capabilities_except(
         self,
         *,
         MeetingId: str,
         ExcludedAttendeeIds: Sequence[AttendeeIdItemTypeDef],
-        Capabilities: AttendeeCapabilitiesTypeDef
+        Capabilities: AttendeeCapabilitiesTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates `AttendeeCapabilities` except the capabilities listed in an
         `ExcludedAttendeeIds`
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.batch_update_attendee_capabilities_except)
@@ -124,15 +124,15 @@
         """
 
     async def create_attendee(
         self,
         *,
         MeetingId: str,
         ExternalUserId: str,
-        Capabilities: AttendeeCapabilitiesTypeDef = ...
+        Capabilities: AttendeeCapabilitiesTypeDef = ...,
     ) -> CreateAttendeeResponseTypeDef:
         """
         Creates a new attendee for an active Amazon Chime SDK meeting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_attendee)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/client/#create_attendee)
         """
@@ -144,15 +144,15 @@
         MediaRegion: str,
         ExternalMeetingId: str,
         MeetingHostId: str = ...,
         NotificationsConfiguration: NotificationsConfigurationTypeDef = ...,
         MeetingFeatures: MeetingFeaturesConfigurationTypeDef = ...,
         PrimaryMeetingId: str = ...,
         TenantIds: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMeetingResponseTypeDef:
         """
         Creates a new Amazon Chime SDK meeting in the specified media Region with no
         initial
         attendees.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_meeting)
@@ -167,15 +167,15 @@
         ExternalMeetingId: str,
         Attendees: Sequence[CreateAttendeeRequestItemTypeDef],
         MeetingHostId: str = ...,
         MeetingFeatures: MeetingFeaturesConfigurationTypeDef = ...,
         NotificationsConfiguration: NotificationsConfigurationTypeDef = ...,
         PrimaryMeetingId: str = ...,
         TenantIds: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMeetingWithAttendeesResponseTypeDef:
         """
         Creates a new Amazon Chime SDK meeting in the specified media Region, with
         attendees.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_meeting_with_attendees)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/client/#create_meeting_with_attendees)
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/literals.py` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/literals.py`

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
     "MediaCapabilitiesType",
     "MeetingFeatureStatusType",
     "TranscribeContentIdentificationTypeType",
     "TranscribeContentRedactionTypeType",
     "TranscribeLanguageCodeType",
     "TranscribeMedicalContentIdentificationTypeType",
@@ -36,15 +35,14 @@
     "TranscribeVocabularyFilterMethodType",
     "ChimeSDKMeetingsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 MediaCapabilitiesType = Literal["None", "Receive", "Send", "SendReceive"]
 MeetingFeatureStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
 TranscribeContentIdentificationTypeType = Literal["PII"]
 TranscribeContentRedactionTypeType = Literal["PII"]
 TranscribeLanguageCodeType = Literal[
     "de-DE",
     "en-AU",
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/literals.pyi` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/type_defs.py` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
     "ResponseMetadataTypeDef",
     "NotificationsConfigurationTypeDef",
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings/type_defs.pyi` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-meetings
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/
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
 
 <a id="types-aiobotocore-chime-sdk-meetings"></a>
 
 # types-aiobotocore-chime-sdk-meetings
 
 [![PyPI - types-aiobotocore-chime-sdk-meetings](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-meetings)](https://pepy.tech/project/types-aiobotocore-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMeetings 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[aiobotocore.ChimeSDKMeetings 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [types-aiobotocore-chime-sdk-meetings docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.9.0/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-meetings-2.9.1/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

