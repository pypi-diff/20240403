# Comparing `tmp/types-aiobotocore-pinpoint-sms-voice-2.9.0.tar.gz` & `tmp/types-aiobotocore-pinpoint-sms-voice-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pinpoint-sms-voice-2.9.0.tar", last modified: Wed Dec 13 20:00:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-pinpoint-sms-voice-2.9.1.tar", last modified: Thu Jan 18 01:21:30 2024, max compression
```

## Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0.tar` & `types-aiobotocore-pinpoint-sms-voice-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:09.737317 types-aiobotocore-pinpoint-sms-voice-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2023-12-13 20:00:09.733317 types-aiobotocore-pinpoint-sms-voice-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:09.737317 types-aiobotocore-pinpoint-sms-voice-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:09.733317 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:09.733317 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:30.049118 types-aiobotocore-pinpoint-sms-voice-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-01-18 01:21:30.049118 types-aiobotocore-pinpoint-sms-voice-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:30.049118 types-aiobotocore-pinpoint-sms-voice-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:30.045118 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:30.045118 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/LICENSE` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/PKG-INFO` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-sms-voice
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/
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
 
 <a id="types-aiobotocore-pinpoint-sms-voice"></a>
 
 # types-aiobotocore-pinpoint-sms-voice
 
 [![PyPI - types-aiobotocore-pinpoint-sms-voice](https://img.shields.io/pypi/v/types-aiobotocore-pinpoint-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-sms-voice)](https://pepy.tech/project/types-aiobotocore-pinpoint-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointSMSVoice 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice)
+[aiobotocore.PinpointSMSVoice 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice)
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
 [types-aiobotocore-pinpoint-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/README.md` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-sms-voice)](https://pepy.tech/project/types-aiobotocore-pinpoint-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointSMSVoice 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice)
+[aiobotocore.PinpointSMSVoice 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice)
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
 [types-aiobotocore-pinpoint-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/setup.py` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pinpoint-sms-voice",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_pinpoint_sms_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PinpointSMSVoice 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PinpointSMSVoice 2.9.1 service generated with"
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
     keywords="aiobotocore pinpoint-sms-voice type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_pinpoint_sms_voice": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/__init__.py` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import PinpointSMSVoiceClient
 
 Client = PinpointSMSVoiceClient
 
-
 __all__ = ("Client", "PinpointSMSVoiceClient")
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/__init__.pyi` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/__main__.py` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PinpointSMSVoice 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PinpointSMSVoice 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice\nOther"
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

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/client.py` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         """
 
     async def create_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestination: EventDestinationDefinitionTypeDef = ...,
-        EventDestinationName: str = ...
+        EventDestinationName: str = ...,
     ) -> Dict[str, Any]:
         """
         Create a new event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/client/#create_configuration_set_event_destination)
         """
@@ -151,29 +151,29 @@
     async def send_voice_message(
         self,
         *,
         CallerId: str = ...,
         ConfigurationSetName: str = ...,
         Content: VoiceMessageContentTypeDef = ...,
         DestinationPhoneNumber: str = ...,
-        OriginationPhoneNumber: str = ...
+        OriginationPhoneNumber: str = ...,
     ) -> SendVoiceMessageResponseTypeDef:
         """
         Create a new voice message and send it to a recipient's phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.send_voice_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/client/#send_voice_message)
         """
 
     async def update_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef = ...
+        EventDestination: EventDestinationDefinitionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Update an event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/client/#update_configuration_set_event_destination)
         """
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/client.pyi` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         """
 
     async def create_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestination: EventDestinationDefinitionTypeDef = ...,
-        EventDestinationName: str = ...
+        EventDestinationName: str = ...,
     ) -> Dict[str, Any]:
         """
         Create a new event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/client/#create_configuration_set_event_destination)
         """
@@ -148,29 +148,29 @@
     async def send_voice_message(
         self,
         *,
         CallerId: str = ...,
         ConfigurationSetName: str = ...,
         Content: VoiceMessageContentTypeDef = ...,
         DestinationPhoneNumber: str = ...,
-        OriginationPhoneNumber: str = ...
+        OriginationPhoneNumber: str = ...,
     ) -> SendVoiceMessageResponseTypeDef:
         """
         Create a new voice message and send it to a recipient's phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.send_voice_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/client/#send_voice_message)
         """
 
     async def update_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef = ...
+        EventDestination: EventDestinationDefinitionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Update an event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/client/#update_configuration_set_event_destination)
         """
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/literals.py` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EventTypeType", "PinpointSMSVoiceServiceName", "ServiceName", "ResourceServiceName")
 
-
 EventTypeType = Literal[
     "ANSWERED", "BUSY", "COMPLETED_CALL", "FAILED", "INITIATED_CALL", "NO_ANSWER", "RINGING"
 ]
 PinpointSMSVoiceServiceName = Literal["pinpoint-sms-voice"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/literals.pyi` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/type_defs.py` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CallInstructionsMessageTypeTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "KinesisFirehoseDestinationTypeDef",
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice/type_defs.pyi` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/PKG-INFO` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-sms-voice
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/
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
 
 <a id="types-aiobotocore-pinpoint-sms-voice"></a>
 
 # types-aiobotocore-pinpoint-sms-voice
 
 [![PyPI - types-aiobotocore-pinpoint-sms-voice](https://img.shields.io/pypi/v/types-aiobotocore-pinpoint-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-sms-voice)](https://pepy.tech/project/types-aiobotocore-pinpoint-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointSMSVoice 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice)
+[aiobotocore.PinpointSMSVoice 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice)
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
 [types-aiobotocore-pinpoint-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-2.9.0/types_aiobotocore_pinpoint_sms_voice.egg-info/SOURCES.txt` & `types-aiobotocore-pinpoint-sms-voice-2.9.1/types_aiobotocore_pinpoint_sms_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

