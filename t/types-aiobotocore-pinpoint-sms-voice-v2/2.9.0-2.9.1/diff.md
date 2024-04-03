# Comparing `tmp/types-aiobotocore-pinpoint-sms-voice-v2-2.9.0.tar.gz` & `tmp/types-aiobotocore-pinpoint-sms-voice-v2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pinpoint-sms-voice-v2-2.9.0.tar", last modified: Wed Dec 13 20:00:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-pinpoint-sms-voice-v2-2.9.1.tar", last modified: Thu Jan 18 01:21:30 2024, max compression
```

## Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0.tar` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:10.109314 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17406 2023-12-13 20:00:10.109314 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15790 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:10.109314 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:10.109314 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67390 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    67386 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18085 2023-12-13 19:51:50.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18083 2023-12-13 19:51:50.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29139 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29117 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    73579 2023-12-13 19:51:51.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    73578 2023-12-13 19:51:50.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:49.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:10.109314 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17406 2023-12-13 20:00:10.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-13 20:00:10.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:10.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:10.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:10.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-13 20:00:10.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:30.381116 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-01-18 01:21:30.381116 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15790 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:30.381116 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:30.377116 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67419 2024-01-18 01:13:26.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67416 2024-01-18 01:13:26.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-01-18 01:13:26.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-01-18 01:13:26.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29155 2024-01-18 01:13:26.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29134 2024-01-18 01:13:26.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    73578 2024-01-18 01:13:27.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73578 2024-01-18 01:13:27.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:25.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:30.381116 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-18 01:21:30.000000 types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/LICENSE` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/PKG-INFO` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-sms-voice-v2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PinpointSMSVoiceV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PinpointSMSVoiceV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/
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
 
 <a id="types-aiobotocore-pinpoint-sms-voice-v2"></a>
 
 # types-aiobotocore-pinpoint-sms-voice-v2
 
 [![PyPI - types-aiobotocore-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/types-aiobotocore-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-sms-voice-v2)](https://pepy.tech/project/types-aiobotocore-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointSMSVoiceV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[aiobotocore.PinpointSMSVoiceV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [types-aiobotocore-pinpoint-sms-voice-v2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/README.md` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-sms-voice-v2)](https://pepy.tech/project/types-aiobotocore-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointSMSVoiceV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[aiobotocore.PinpointSMSVoiceV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [types-aiobotocore-pinpoint-sms-voice-v2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/setup.py` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pinpoint-sms-voice-v2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_pinpoint_sms_voice_v2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PinpointSMSVoiceV2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PinpointSMSVoiceV2 2.9.1 service generated with"
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
         "aiobotocore pinpoint-sms-voice-v2 type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_pinpoint_sms_voice_v2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/__init__.py` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     DescribeVerifiedDestinationNumbersPaginator,
     ListPoolOriginationIdentitiesPaginator,
     ListRegistrationAssociationsPaginator,
 )
 
 Client = PinpointSMSVoiceV2Client
 
