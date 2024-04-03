# Comparing `tmp/types-aiobotocore-chime-2.9.0.tar.gz` & `tmp/types-aiobotocore-chime-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-2.9.0.tar", last modified: Wed Dec 13 19:58:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-2.9.1.tar", last modified: Thu Jan 18 01:20:11 2024, max compression
```

## Comparing `types-aiobotocore-chime-2.9.0.tar` & `types-aiobotocore-chime-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:44.698011 types-aiobotocore-chime-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12914 2023-12-13 19:58:44.698011 types-aiobotocore-chime-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:44.698011 types-aiobotocore-chime-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:44.698011 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   127645 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   127641 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2023-12-13 19:41:56.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14069 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   122879 2023-12-13 19:41:58.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   122878 2023-12-13 19:41:57.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:55.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:44.698011 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12914 2023-12-13 19:58:44.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 19:58:44.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:44.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:44.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:44.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 19:58:44.000000 types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.881482 types-aiobotocore-chime-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:52.000000 types-aiobotocore-chime-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12934 2024-01-18 01:20:11.881482 types-aiobotocore-chime-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-01-18 01:03:52.000000 types-aiobotocore-chime-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:11.881482 types-aiobotocore-chime-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:03:52.000000 types-aiobotocore-chime-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.881482 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-18 01:03:52.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-18 01:03:52.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:03:52.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127684 2024-01-18 01:03:53.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127681 2024-01-18 01:03:53.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14069 2024-01-18 01:03:53.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14069 2024-01-18 01:03:53.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-01-18 01:03:53.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-01-18 01:03:53.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:52.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   122878 2024-01-18 01:03:56.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122878 2024-01-18 01:03:55.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:52.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.881482 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12934 2024-01-18 01:20:11.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-18 01:20:11.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:11.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:11.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:11.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:20:11.000000 types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-2.9.0/LICENSE` & `types-aiobotocore-chime-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-chime-2.9.0/PKG-INFO` & `types-aiobotocore-chime-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Chime 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Chime 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/
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
 
 <a id="types-aiobotocore-chime"></a>
 
 # types-aiobotocore-chime
 
 [![PyPI - types-aiobotocore-chime](https://img.shields.io/pypi/v/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[aiobotocore.Chime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [types-aiobotocore-chime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-2.9.0/README.md` & `types-aiobotocore-chime-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[aiobotocore.Chime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [types-aiobotocore-chime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-2.9.0/setup.py` & `types-aiobotocore-chime-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Chime 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Chime 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore chime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/__init__.py` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import ChimeClient
 from .paginator import ListAccountsPaginator, ListUsersPaginator
 
 Client = ChimeClient
 
-
 __all__ = ("ChimeClient", "Client", "ListAccountsPaginator", "ListUsersPaginator")
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/__init__.pyi` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/__main__.py` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Chime 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Chime 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
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

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/client.py` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ChimeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -289,15 +288,15 @@
         """
 
     async def associate_phone_numbers_with_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         E164PhoneNumbers: Sequence[str],
-        ForceAssociate: bool = ...
+        ForceAssociate: bool = ...,
     ) -> AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef:
         """
         Associates phone numbers with the specified Amazon Chime Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.associate_phone_numbers_with_voice_connector_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#associate_phone_numbers_with_voice_connector_group)
         """
@@ -326,15 +325,15 @@
 
     async def batch_create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArns: Sequence[str],
         Type: ChannelMembershipTypeType = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> BatchCreateChannelMembershipResponseTypeDef:
         """
         Adds a specified number of users to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.batch_create_channel_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#batch_create_channel_membership)
         """
@@ -429,15 +428,15 @@
 
     async def create_app_instance(
         self,
         *,
         Name: str,
         ClientRequestToken: str,
         Metadata: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppInstanceResponseTypeDef:
         """
         Creates an Amazon Chime SDK messaging `AppInstance` under an AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_app_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_app_instance)
         """
@@ -456,15 +455,15 @@
         self,
         *,
         AppInstanceArn: str,
         AppInstanceUserId: str,
         Name: str,
         ClientRequestToken: str,
         Metadata: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppInstanceUserResponseTypeDef:
         """
         Creates a user under an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_app_instance_user)
         """
@@ -495,15 +494,15 @@
         AppInstanceArn: str,
         Name: str,
         ClientRequestToken: str,
         Mode: ChannelModeType = ...,
         Privacy: ChannelPrivacyType = ...,
         Metadata: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel to which you can add users and send messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_channel)
         """
@@ -520,15 +519,15 @@
 
     async def create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         Type: ChannelMembershipTypeType,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> CreateChannelMembershipResponseTypeDef:
         """
         Adds a user to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_channel_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_channel_membership)
         """
@@ -547,15 +546,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_media_capture_pipeline)
         """
@@ -564,15 +563,15 @@
         self,
         *,
         ClientRequestToken: str,
         ExternalMeetingId: str = ...,
         MeetingHostId: str = ...,
         MediaRegion: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        NotificationsConfiguration: MeetingNotificationConfigurationTypeDef = ...
+        NotificationsConfiguration: MeetingNotificationConfigurationTypeDef = ...,
     ) -> CreateMeetingResponseTypeDef:
         """
         Creates a new Amazon Chime SDK meeting in the specified media Region with no
         initial
         attendees.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_meeting)
@@ -597,15 +596,15 @@
         *,
         ClientRequestToken: str,
         ExternalMeetingId: str = ...,
         MeetingHostId: str = ...,
         MediaRegion: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         NotificationsConfiguration: MeetingNotificationConfigurationTypeDef = ...,
-        Attendees: Sequence[CreateAttendeeRequestItemTypeDef] = ...
+        Attendees: Sequence[CreateAttendeeRequestItemTypeDef] = ...,
     ) -> CreateMeetingWithAttendeesResponseTypeDef:
         """
         Creates a new Amazon Chime SDK meeting in the specified media Region, with
         attendees.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_meeting_with_attendees)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_meeting_with_attendees)
@@ -627,15 +626,15 @@
         VoiceConnectorId: str,
         ParticipantPhoneNumbers: Sequence[str],
         Capabilities: Sequence[CapabilityType],
         Name: str = ...,
         ExpiryMinutes: int = ...,
         NumberSelectionBehavior: NumberSelectionBehaviorType = ...,
         GeoMatchLevel: GeoMatchLevelType = ...,
-        GeoMatchParams: GeoMatchParamsTypeDef = ...
+        GeoMatchParams: GeoMatchParamsTypeDef = ...,
     ) -> CreateProxySessionResponseTypeDef:
         """
         Creates a proxy session on the specified Amazon Chime Voice Connector for the
         specified participant phone
         numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_proxy_session)
@@ -674,15 +673,15 @@
 
     async def create_sip_media_application_call(
         self,
         *,
         FromPhoneNumber: str,
         ToPhoneNumber: str,
         SipMediaApplicationId: str,
-        SipHeaders: Mapping[str, str] = ...
+        SipHeaders: Mapping[str, str] = ...,
     ) -> CreateSipMediaApplicationCallResponseTypeDef:
         """
         Creates an outbound call to a phone number from the phone number specified in
         the request, and it invokes the endpoint of the specified
         `sipMediaApplicationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_sip_media_application_call)
@@ -692,15 +691,15 @@
     async def create_sip_rule(
         self,
         *,
         Name: str,
         TriggerType: SipRuleTriggerTypeType,
         TriggerValue: str,
         TargetApplications: Sequence[SipRuleTargetApplicationTypeDef],
-        Disabled: bool = ...
+        Disabled: bool = ...,
     ) -> CreateSipRuleResponseTypeDef:
         """
         Creates a SIP rule which can be used to run a SIP media application as a target
         for a specific trigger
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_sip_rule)
@@ -1592,15 +1591,15 @@
 
     async def list_channel_bans(
         self,
         *,
         ChannelArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelBansResponseTypeDef:
         """
         Lists all the users banned from a particular channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_bans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_bans)
         """
@@ -1608,30 +1607,30 @@
     async def list_channel_memberships(
         self,
         *,
         ChannelArn: str,
         Type: ChannelMembershipTypeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelMembershipsResponseTypeDef:
         """
         Lists all channel memberships in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_memberships)
         """
 
     async def list_channel_memberships_for_app_instance_user(
         self,
         *,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
         """
         Lists all channels that a particular `AppInstanceUser` is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_memberships_for_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_memberships_for_app_instance_user)
         """
@@ -1641,30 +1640,30 @@
         *,
         ChannelArn: str,
         SortOrder: SortOrderType = ...,
         NotBefore: TimestampTypeDef = ...,
         NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_messages)
         """
 
     async def list_channel_moderators(
         self,
         *,
         ChannelArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelModeratorsResponseTypeDef:
         """
         Lists all the moderators for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_moderators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_moderators)
         """
@@ -1672,30 +1671,30 @@
     async def list_channels(
         self,
         *,
         AppInstanceArn: str,
         Privacy: ChannelPrivacyType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelsResponseTypeDef:
         """
         Lists all Channels created under a single Chime App as a paginated list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channels)
         """
 
     async def list_channels_moderated_by_app_instance_user(
         self,
         *,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
         A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channels_moderated_by_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channels_moderated_by_app_instance_user)
         """
@@ -1742,15 +1741,15 @@
         self,
         *,
         Status: PhoneNumberStatusType = ...,
         ProductType: PhoneNumberProductTypeType = ...,
         FilterName: PhoneNumberAssociationNameType = ...,
         FilterValue: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPhoneNumbersResponseTypeDef:
         """
         Lists the phone numbers for the specified Amazon Chime account, Amazon Chime
         user, Amazon Chime Voice Connector, or Amazon Chime Voice Connector
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_phone_numbers)
@@ -1759,15 +1758,15 @@
 
     async def list_proxy_sessions(
         self,
         *,
         VoiceConnectorId: str,
         Status: ProxySessionStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProxySessionsResponseTypeDef:
         """
         Lists the proxy sessions for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_proxy_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_proxy_sessions)
         """
@@ -1837,15 +1836,15 @@
     async def list_users(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListUsersResponseTypeDef:
         """
         Lists the users that belong to the specified Amazon Chime account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_users)
         """
@@ -1890,43 +1889,43 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#logout_user)
         """
 
     async def put_app_instance_retention_settings(
         self,
         *,
         AppInstanceArn: str,
-        AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef
+        AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,
     ) -> PutAppInstanceRetentionSettingsResponseTypeDef:
         """
         Sets the amount of time in days that a given `AppInstance` retains data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_app_instance_retention_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_app_instance_retention_settings)
         """
 
     async def put_app_instance_streaming_configurations(
         self,
         *,
         AppInstanceArn: str,
-        AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef]
+        AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef],
     ) -> PutAppInstanceStreamingConfigurationsResponseTypeDef:
         """
         The data streaming configurations of an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_app_instance_streaming_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_app_instance_streaming_configurations)
         """
 
     async def put_events_configuration(
         self,
         *,
         AccountId: str,
         BotId: str,
         OutboundEventsHTTPSEndpoint: str = ...,
-        LambdaFunctionArn: str = ...
+        LambdaFunctionArn: str = ...,
     ) -> PutEventsConfigurationResponseTypeDef:
         """
         Creates an events configuration that allows a bot to receive outgoing events
         sent by Amazon
         Chime.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_events_configuration)
