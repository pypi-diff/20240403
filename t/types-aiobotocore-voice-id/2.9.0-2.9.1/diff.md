# Comparing `tmp/types-aiobotocore-voice-id-2.9.0.tar.gz` & `tmp/types-aiobotocore-voice-id-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-voice-id-2.9.0.tar", last modified: Wed Dec 13 20:00:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-voice-id-2.9.1.tar", last modified: Thu Jan 18 01:22:00 2024, max compression
```

## Comparing `types-aiobotocore-voice-id-2.9.0.tar` & `types-aiobotocore-voice-id-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.737024 types-aiobotocore-voice-id-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2023-12-13 20:00:43.737024 types-aiobotocore-voice-id-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:43.737024 types-aiobotocore-voice-id-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.737024 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25022 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25018 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10626 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    27796 2023-12-13 19:57:34.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27795 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:33.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.737024 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2023-12-13 20:00:43.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 20:00:43.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:43.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:43.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:43.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:43.000000 types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.892979 types-aiobotocore-voice-id-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-01-18 01:22:00.892979 types-aiobotocore-voice-id-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:00.892979 types-aiobotocore-voice-id-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.892979 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    27795 2024-01-18 01:19:03.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27795 2024-01-18 01:19:03.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:02.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.892979 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-01-18 01:22:00.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:22:00.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:00.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:00.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:00.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:22:00.000000 types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-voice-id-2.9.0/LICENSE` & `types-aiobotocore-voice-id-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-voice-id-2.9.0/PKG-INFO` & `types-aiobotocore-voice-id-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-voice-id
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.VoiceID 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.VoiceID 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/
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
 
 <a id="types-aiobotocore-voice-id"></a>
 
 # types-aiobotocore-voice-id
 
 [![PyPI - types-aiobotocore-voice-id](https://img.shields.io/pypi/v/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VoiceID 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[aiobotocore.VoiceID 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [types-aiobotocore-voice-id docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-voice-id-2.9.0/README.md` & `types-aiobotocore-voice-id-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VoiceID 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[aiobotocore.VoiceID 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [types-aiobotocore-voice-id docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-voice-id-2.9.0/setup.py` & `types-aiobotocore-voice-id-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-voice-id",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.VoiceID 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.VoiceID 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore voice-id type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_voice_id": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/__init__.py` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListSpeakerEnrollmentJobsPaginator,
     ListSpeakersPaginator,
     ListWatchlistsPaginator,
 )
 
 Client = VoiceIDClient
 
-
 __all__ = (
     "Client",
     "ListDomainsPaginator",
     "ListFraudsterRegistrationJobsPaginator",
     "ListFraudstersPaginator",
     "ListSpeakerEnrollmentJobsPaginator",
     "ListSpeakersPaginator",
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/__init__.pyi` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/__main__.py` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VoiceID 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.VoiceID 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/client.py` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("VoiceIDClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -137,15 +136,15 @@
     async def create_domain(
         self,
         *,
         Name: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a domain that contains all Amazon Connect Voice ID data, such as
         speakers, fraudsters, customer audio, and
         voiceprints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.create_domain)
@@ -306,15 +305,15 @@
 
     async def list_fraudster_registration_jobs(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFraudsterRegistrationJobsResponseTypeDef:
         """
         Lists all the fraudster registration jobs in the domain with the given
         `JobStatus`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.list_fraudster_registration_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#list_fraudster_registration_jobs)
@@ -332,15 +331,15 @@
 
     async def list_speaker_enrollment_jobs(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListSpeakerEnrollmentJobsResponseTypeDef:
         """
         Lists all the speaker enrollment jobs in the domain with the specified
         `JobStatus`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.list_speaker_enrollment_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#list_speaker_enrollment_jobs)
@@ -391,15 +390,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: RegistrationConfigTypeDef = ...
+        RegistrationConfig: RegistrationConfigTypeDef = ...,
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_fraudster_registration_job)
         """
@@ -409,15 +408,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         EnrollmentConfig: EnrollmentConfigTypeDef = ...,
-        JobName: str = ...
+        JobName: str = ...,
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_speaker_enrollment_job)
         """
@@ -440,15 +439,15 @@
 
     async def update_domain(
         self,
         *,
         DomainId: str,
         Name: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.update_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#update_domain)
         """
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/client.pyi` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     async def create_domain(
         self,
         *,
         Name: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a domain that contains all Amazon Connect Voice ID data, such as
         speakers, fraudsters, customer audio, and
         voiceprints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.create_domain)
@@ -302,15 +302,15 @@
 
     async def list_fraudster_registration_jobs(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFraudsterRegistrationJobsResponseTypeDef:
         """
         Lists all the fraudster registration jobs in the domain with the given
         `JobStatus`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.list_fraudster_registration_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#list_fraudster_registration_jobs)
@@ -328,15 +328,15 @@
 
     async def list_speaker_enrollment_jobs(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListSpeakerEnrollmentJobsResponseTypeDef:
         """
         Lists all the speaker enrollment jobs in the domain with the specified
         `JobStatus`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.list_speaker_enrollment_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#list_speaker_enrollment_jobs)
@@ -387,15 +387,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: RegistrationConfigTypeDef = ...
+        RegistrationConfig: RegistrationConfigTypeDef = ...,
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_fraudster_registration_job)
         """
@@ -405,15 +405,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         EnrollmentConfig: EnrollmentConfigTypeDef = ...,
-        JobName: str = ...
+        JobName: str = ...,
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_speaker_enrollment_job)
         """
@@ -436,15 +436,15 @@
 
     async def update_domain(
         self,
         *,
         DomainId: str,
         Name: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.update_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#update_domain)
         """
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/literals.py` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/literals.py`

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
     "AuthenticationDecisionType",
     "DomainStatusType",
     "DuplicateRegistrationActionType",
     "ExistingEnrollmentActionType",
     "FraudDetectionActionType",
     "FraudDetectionDecisionType",
@@ -42,15 +41,14 @@
     "VoiceIDServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AuthenticationDecisionType = Literal[
     "ACCEPT",
     "NOT_ENOUGH_SPEECH",
     "REJECT",
     "SPEAKER_EXPIRED",
     "SPEAKER_ID_NOT_PROVIDED",
     "SPEAKER_NOT_ENROLLED",
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/literals.pyi` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/paginator.py` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     "ListFraudsterRegistrationJobsPaginator",
     "ListFraudstersPaginator",
     "ListSpeakerEnrollmentJobsPaginator",
     "ListSpeakersPaginator",
     "ListWatchlistsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -89,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFraudsterRegistrationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listfraudsterregistrationjobspaginator)
         """
 
 
@@ -108,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         WatchlistId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFraudstersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listfraudsterspaginator)
         """
 
 
@@ -127,15 +126,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listspeakerenrollmentjobspaginator)
         """
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/paginator.pyi` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFraudsterRegistrationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listfraudsterregistrationjobspaginator)
         """
 
 class ListFraudstersPaginator(AioPaginator):
@@ -103,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         WatchlistId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFraudstersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listfraudsterspaginator)
         """
 
 class ListSpeakerEnrollmentJobsPaginator(AioPaginator):
@@ -121,15 +121,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listspeakerenrollmentjobspaginator)
         """
 
 class ListSpeakersPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/type_defs.py` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/type_defs.py`

 * *Files 0% similar despite different names*

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
     "AssociateFraudsterRequestRequestTypeDef",
     "FraudsterTypeDef",
     "ResponseMetadataTypeDef",
     "AuthenticationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id/type_defs.pyi` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/PKG-INFO` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-voice-id
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.VoiceID 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.VoiceID 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/
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
 
 <a id="types-aiobotocore-voice-id"></a>
 
 # types-aiobotocore-voice-id
 
 [![PyPI - types-aiobotocore-voice-id](https://img.shields.io/pypi/v/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VoiceID 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[aiobotocore.VoiceID 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [types-aiobotocore-voice-id docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-voice-id-2.9.0/types_aiobotocore_voice_id.egg-info/SOURCES.txt` & `types-aiobotocore-voice-id-2.9.1/types_aiobotocore_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