-
 __all__ = (
     "Client",
     "DescribeAccountAttributesPaginator",
     "DescribeAccountLimitsPaginator",
     "DescribeConfigurationSetsPaginator",
     "DescribeKeywordsPaginator",
     "DescribeOptOutListsPaginator",
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/__init__.pyi` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/__main__.py` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PinpointSMSVoiceV2 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PinpointSMSVoiceV2 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2\nOther"
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

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/client.py` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PinpointSMSVoiceV2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -230,15 +229,15 @@
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         MatchingEventTypes: Sequence[EventTypeType],
         CloudWatchLogsDestination: CloudWatchLogsDestinationTypeDef = ...,
         KinesisFirehoseDestination: KinesisFirehoseDestinationTypeDef = ...,
         SnsDestination: SnsDestinationTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateEventDestinationResultTypeDef:
         """
         Creates a new event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#create_event_destination)
         """
@@ -257,15 +256,15 @@
         self,
         *,
         OriginationIdentity: str,
         IsoCountryCode: str,
         MessageType: MessageTypeType,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreatePoolResultTypeDef:
         """
         Creates a new pool and associates the specified origination identity to the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#create_pool)
@@ -295,15 +294,15 @@
 
     async def create_registration_attachment(
         self,
         *,
         AttachmentBody: BlobTypeDef = ...,
         AttachmentUrl: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateRegistrationAttachmentResultTypeDef:
         """
         Create a new registration attachment to use for uploading a file or a URL to a
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_registration_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#create_registration_attachment)
@@ -320,15 +319,15 @@
         """
 
     async def create_verified_destination_number(
         self,
         *,
         DestinationPhoneNumber: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateVerifiedDestinationNumberResultTypeDef:
         """
         You can only send messages to verified destination numbers when your account is
         in the
         sandbox.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_verified_destination_number)
@@ -496,15 +495,15 @@
 
     async def describe_configuration_sets(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeConfigurationSetsResultTypeDef:
         """
         Describes the specified configuration sets or all in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_configuration_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_configuration_sets)
         """
@@ -512,15 +511,15 @@
     async def describe_keywords(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeKeywordsResultTypeDef:
         """
         Describes the specified keywords or all keywords on your origination phone
         number or
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_keywords)
@@ -540,15 +539,15 @@
     async def describe_opted_out_numbers(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeOptedOutNumbersResultTypeDef:
         """
         Describes the specified opted out destination numbers or all opted out
         destination numbers in an opt-out
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_opted_out_numbers)
@@ -557,15 +556,15 @@
 
     async def describe_phone_numbers(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribePhoneNumbersResultTypeDef:
         """
         Describes the specified origination phone number, or all the phone numbers in
         your
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_phone_numbers)
@@ -574,15 +573,15 @@
 
     async def describe_pools(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribePoolsResultTypeDef:
         """
         Retrieves the specified pools or all pools associated with your Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_pools)
@@ -591,15 +590,15 @@
 
     async def describe_registration_attachments(
         self,
         *,
         RegistrationAttachmentIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationAttachmentsResultTypeDef:
         """
         Retrieves the specified registration attachments or all registration
         attachments associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_attachments)
@@ -609,15 +608,15 @@
     async def describe_registration_field_definitions(
         self,
         *,
         RegistrationType: str,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationFieldDefinitionsResultTypeDef:
         """
         Retrieves the specified registration type field definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_field_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_field_definitions)
         """
@@ -626,45 +625,45 @@
         self,
         *,
         RegistrationId: str,
         VersionNumber: int = ...,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationFieldValuesResultTypeDef:
         """
         Retrieves the specified registration field values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_field_values)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_field_values)
         """
 
     async def describe_registration_section_definitions(
         self,
         *,
         RegistrationType: str,
         SectionPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationSectionDefinitionsResultTypeDef:
         """
         Retrieves the specified registration section definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_section_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_section_definitions)
         """
 
     async def describe_registration_type_definitions(
         self,
         *,
         RegistrationTypes: Sequence[str] = ...,
         Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationTypeDefinitionsResultTypeDef:
         """
         Retrieves the specified registration type definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_type_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_type_definitions)
         """
@@ -672,45 +671,45 @@
     async def describe_registration_versions(
         self,
         *,
         RegistrationId: str,
         VersionNumbers: Sequence[int] = ...,
         Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationVersionsResultTypeDef:
         """
         Retrieves the specified registration version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_versions)
         """
 
     async def describe_registrations(
         self,
         *,
         RegistrationIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationsResultTypeDef:
         """
         Retrieves the specified registrations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registrations)
         """
 
     async def describe_sender_ids(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeSenderIdsResultTypeDef:
         """
         Describes the specified SenderIds or all SenderIds associated with your Amazon
         Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_sender_ids)
@@ -732,15 +731,15 @@
     async def describe_verified_destination_numbers(
         self,
         *,
         VerifiedDestinationNumberIds: Sequence[str] = ...,
         DestinationPhoneNumbers: Sequence[str] = ...,
         Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeVerifiedDestinationNumbersResultTypeDef:
         """
         Retrieves the specified verified destiona numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_verified_destination_numbers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_verified_destination_numbers)
         """
@@ -781,30 +780,30 @@
 
     async def list_pool_origination_identities(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPoolOriginationIdentitiesResultTypeDef:
         """
         Lists all associated origination identities in your pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.list_pool_origination_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#list_pool_origination_identities)
         """
 
     async def list_registration_associations(
         self,
         *,
         RegistrationId: str,
         Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRegistrationAssociationsResultTypeDef:
         """
         Retreive all of the origination identies that are associated with a
         registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.list_registration_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#list_registration_associations)
@@ -820,15 +819,15 @@
 
     async def put_keyword(
         self,
         *,
         OriginationIdentity: str,
         Keyword: str,
         KeywordMessage: str,
-        KeywordAction: KeywordActionType = ...
+        KeywordAction: KeywordActionType = ...,
     ) -> PutKeywordResultTypeDef:
         """
         Creates or updates a keyword configuration on an origination phone number or
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.put_keyword)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#put_keyword)
@@ -847,15 +846,15 @@
     async def put_registration_field_value(
         self,
         *,
         RegistrationId: str,
         FieldPath: str,
         SelectChoices: Sequence[str] = ...,
         TextValue: str = ...,
-        RegistrationAttachmentId: str = ...
+        RegistrationAttachmentId: str = ...,
     ) -> PutRegistrationFieldValueResultTypeDef:
         """
         Creates or updates a field value for a registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.put_registration_field_value)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#put_registration_field_value)
         """
@@ -886,15 +885,15 @@
         NumberCapabilities: Sequence[NumberCapabilityType],
         NumberType: RequestableNumberTypeType,
         OptOutListName: str = ...,
         PoolId: str = ...,
         RegistrationId: str = ...,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RequestPhoneNumberResultTypeDef:
         """
         Request an origination phone number for use in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.request_phone_number)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#request_phone_number)
         """
@@ -903,15 +902,15 @@
         self,
         *,
         SenderId: str,
         IsoCountryCode: str,
         MessageTypes: Sequence[MessageTypeType] = ...,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RequestSenderIdResultTypeDef:
         """
         Request a new sender ID that doesn't require registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.request_sender_id)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#request_sender_id)
         """
@@ -921,15 +920,15 @@
         *,
         VerifiedDestinationNumberId: str,
         VerificationChannel: VerificationChannelType,
         LanguageCode: LanguageCodeType = ...,
         OriginationIdentity: str = ...,
         ConfigurationSetName: str = ...,
         Context: Mapping[str, str] = ...,
-        DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...
+        DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...,
     ) -> SendDestinationNumberVerificationCodeResultTypeDef:
         """
         Before you can send test messages to a verified destination phone number you
         need to opt-in the verified destination phone
         number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_destination_number_verification_code)
@@ -945,15 +944,15 @@
         MessageType: MessageTypeType = ...,
         Keyword: str = ...,
         ConfigurationSetName: str = ...,
         MaxPrice: str = ...,
         TimeToLive: int = ...,
         Context: Mapping[str, str] = ...,
         DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> SendTextMessageResultTypeDef:
         """
         Creates a new text message and sends it to a recipient's phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_text_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#send_text_message)
         """
@@ -966,15 +965,15 @@
         MessageBody: str = ...,
         MessageBodyTextType: VoiceMessageBodyTextTypeType = ...,
         VoiceId: VoiceIdType = ...,
         ConfigurationSetName: str = ...,
         MaxPricePerMinute: str = ...,
         TimeToLive: int = ...,
         Context: Mapping[str, str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> SendVoiceMessageResultTypeDef:
         """
         Allows you to send a request that sends a voice message through Amazon Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_voice_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#send_voice_message)
         """
@@ -1054,15 +1053,15 @@
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         Enabled: bool = ...,
         MatchingEventTypes: Sequence[EventTypeType] = ...,
         CloudWatchLogsDestination: CloudWatchLogsDestinationTypeDef = ...,
         KinesisFirehoseDestination: KinesisFirehoseDestinationTypeDef = ...,
-        SnsDestination: SnsDestinationTypeDef = ...
+        SnsDestination: SnsDestinationTypeDef = ...,
     ) -> UpdateEventDestinationResultTypeDef:
         """
         Updates an existing event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#update_event_destination)
         """
@@ -1072,15 +1071,15 @@
         *,
         PhoneNumberId: str,
         TwoWayEnabled: bool = ...,
         TwoWayChannelArn: str = ...,
         TwoWayChannelRole: str = ...,
         SelfManagedOptOutsEnabled: bool = ...,
         OptOutListName: str = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdatePhoneNumberResultTypeDef:
         """
         Updates the configuration of an existing origination phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_phone_number)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#update_phone_number)
         """
@@ -1091,15 +1090,15 @@
         PoolId: str,
         TwoWayEnabled: bool = ...,
         TwoWayChannelArn: str = ...,
         TwoWayChannelRole: str = ...,
         SelfManagedOptOutsEnabled: bool = ...,
         OptOutListName: str = ...,
         SharedRoutesEnabled: bool = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdatePoolResultTypeDef:
         """
         Updates the configuration of an existing pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#update_pool)
         """
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/client.pyi` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         MatchingEventTypes: Sequence[EventTypeType],
         CloudWatchLogsDestination: CloudWatchLogsDestinationTypeDef = ...,
         KinesisFirehoseDestination: KinesisFirehoseDestinationTypeDef = ...,
         SnsDestination: SnsDestinationTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateEventDestinationResultTypeDef:
         """
         Creates a new event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#create_event_destination)
         """
@@ -253,15 +253,15 @@
         self,
         *,
         OriginationIdentity: str,
         IsoCountryCode: str,
         MessageType: MessageTypeType,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreatePoolResultTypeDef:
         """
         Creates a new pool and associates the specified origination identity to the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#create_pool)
@@ -291,15 +291,15 @@
 
     async def create_registration_attachment(
         self,
         *,
         AttachmentBody: BlobTypeDef = ...,
         AttachmentUrl: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateRegistrationAttachmentResultTypeDef:
         """
         Create a new registration attachment to use for uploading a file or a URL to a
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_registration_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#create_registration_attachment)
@@ -316,15 +316,15 @@
         """
 
     async def create_verified_destination_number(
         self,
         *,
         DestinationPhoneNumber: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateVerifiedDestinationNumberResultTypeDef:
         """
         You can only send messages to verified destination numbers when your account is
         in the
         sandbox.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_verified_destination_number)