@@ -1943,28 +1942,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_retention_settings)
         """
 
     async def put_sip_media_application_logging_configuration(
         self,
         *,
         SipMediaApplicationId: str,
-        SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...
+        SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...,
     ) -> PutSipMediaApplicationLoggingConfigurationResponseTypeDef:
         """
         Updates the logging configuration for the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_sip_media_application_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_sip_media_application_logging_configuration)
         """
 
     async def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef,
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Puts emergency calling configuration details to the specified Amazon Chime
         Voice Connector, such as emergency phone numbers and calling
         countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
@@ -1994,15 +1993,15 @@
     async def put_voice_connector_proxy(
         self,
         *,
         VoiceConnectorId: str,
         DefaultSessionExpiryMinutes: int,
         PhoneNumberPoolCountries: Sequence[str],
         FallBackPhoneNumber: str = ...,
-        Disabled: bool = ...
+        Disabled: bool = ...,
     ) -> PutVoiceConnectorProxyResponseTypeDef:
         """
         Puts the specified proxy configuration to the specified Amazon Chime Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_proxy)
@@ -2106,15 +2105,15 @@
         AreaCode: str = ...,
         City: str = ...,
         Country: str = ...,
         State: str = ...,
         TollFreePrefix: str = ...,
         PhoneNumberType: PhoneNumberTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
         Searches for phone numbers that can be ordered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.search_available_phone_numbers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#search_available_phone_numbers)
         """
@@ -2124,15 +2123,15 @@
         *,
         ChannelArn: str,
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         Metadata: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.send_channel_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#send_channel_message)
         """