@@ -492,15 +492,15 @@
 
     async def describe_configuration_sets(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeConfigurationSetsResultTypeDef:
         """
         Describes the specified configuration sets or all in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_configuration_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_configuration_sets)
         """
@@ -508,15 +508,15 @@
     async def describe_keywords(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeKeywordsResultTypeDef:
         """
         Describes the specified keywords or all keywords on your origination phone
         number or
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_keywords)
@@ -536,15 +536,15 @@
     async def describe_opted_out_numbers(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeOptedOutNumbersResultTypeDef:
         """
         Describes the specified opted out destination numbers or all opted out
         destination numbers in an opt-out
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_opted_out_numbers)
@@ -553,15 +553,15 @@
 
     async def describe_phone_numbers(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribePhoneNumbersResultTypeDef:
         """
         Describes the specified origination phone number, or all the phone numbers in
         your
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_phone_numbers)
@@ -570,15 +570,15 @@
 
     async def describe_pools(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribePoolsResultTypeDef:
         """
         Retrieves the specified pools or all pools associated with your Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_pools)
@@ -587,15 +587,15 @@
 
     async def describe_registration_attachments(
         self,
         *,
         RegistrationAttachmentIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationAttachmentsResultTypeDef:
         """
         Retrieves the specified registration attachments or all registration
         attachments associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_attachments)
@@ -605,15 +605,15 @@
     async def describe_registration_field_definitions(
         self,
         *,
         RegistrationType: str,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationFieldDefinitionsResultTypeDef:
         """
         Retrieves the specified registration type field definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_field_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_field_definitions)
         """
@@ -622,45 +622,45 @@
         self,
         *,
         RegistrationId: str,
         VersionNumber: int = ...,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationFieldValuesResultTypeDef:
         """
         Retrieves the specified registration field values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_field_values)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_field_values)
         """
 
     async def describe_registration_section_definitions(
         self,
         *,
         RegistrationType: str,
         SectionPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationSectionDefinitionsResultTypeDef:
         """
         Retrieves the specified registration section definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_section_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_section_definitions)
         """
 
     async def describe_registration_type_definitions(
         self,
         *,
         RegistrationTypes: Sequence[str] = ...,
         Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationTypeDefinitionsResultTypeDef:
         """
         Retrieves the specified registration type definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_type_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_type_definitions)
         """
@@ -668,45 +668,45 @@
     async def describe_registration_versions(
         self,
         *,
         RegistrationId: str,
         VersionNumbers: Sequence[int] = ...,
         Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationVersionsResultTypeDef:
         """
         Retrieves the specified registration version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registration_versions)
         """
 
     async def describe_registrations(
         self,
         *,
         RegistrationIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationsResultTypeDef:
         """
         Retrieves the specified registrations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_registrations)
         """
 
     async def describe_sender_ids(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeSenderIdsResultTypeDef:
         """
         Describes the specified SenderIds or all SenderIds associated with your Amazon
         Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_sender_ids)
@@ -728,15 +728,15 @@
     async def describe_verified_destination_numbers(
         self,
         *,
         VerifiedDestinationNumberIds: Sequence[str] = ...,
         DestinationPhoneNumbers: Sequence[str] = ...,
         Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeVerifiedDestinationNumbersResultTypeDef:
         """
         Retrieves the specified verified destiona numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_verified_destination_numbers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#describe_verified_destination_numbers)
         """
@@ -777,30 +777,30 @@
 
     async def list_pool_origination_identities(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPoolOriginationIdentitiesResultTypeDef:
         """
         Lists all associated origination identities in your pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.list_pool_origination_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#list_pool_origination_identities)
         """
 
     async def list_registration_associations(
         self,
         *,
         RegistrationId: str,
         Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRegistrationAssociationsResultTypeDef:
         """
         Retreive all of the origination identies that are associated with a
         registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.list_registration_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#list_registration_associations)
@@ -816,15 +816,15 @@
 
     async def put_keyword(
         self,
         *,
         OriginationIdentity: str,
         Keyword: str,
         KeywordMessage: str,
-        KeywordAction: KeywordActionType = ...
+        KeywordAction: KeywordActionType = ...,
     ) -> PutKeywordResultTypeDef:
         """
         Creates or updates a keyword configuration on an origination phone number or
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.put_keyword)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#put_keyword)
@@ -843,15 +843,15 @@
     async def put_registration_field_value(
         self,
         *,
         RegistrationId: str,
         FieldPath: str,
         SelectChoices: Sequence[str] = ...,
         TextValue: str = ...,
-        RegistrationAttachmentId: str = ...
+        RegistrationAttachmentId: str = ...,
     ) -> PutRegistrationFieldValueResultTypeDef:
         """
         Creates or updates a field value for a registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.put_registration_field_value)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#put_registration_field_value)
         """
@@ -882,15 +882,15 @@
         NumberCapabilities: Sequence[NumberCapabilityType],
         NumberType: RequestableNumberTypeType,
         OptOutListName: str = ...,
         PoolId: str = ...,
         RegistrationId: str = ...,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RequestPhoneNumberResultTypeDef:
         """
         Request an origination phone number for use in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.request_phone_number)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#request_phone_number)
         """
@@ -899,15 +899,15 @@
         self,
         *,
         SenderId: str,
         IsoCountryCode: str,
         MessageTypes: Sequence[MessageTypeType] = ...,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RequestSenderIdResultTypeDef:
         """
         Request a new sender ID that doesn't require registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.request_sender_id)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#request_sender_id)
         """
@@ -917,15 +917,15 @@
         *,
         VerifiedDestinationNumberId: str,
         VerificationChannel: VerificationChannelType,
         LanguageCode: LanguageCodeType = ...,
         OriginationIdentity: str = ...,
         ConfigurationSetName: str = ...,
         Context: Mapping[str, str] = ...,
-        DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...
+        DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...,
     ) -> SendDestinationNumberVerificationCodeResultTypeDef:
         """
         Before you can send test messages to a verified destination phone number you
         need to opt-in the verified destination phone
         number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_destination_number_verification_code)
@@ -941,15 +941,15 @@
         MessageType: MessageTypeType = ...,
         Keyword: str = ...,
         ConfigurationSetName: str = ...,
         MaxPrice: str = ...,
         TimeToLive: int = ...,
         Context: Mapping[str, str] = ...,
         DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> SendTextMessageResultTypeDef:
         """
         Creates a new text message and sends it to a recipient's phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_text_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#send_text_message)
         """
@@ -962,15 +962,15 @@
         MessageBody: str = ...,
         MessageBodyTextType: VoiceMessageBodyTextTypeType = ...,
         VoiceId: VoiceIdType = ...,
         ConfigurationSetName: str = ...,
         MaxPricePerMinute: str = ...,
         TimeToLive: int = ...,
         Context: Mapping[str, str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> SendVoiceMessageResultTypeDef:
         """
         Allows you to send a request that sends a voice message through Amazon Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_voice_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#send_voice_message)
         """
@@ -1050,15 +1050,15 @@
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         Enabled: bool = ...,
         MatchingEventTypes: Sequence[EventTypeType] = ...,
         CloudWatchLogsDestination: CloudWatchLogsDestinationTypeDef = ...,
         KinesisFirehoseDestination: KinesisFirehoseDestinationTypeDef = ...,
-        SnsDestination: SnsDestinationTypeDef = ...
+        SnsDestination: SnsDestinationTypeDef = ...,
     ) -> UpdateEventDestinationResultTypeDef:
         """
         Updates an existing event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#update_event_destination)
         """
@@ -1068,15 +1068,15 @@
         *,
         PhoneNumberId: str,
         TwoWayEnabled: bool = ...,
         TwoWayChannelArn: str = ...,
         TwoWayChannelRole: str = ...,
         SelfManagedOptOutsEnabled: bool = ...,
         OptOutListName: str = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdatePhoneNumberResultTypeDef:
         """
         Updates the configuration of an existing origination phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_phone_number)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#update_phone_number)
         """
@@ -1087,15 +1087,15 @@
         PoolId: str,
         TwoWayEnabled: bool = ...,
         TwoWayChannelArn: str = ...,
         TwoWayChannelRole: str = ...,
         SelfManagedOptOutsEnabled: bool = ...,
         OptOutListName: str = ...,
         SharedRoutesEnabled: bool = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdatePoolResultTypeDef:
         """
         Updates the configuration of an existing pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/client/#update_pool)
         """
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/literals.py` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/literals.py`

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
     "AccountAttributeNameType",
     "AccountLimitNameType",
     "AttachmentStatusType",
     "AttachmentUploadErrorReasonType",
     "ConfigurationSetFilterNameType",
     "DescribeAccountAttributesPaginatorName",
@@ -82,15 +81,14 @@
     "PinpointSMSVoiceV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountAttributeNameType = Literal["ACCOUNT_TIER"]
 AccountLimitNameType = Literal[
     "CONFIGURATION_SETS",
     "OPT_OUT_LISTS",
     "PHONE_NUMBERS",
     "POOLS",
     "REGISTRATIONS",
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/literals.pyi` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/paginator.py` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -121,390 +121,368 @@
     "DescribeSenderIdsPaginator",
     "DescribeSpendLimitsPaginator",
     "DescribeVerifiedDestinationNumbersPaginator",
     "ListPoolOriginationIdentitiesPaginator",
     "ListRegistrationAssociationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeAccountAttributesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountAttributesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
         """
 