@@ -2270,15 +2269,15 @@
     async def update_channel(
         self,
         *,
         ChannelArn: str,
         Name: str,
         Mode: ChannelModeType,
         Metadata: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Update a channel's attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_channel)
         """
@@ -2286,15 +2285,15 @@
     async def update_channel_message(
         self,
         *,
         ChannelArn: str,
         MessageId: str,
         Content: str = ...,
         Metadata: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> UpdateChannelMessageResponseTypeDef:
         """
         Updates the content of a message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_channel_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_channel_message)
         """
@@ -2309,15 +2308,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_channel_read_marker)
         """
 
     async def update_global_settings(
         self,
         *,
         BusinessCalling: BusinessCallingSettingsTypeDef = ...,
-        VoiceConnector: VoiceConnectorSettingsTypeDef = ...
+        VoiceConnector: VoiceConnectorSettingsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates global settings for the administrator's AWS account, such as Amazon
         Chime Business Calling and Amazon Chime Voice Connector
         settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_global_settings)
@@ -2325,15 +2324,15 @@
         """
 
     async def update_phone_number(
         self,
         *,
         PhoneNumberId: str,
         ProductType: PhoneNumberProductTypeType = ...,
-        CallingName: str = ...
+        CallingName: str = ...,
     ) -> UpdatePhoneNumberResponseTypeDef:
         """
         Updates phone number details, such as product type or calling name, for the
         specified phone number
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_phone_number)
@@ -2354,15 +2353,15 @@
 
     async def update_proxy_session(
         self,
         *,
         VoiceConnectorId: str,
         ProxySessionId: str,
         Capabilities: Sequence[CapabilityType],
-        ExpiryMinutes: int = ...
+        ExpiryMinutes: int = ...,
     ) -> UpdateProxySessionResponseTypeDef:
         """
         Updates the specified proxy session details, such as voice or SMS capabilities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_proxy_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_proxy_session)
         """