-
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
         """
 
-
 class DescribeConfigurationSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigurationSetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
         """
 
-
 class DescribeKeywordsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
     """
 
     def paginate(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeKeywordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
         """
 
-
 class DescribeOptOutListsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOptOutListsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
         """
 
-
 class DescribeOptedOutNumbersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOptedOutNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
         """
 
-
 class DescribePhoneNumbersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
     """
 
     def paginate(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
         """
 
-
 class DescribePoolsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
     """
 
     def paginate(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
         """
 
-
 class DescribeRegistrationAttachmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationattachmentspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationAttachmentIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationattachmentspaginator)
         """
 
-
 class DescribeRegistrationFieldDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationfielddefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationType: str,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationFieldDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationfielddefinitionspaginator)
         """
 
-
 class DescribeRegistrationFieldValuesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldValues)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationfieldvaluespaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         VersionNumber: int = ...,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationFieldValuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationfieldvaluespaginator)
         """
 
-
 class DescribeRegistrationSectionDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationSectionDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationsectiondefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationType: str,
         SectionPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationSectionDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationSectionDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationsectiondefinitionspaginator)
         """
 
-
 class DescribeRegistrationTypeDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationTypeDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationtypedefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationTypes: Sequence[str] = ...,
         Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationTypeDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationTypeDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationtypedefinitionspaginator)
         """
 
-
 class DescribeRegistrationVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationversionspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         VersionNumbers: Sequence[int] = ...,
         Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationversionspaginator)
         """
 