@@ -2392,15 +2391,15 @@
         """
 
     async def update_sip_media_application(
         self,
         *,
         SipMediaApplicationId: str,
         Name: str = ...,
-        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...
+        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...,
     ) -> UpdateSipMediaApplicationResponseTypeDef:
         """
         Updates the details of the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_sip_media_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_sip_media_application)
         """
@@ -2419,15 +2418,15 @@
 
     async def update_sip_rule(
         self,
         *,
         SipRuleId: str,
         Name: str,
         Disabled: bool = ...,
-        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
+        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...,
     ) -> UpdateSipRuleResponseTypeDef:
         """
         Updates the details of the specified SIP rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_sip_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_sip_rule)
         """
@@ -2435,15 +2434,15 @@
     async def update_user(
         self,
         *,
         AccountId: str,
         UserId: str,
         LicenseType: LicenseType = ...,
         UserType: UserTypeType = ...,
-        AlexaForBusinessMetadata: AlexaForBusinessMetadataTypeDef = ...
+        AlexaForBusinessMetadata: AlexaForBusinessMetadataTypeDef = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates user details for a specified user ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_user)
         """
@@ -2469,15 +2468,15 @@
         """
 
     async def update_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         Name: str,
-        VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef]
+        VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef],
     ) -> UpdateVoiceConnectorGroupResponseTypeDef:
         """
         Updates details of the specified Amazon Chime Voice Connector group, such as
         the name and Amazon Chime Voice Connector priority
         ranking.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_voice_connector_group)
@@ -2489,15 +2488,15 @@
         *,
         AwsAccountId: str,
         StreetNumber: str,
         StreetInfo: str,
         City: str,
         State: str,
         Country: str,