-
 class DescribeRegistrationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationspaginator)
         """
 
-
 class DescribeSenderIdsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
     """
 
     def paginate(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSenderIdsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
         """
 
-
 class DescribeSpendLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSpendLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
         """
 
-
 class DescribeVerifiedDestinationNumbersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeVerifiedDestinationNumbers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeverifieddestinationnumberspaginator)
     """
 
     def paginate(
         self,
         *,
         VerifiedDestinationNumberIds: Sequence[str] = ...,
         DestinationPhoneNumbers: Sequence[str] = ...,
         Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeVerifiedDestinationNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeVerifiedDestinationNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeverifieddestinationnumberspaginator)
         """
 
-
 class ListPoolOriginationIdentitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
     """
 
     def paginate(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPoolOriginationIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
         """
 
-
 class ListRegistrationAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListRegistrationAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#listregistrationassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRegistrationAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListRegistrationAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#listregistrationassociationspaginator)
         """
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/paginator.pyi` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/paginator.py`

 * *Files 9% similar despite different names*

```diff
@@ -123,366 +123,387 @@
     "DescribeVerifiedDestinationNumbersPaginator",
     "ListPoolOriginationIdentitiesPaginator",
     "ListRegistrationAssociationsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeAccountAttributesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountAttributesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
         """
 