-        PostalCode: str
+        PostalCode: str,
     ) -> ValidateE911AddressResponseTypeDef:
         """
         Validates an address to be used for 911 calls made with Amazon Chime Voice
         Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.validate_e911_address)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#validate_e911_address)
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/client.pyi` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         """
 
     async def associate_phone_numbers_with_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         E164PhoneNumbers: Sequence[str],
-        ForceAssociate: bool = ...
+        ForceAssociate: bool = ...,
     ) -> AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef:
         """
         Associates phone numbers with the specified Amazon Chime Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.associate_phone_numbers_with_voice_connector_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#associate_phone_numbers_with_voice_connector_group)
         """
@@ -322,15 +322,15 @@
 
     async def batch_create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArns: Sequence[str],
         Type: ChannelMembershipTypeType = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> BatchCreateChannelMembershipResponseTypeDef:
         """
         Adds a specified number of users to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.batch_create_channel_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#batch_create_channel_membership)
         """
@@ -425,15 +425,15 @@
 
     async def create_app_instance(
         self,
         *,
         Name: str,
         ClientRequestToken: str,
         Metadata: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppInstanceResponseTypeDef:
         """
         Creates an Amazon Chime SDK messaging `AppInstance` under an AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_app_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_app_instance)
         """
@@ -452,15 +452,15 @@
         self,
         *,
         AppInstanceArn: str,
         AppInstanceUserId: str,
         Name: str,
         ClientRequestToken: str,
         Metadata: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppInstanceUserResponseTypeDef:
         """
         Creates a user under an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_app_instance_user)
         """
@@ -491,15 +491,15 @@
         AppInstanceArn: str,
         Name: str,
         ClientRequestToken: str,
         Mode: ChannelModeType = ...,
         Privacy: ChannelPrivacyType = ...,
         Metadata: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel to which you can add users and send messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_channel)
         """
@@ -516,15 +516,15 @@
 
     async def create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         Type: ChannelMembershipTypeType,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> CreateChannelMembershipResponseTypeDef:
         """
         Adds a user to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_channel_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_channel_membership)
         """
@@ -543,15 +543,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_media_capture_pipeline)
         """
@@ -560,15 +560,15 @@
         self,
         *,
         ClientRequestToken: str,
         ExternalMeetingId: str = ...,
         MeetingHostId: str = ...,
         MediaRegion: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        NotificationsConfiguration: MeetingNotificationConfigurationTypeDef = ...
+        NotificationsConfiguration: MeetingNotificationConfigurationTypeDef = ...,
     ) -> CreateMeetingResponseTypeDef:
         """
         Creates a new Amazon Chime SDK meeting in the specified media Region with no
         initial
         attendees.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_meeting)
@@ -593,15 +593,15 @@
         *,
         ClientRequestToken: str,
         ExternalMeetingId: str = ...,
         MeetingHostId: str = ...,
         MediaRegion: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         NotificationsConfiguration: MeetingNotificationConfigurationTypeDef = ...,
-        Attendees: Sequence[CreateAttendeeRequestItemTypeDef] = ...
+        Attendees: Sequence[CreateAttendeeRequestItemTypeDef] = ...,
     ) -> CreateMeetingWithAttendeesResponseTypeDef:
         """
         Creates a new Amazon Chime SDK meeting in the specified media Region, with
         attendees.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_meeting_with_attendees)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_meeting_with_attendees)
@@ -623,15 +623,15 @@
         VoiceConnectorId: str,
         ParticipantPhoneNumbers: Sequence[str],
         Capabilities: Sequence[CapabilityType],
         Name: str = ...,
         ExpiryMinutes: int = ...,
         NumberSelectionBehavior: NumberSelectionBehaviorType = ...,
         GeoMatchLevel: GeoMatchLevelType = ...,
-        GeoMatchParams: GeoMatchParamsTypeDef = ...
+        GeoMatchParams: GeoMatchParamsTypeDef = ...,
     ) -> CreateProxySessionResponseTypeDef:
         """
         Creates a proxy session on the specified Amazon Chime Voice Connector for the
         specified participant phone
         numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_proxy_session)
@@ -670,15 +670,15 @@
 
     async def create_sip_media_application_call(
         self,
         *,
         FromPhoneNumber: str,
         ToPhoneNumber: str,
         SipMediaApplicationId: str,
-        SipHeaders: Mapping[str, str] = ...
+        SipHeaders: Mapping[str, str] = ...,
     ) -> CreateSipMediaApplicationCallResponseTypeDef:
         """
         Creates an outbound call to a phone number from the phone number specified in
         the request, and it invokes the endpoint of the specified
         `sipMediaApplicationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_sip_media_application_call)
@@ -688,15 +688,15 @@
     async def create_sip_rule(
         self,
         *,
         Name: str,
         TriggerType: SipRuleTriggerTypeType,
         TriggerValue: str,
         TargetApplications: Sequence[SipRuleTargetApplicationTypeDef],
-        Disabled: bool = ...
+        Disabled: bool = ...,
     ) -> CreateSipRuleResponseTypeDef:
         """
         Creates a SIP rule which can be used to run a SIP media application as a target
         for a specific trigger
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_sip_rule)
@@ -1588,15 +1588,15 @@
 
     async def list_channel_bans(
         self,
         *,
         ChannelArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelBansResponseTypeDef:
         """
         Lists all the users banned from a particular channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_bans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_bans)
         """
@@ -1604,30 +1604,30 @@
     async def list_channel_memberships(
         self,
         *,
         ChannelArn: str,
         Type: ChannelMembershipTypeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelMembershipsResponseTypeDef:
         """
         Lists all channel memberships in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_memberships)
         """
 
     async def list_channel_memberships_for_app_instance_user(
         self,
         *,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
         """
         Lists all channels that a particular `AppInstanceUser` is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_memberships_for_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_memberships_for_app_instance_user)
         """
@@ -1637,30 +1637,30 @@
         *,
         ChannelArn: str,
         SortOrder: SortOrderType = ...,
         NotBefore: TimestampTypeDef = ...,
         NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_messages)
         """
 
     async def list_channel_moderators(
         self,
         *,
         ChannelArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelModeratorsResponseTypeDef:
         """
         Lists all the moderators for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channel_moderators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_moderators)
         """
@@ -1668,30 +1668,30 @@
     async def list_channels(
         self,
         *,
         AppInstanceArn: str,
         Privacy: ChannelPrivacyType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelsResponseTypeDef:
         """
         Lists all Channels created under a single Chime App as a paginated list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channels)
         """
 
     async def list_channels_moderated_by_app_instance_user(
         self,
         *,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
         A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channels_moderated_by_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channels_moderated_by_app_instance_user)
         """
@@ -1738,15 +1738,15 @@
         self,
         *,
         Status: PhoneNumberStatusType = ...,
         ProductType: PhoneNumberProductTypeType = ...,
         FilterName: PhoneNumberAssociationNameType = ...,
         FilterValue: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPhoneNumbersResponseTypeDef:
         """
         Lists the phone numbers for the specified Amazon Chime account, Amazon Chime
         user, Amazon Chime Voice Connector, or Amazon Chime Voice Connector
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_phone_numbers)
@@ -1755,15 +1755,15 @@
 
     async def list_proxy_sessions(
         self,
         *,
         VoiceConnectorId: str,
         Status: ProxySessionStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProxySessionsResponseTypeDef:
         """
         Lists the proxy sessions for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_proxy_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_proxy_sessions)
         """
@@ -1833,15 +1833,15 @@
     async def list_users(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListUsersResponseTypeDef:
         """
         Lists the users that belong to the specified Amazon Chime account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_users)
         """
@@ -1886,43 +1886,43 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#logout_user)
         """
 
     async def put_app_instance_retention_settings(
         self,
         *,
         AppInstanceArn: str,
-        AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef
+        AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,
     ) -> PutAppInstanceRetentionSettingsResponseTypeDef:
         """
         Sets the amount of time in days that a given `AppInstance` retains data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_app_instance_retention_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_app_instance_retention_settings)
         """
 
     async def put_app_instance_streaming_configurations(
         self,
         *,
         AppInstanceArn: str,
-        AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef]
+        AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef],
     ) -> PutAppInstanceStreamingConfigurationsResponseTypeDef:
         """
         The data streaming configurations of an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_app_instance_streaming_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_app_instance_streaming_configurations)
         """
 
     async def put_events_configuration(
         self,
         *,
         AccountId: str,
         BotId: str,
         OutboundEventsHTTPSEndpoint: str = ...,
-        LambdaFunctionArn: str = ...
+        LambdaFunctionArn: str = ...,
     ) -> PutEventsConfigurationResponseTypeDef:
         """
         Creates an events configuration that allows a bot to receive outgoing events
         sent by Amazon
         Chime.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_events_configuration)
@@ -1939,28 +1939,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_retention_settings)
         """
 
     async def put_sip_media_application_logging_configuration(
         self,
         *,
         SipMediaApplicationId: str,
-        SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...
+        SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...,
     ) -> PutSipMediaApplicationLoggingConfigurationResponseTypeDef:
         """
         Updates the logging configuration for the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_sip_media_application_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_sip_media_application_logging_configuration)
         """
 
     async def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef,
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Puts emergency calling configuration details to the specified Amazon Chime
         Voice Connector, such as emergency phone numbers and calling
         countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
@@ -1990,15 +1990,15 @@
     async def put_voice_connector_proxy(
         self,
         *,
         VoiceConnectorId: str,
         DefaultSessionExpiryMinutes: int,
         PhoneNumberPoolCountries: Sequence[str],
         FallBackPhoneNumber: str = ...,
-        Disabled: bool = ...
+        Disabled: bool = ...,
     ) -> PutVoiceConnectorProxyResponseTypeDef:
         """
         Puts the specified proxy configuration to the specified Amazon Chime Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_proxy)
@@ -2102,15 +2102,15 @@
         AreaCode: str = ...,
         City: str = ...,
         Country: str = ...,
         State: str = ...,
         TollFreePrefix: str = ...,
         PhoneNumberType: PhoneNumberTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
         Searches for phone numbers that can be ordered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.search_available_phone_numbers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#search_available_phone_numbers)
         """
@@ -2120,15 +2120,15 @@
         *,
         ChannelArn: str,
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         Metadata: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.send_channel_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#send_channel_message)
         """
@@ -2266,15 +2266,15 @@
     async def update_channel(
         self,
         *,
         ChannelArn: str,
         Name: str,
         Mode: ChannelModeType,
         Metadata: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Update a channel's attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_channel)
         """
@@ -2282,15 +2282,15 @@
     async def update_channel_message(
         self,
         *,
         ChannelArn: str,
         MessageId: str,
         Content: str = ...,
         Metadata: str = ...,
-        ChimeBearer: str = ...
+        ChimeBearer: str = ...,
     ) -> UpdateChannelMessageResponseTypeDef:
         """
         Updates the content of a message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_channel_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_channel_message)
         """
@@ -2305,15 +2305,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_channel_read_marker)
         """
 
     async def update_global_settings(
         self,
         *,
         BusinessCalling: BusinessCallingSettingsTypeDef = ...,
-        VoiceConnector: VoiceConnectorSettingsTypeDef = ...
+        VoiceConnector: VoiceConnectorSettingsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates global settings for the administrator's AWS account, such as Amazon
         Chime Business Calling and Amazon Chime Voice Connector
         settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_global_settings)
@@ -2321,15 +2321,15 @@
         """
 
     async def update_phone_number(
         self,
         *,
         PhoneNumberId: str,
         ProductType: PhoneNumberProductTypeType = ...,
-        CallingName: str = ...
+        CallingName: str = ...,
     ) -> UpdatePhoneNumberResponseTypeDef:
         """
         Updates phone number details, such as product type or calling name, for the
         specified phone number
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_phone_number)
@@ -2350,15 +2350,15 @@
 
     async def update_proxy_session(
         self,
         *,
         VoiceConnectorId: str,
         ProxySessionId: str,
         Capabilities: Sequence[CapabilityType],
-        ExpiryMinutes: int = ...
+        ExpiryMinutes: int = ...,
     ) -> UpdateProxySessionResponseTypeDef:
         """
         Updates the specified proxy session details, such as voice or SMS capabilities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_proxy_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_proxy_session)
         """
@@ -2388,15 +2388,15 @@
         """
 
     async def update_sip_media_application(
         self,
         *,
         SipMediaApplicationId: str,
         Name: str = ...,
-        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...
+        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...,
     ) -> UpdateSipMediaApplicationResponseTypeDef:
         """
         Updates the details of the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_sip_media_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_sip_media_application)
         """
@@ -2415,15 +2415,15 @@
 
     async def update_sip_rule(
         self,
         *,
         SipRuleId: str,
         Name: str,
         Disabled: bool = ...,
-        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
+        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...,
     ) -> UpdateSipRuleResponseTypeDef:
         """
         Updates the details of the specified SIP rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_sip_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_sip_rule)
         """
@@ -2431,15 +2431,15 @@
     async def update_user(
         self,
         *,
         AccountId: str,
         UserId: str,
         LicenseType: LicenseType = ...,
         UserType: UserTypeType = ...,
-        AlexaForBusinessMetadata: AlexaForBusinessMetadataTypeDef = ...
+        AlexaForBusinessMetadata: AlexaForBusinessMetadataTypeDef = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates user details for a specified user ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#update_user)
         """
@@ -2465,15 +2465,15 @@
         """
 
     async def update_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         Name: str,
-        VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef]
+        VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef],
     ) -> UpdateVoiceConnectorGroupResponseTypeDef:
         """
         Updates details of the specified Amazon Chime Voice Connector group, such as
         the name and Amazon Chime Voice Connector priority
         ranking.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.update_voice_connector_group)
@@ -2485,15 +2485,15 @@
         *,
         AwsAccountId: str,
         StreetNumber: str,
         StreetInfo: str,
         City: str,
         State: str,
         Country: str,
-        PostalCode: str
+        PostalCode: str,
     ) -> ValidateE911AddressResponseTypeDef:
         """
         Validates an address to be used for 911 calls made with Amazon Chime Voice
         Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.validate_e911_address)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#validate_e911_address)
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/literals.py` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/literals.py`

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
     "AccountStatusType",
     "AccountTypeType",
     "AppInstanceDataTypeType",
     "ArtifactsStateType",
     "AudioMuxTypeType",
     "BotTypeType",
@@ -76,15 +75,14 @@
     "VoiceConnectorAwsRegionType",
     "ChimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AccountStatusType = Literal["Active", "Suspended"]
 AccountTypeType = Literal["EnterpriseDirectory", "EnterpriseLWA", "EnterpriseOIDC", "Team"]
 AppInstanceDataTypeType = Literal["Channel", "ChannelMessage"]
 ArtifactsStateType = Literal["Disabled", "Enabled"]
 AudioMuxTypeType = Literal["AudioOnly", "AudioWithActiveSpeakerVideo"]
 BotTypeType = Literal["ChatBot"]
 CallingNameStatusType = Literal["Unassigned", "UpdateFailed", "UpdateInProgress", "UpdateSucceeded"]
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/literals.pyi` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/paginator.py` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from botocore.paginate import PageIterator
 
 from .literals import UserTypeType
 from .type_defs import ListAccountsResponseTypeDef, ListUsersResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListAccountsPaginator", "ListUsersPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -51,15 +50,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str = ...,
         UserEmail: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/paginators/#listaccountspaginator)
         """
 
 
@@ -71,13 +70,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/paginator.pyi` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str = ...,
         UserEmail: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/paginators/#listaccountspaginator)
         """
 
 class ListUsersPaginator(AioPaginator):
@@ -67,13 +67,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/type_defs.py` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSettingsTypeDef",
     "SigninDelegateGroupTypeDef",
     "AddressTypeDef",
     "AlexaForBusinessMetadataTypeDef",
     "IdentityTypeDef",
     "ChannelRetentionSettingsTypeDef",
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime/type_defs.pyi` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/PKG-INFO` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Chime 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Chime 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/
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
 
 <a id="types-aiobotocore-chime"></a>
 
 # types-aiobotocore-chime
 
 [![PyPI - types-aiobotocore-chime](https://img.shields.io/pypi/v/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[aiobotocore.Chime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [types-aiobotocore-chime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-2.9.0/types_aiobotocore_chime.egg-info/SOURCES.txt` & `types-aiobotocore-chime-2.9.1/types_aiobotocore_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