+
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
         """
 
+
 class DescribeConfigurationSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigurationSetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
         """
 
+
 class DescribeKeywordsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
     """
 
     def paginate(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeKeywordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
         """
 
+
 class DescribeOptOutListsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOptOutListsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
         """
 
+
 class DescribeOptedOutNumbersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOptedOutNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
         """
 
+
 class DescribePhoneNumbersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
     """
 
     def paginate(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
         """
 
+
 class DescribePoolsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
     """
 
     def paginate(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
         """
 
+
 class DescribeRegistrationAttachmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationattachmentspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationAttachmentIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationattachmentspaginator)
         """
 
+
 class DescribeRegistrationFieldDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationfielddefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationType: str,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationFieldDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationfielddefinitionspaginator)
         """
 
+
 class DescribeRegistrationFieldValuesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldValues)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationfieldvaluespaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         VersionNumber: int = ...,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationFieldValuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationfieldvaluespaginator)
         """
 
+
 class DescribeRegistrationSectionDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationSectionDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationsectiondefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationType: str,
         SectionPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationSectionDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationSectionDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationsectiondefinitionspaginator)
         """
 
+
 class DescribeRegistrationTypeDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationTypeDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationtypedefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationTypes: Sequence[str] = ...,
         Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationTypeDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationTypeDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationtypedefinitionspaginator)
         """
 
+
 class DescribeRegistrationVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationversionspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         VersionNumbers: Sequence[int] = ...,
         Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationversionspaginator)
         """
 
+
 class DescribeRegistrationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegistrationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeregistrationspaginator)
         """
 
+
 class DescribeSenderIdsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
     """
 
     def paginate(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSenderIdsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
         """
 
+
 class DescribeSpendLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSpendLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
         """
 
+
 class DescribeVerifiedDestinationNumbersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeVerifiedDestinationNumbers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeverifieddestinationnumberspaginator)
     """
 
     def paginate(
         self,
         *,
         VerifiedDestinationNumberIds: Sequence[str] = ...,
         DestinationPhoneNumbers: Sequence[str] = ...,
         Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeVerifiedDestinationNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeVerifiedDestinationNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#describeverifieddestinationnumberspaginator)
         """
 
+
 class ListPoolOriginationIdentitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
     """
 
     def paginate(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPoolOriginationIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
         """
 
+
 class ListRegistrationAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListRegistrationAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#listregistrationassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRegistrationAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListRegistrationAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/paginators/#listregistrationassociationspaginator)
         """
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/type_defs.py` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BlobTypeDef",
     "CloudWatchLogsDestinationTypeDef",
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2/type_defs.pyi` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/PKG-INFO` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-sms-voice-v2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PinpointSMSVoiceV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PinpointSMSVoiceV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/
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
 
 <a id="types-aiobotocore-pinpoint-sms-voice-v2"></a>
 
 # types-aiobotocore-pinpoint-sms-voice-v2
 
 [![PyPI - types-aiobotocore-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/types-aiobotocore-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-sms-voice-v2)](https://pepy.tech/project/types-aiobotocore-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointSMSVoiceV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[aiobotocore.PinpointSMSVoiceV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [types-aiobotocore-pinpoint-sms-voice-v2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-sms-voice-v2-2.9.0/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/SOURCES.txt` & `types-aiobotocore-pinpoint-sms-voice-v2-2.9.1/types_aiobotocore_pinpoint_sms_voice_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

