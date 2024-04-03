# Comparing `tmp/types-aiobotocore-sesv2-2.9.0.tar.gz` & `tmp/types-aiobotocore-sesv2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sesv2-2.9.0.tar", last modified: Wed Dec 13 20:00:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-sesv2-2.9.1.tar", last modified: Thu Jan 18 01:21:49 2024, max compression
```

## Comparing `types-aiobotocore-sesv2-2.9.0.tar` & `types-aiobotocore-sesv2-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:31.369130 types-aiobotocore-sesv2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12129 2023-12-13 20:00:31.369130 types-aiobotocore-sesv2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:31.369130 types-aiobotocore-sesv2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:31.369130 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63048 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    63045 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13052 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    66440 2023-12-13 19:56:32.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    66439 2023-12-13 19:56:28.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:27.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:31.369130 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12129 2023-12-13 20:00:31.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-13 20:00:31.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:31.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:31.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:31.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 20:00:31.000000 types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:49.705030 types-aiobotocore-sesv2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-01-18 01:21:49.705030 types-aiobotocore-sesv2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:49.705030 types-aiobotocore-sesv2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:49.705030 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63074 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63071 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-01-18 01:17:59.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-01-18 01:17:59.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    66439 2024-01-18 01:18:00.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66439 2024-01-18 01:17:59.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:58.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:49.705030 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-01-18 01:21:49.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-18 01:21:49.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:49.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:49.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:49.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:21:49.000000 types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sesv2-2.9.0/LICENSE` & `types-aiobotocore-sesv2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sesv2-2.9.0/PKG-INFO` & `types-aiobotocore-sesv2-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sesv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SESV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SESV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/
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
 
 <a id="types-aiobotocore-sesv2"></a>
 
 # types-aiobotocore-sesv2
 
 [![PyPI - types-aiobotocore-sesv2](https://img.shields.io/pypi/v/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sesv2)](https://pepy.tech/project/types-aiobotocore-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SESV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[aiobotocore.SESV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [types-aiobotocore-sesv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sesv2-2.9.0/README.md` & `types-aiobotocore-sesv2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sesv2)](https://pepy.tech/project/types-aiobotocore-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SESV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[aiobotocore.SESV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [types-aiobotocore-sesv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sesv2-2.9.0/setup.py` & `types-aiobotocore-sesv2-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sesv2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SESV2 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SESV2 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore sesv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sesv2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/__main__.py` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SESV2 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SESV2 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
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

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/client.py` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,29 +193,29 @@
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
         ReputationOptions: ReputationOptionsTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SuppressionOptions: SuppressionOptionsTypeDef = ...,
-        VdmOptions: VdmOptionsTypeDef = ...
+        VdmOptions: VdmOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_configuration_set)
         """
 
     async def create_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef
+        EventDestination: EventDestinationDefinitionTypeDef,
     ) -> Dict[str, Any]:
         """
         Create an event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_configuration_set_event_destination)
         """
@@ -223,15 +223,15 @@
     async def create_contact(
         self,
         *,
         ContactListName: str,
         EmailAddress: str,
         TopicPreferences: Sequence[TopicPreferenceTypeDef] = ...,
         UnsubscribeAll: bool = ...,
-        AttributesData: str = ...
+        AttributesData: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a contact, which is an end-user who is receiving the email, and adds
         them to a contact
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_contact)
@@ -240,15 +240,15 @@
 
     async def create_contact_list(
         self,
         *,
         ContactListName: str,
         Topics: Sequence[TopicTypeDef] = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a contact list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_contact_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_contact_list)
         """
@@ -257,15 +257,15 @@
         self,
         *,
         TemplateName: str,
         FromEmailAddress: str,
         TemplateSubject: str,
         TemplateContent: str,
         SuccessRedirectionURL: str,
-        FailureRedirectionURL: str
+        FailureRedirectionURL: str,
     ) -> Dict[str, Any]:
         """
         Creates a new custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_custom_verification_email_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_custom_verification_email_template)
         """
@@ -282,30 +282,30 @@
 
     async def create_deliverability_test_report(
         self,
         *,
         FromEmailAddress: str,
         Content: EmailContentTypeDef,
         ReportName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDeliverabilityTestReportResponseTypeDef:
         """
         Create a new predictive inbox placement test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_deliverability_test_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_deliverability_test_report)
         """
 
     async def create_email_identity(
         self,
         *,
         EmailIdentity: str,
         Tags: Sequence[TagTypeDef] = ...,
         DkimSigningAttributes: DkimSigningAttributesTypeDef = ...,
-        ConfigurationSetName: str = ...
+        ConfigurationSetName: str = ...,
     ) -> CreateEmailIdentityResponseTypeDef:
         """
         Starts the process of verifying an email identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_email_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_email_identity)
         """
@@ -332,28 +332,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_email_template)
         """
 
     async def create_export_job(
         self,
         *,
         ExportDataSource: ExportDataSourceTypeDef,
-        ExportDestination: ExportDestinationTypeDef
+        ExportDestination: ExportDestinationTypeDef,
     ) -> CreateExportJobResponseTypeDef:
         """
         Creates an export job for a data source and destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_export_job)
         """
 
     async def create_import_job(
         self,
         *,
         ImportDestination: ImportDestinationTypeDef,
-        ImportDataSource: ImportDataSourceTypeDef
+        ImportDataSource: ImportDataSourceTypeDef,
     ) -> CreateImportJobResponseTypeDef:
         """
         Creates an import job for a data destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_import_job)
         """
@@ -702,15 +702,15 @@
 
     async def list_contacts(
         self,
         *,
         ContactListName: str,
         Filter: ListContactsFilterTypeDef = ...,
         PageSize: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListContactsResponseTypeDef:
         """
         Lists the contacts present in a specific contact list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_contacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_contacts)
         """
@@ -754,15 +754,15 @@
     async def list_domain_deliverability_campaigns(
         self,
         *,
         StartDate: TimestampTypeDef,
         EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListDomainDeliverabilityCampaignsResponseTypeDef:
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_domain_deliverability_campaigns)
@@ -795,43 +795,43 @@
 
     async def list_export_jobs(
         self,
         *,
         NextToken: str = ...,
         PageSize: int = ...,
         ExportSourceType: ExportSourceTypeType = ...,
-        JobStatus: JobStatusType = ...
+        JobStatus: JobStatusType = ...,
     ) -> ListExportJobsResponseTypeDef:
         """
         Lists all of the export jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_export_jobs)
         """
 
     async def list_import_jobs(
         self,
         *,
         ImportDestinationType: ImportDestinationTypeType = ...,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListImportJobsResponseTypeDef:
         """
         Lists all of the import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_import_jobs)
         """
 
     async def list_recommendations(
         self,
         *,
         Filter: Mapping[ListRecommendationsFilterKeyType, str] = ...,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         Lists the recommendations present in your Amazon SES account in the current
         Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_recommendations)
@@ -841,15 +841,15 @@
     async def list_suppressed_destinations(
         self,
         *,
         Reasons: Sequence[SuppressionListReasonType] = ...,
         StartDate: TimestampTypeDef = ...,
         EndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListSuppressedDestinationsResponseTypeDef:
         """
         Retrieves a list of email addresses that are on the suppression list for your
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_suppressed_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_suppressed_destinations)
@@ -881,15 +881,15 @@
         self,
         *,
         MailType: MailTypeType,
         WebsiteURL: str,
         UseCaseDescription: str,
         ContactLanguage: ContactLanguageType = ...,
         AdditionalContactEmailAddresses: Sequence[str] = ...,
-        ProductionAccessEnabled: bool = ...
+        ProductionAccessEnabled: bool = ...,
     ) -> Dict[str, Any]:
         """
         Update your Amazon SES account details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_account_details)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_account_details)
         """
@@ -923,15 +923,15 @@
         """
 
     async def put_configuration_set_delivery_options(
         self,
         *,
         ConfigurationSetName: str,
         TlsPolicy: TlsPolicyType = ...,
-        SendingPoolName: str = ...
+        SendingPoolName: str = ...,
     ) -> Dict[str, Any]:
         """
         Associate a configuration set with a dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_delivery_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_configuration_set_delivery_options)
         """
@@ -960,15 +960,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_configuration_set_sending_options)
         """
 
     async def put_configuration_set_suppression_options(
         self,
         *,
         ConfigurationSetName: str,
-        SuppressedReasons: Sequence[SuppressionListReasonType] = ...
+        SuppressedReasons: Sequence[SuppressionListReasonType] = ...,
     ) -> Dict[str, Any]:
         """
         Specify the account suppression list preferences for a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_suppression_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_configuration_set_suppression_options)
         """
@@ -1026,15 +1026,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_dedicated_ip_warmup_attributes)
         """
 
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_deliverability_dashboard_option)
         """
@@ -1060,15 +1060,15 @@
         """
 
     async def put_email_identity_dkim_signing_attributes(
         self,
         *,
         EmailIdentity: str,
         SigningAttributesOrigin: DkimSigningAttributesOriginType,
-        SigningAttributes: DkimSigningAttributesTypeDef = ...
+        SigningAttributes: DkimSigningAttributesTypeDef = ...,
     ) -> PutEmailIdentityDkimSigningAttributesResponseTypeDef:
         """
         Used to configure or change the DKIM authentication settings for an email
         domain
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_dkim_signing_attributes)
@@ -1086,15 +1086,15 @@
         """
 
     async def put_email_identity_mail_from_attributes(
         self,
         *,
         EmailIdentity: str,
         MailFromDomain: str = ...,
-        BehaviorOnMxFailure: BehaviorOnMxFailureType = ...
+        BehaviorOnMxFailure: BehaviorOnMxFailureType = ...,
     ) -> Dict[str, Any]:
         """
         Used to enable or disable the custom Mail-From domain configuration for an
         email
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_mail_from_attributes)
@@ -1118,15 +1118,15 @@
         BulkEmailEntries: Sequence[BulkEmailEntryTypeDef],
         FromEmailAddress: str = ...,
         FromEmailAddressIdentityArn: str = ...,
         ReplyToAddresses: Sequence[str] = ...,
         FeedbackForwardingEmailAddress: str = ...,
         FeedbackForwardingEmailAddressIdentityArn: str = ...,
         DefaultEmailTags: Sequence[MessageTagTypeDef] = ...,
-        ConfigurationSetName: str = ...
+        ConfigurationSetName: str = ...,
     ) -> SendBulkEmailResponseTypeDef:
         """
         Composes an email message to multiple destinations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.send_bulk_email)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#send_bulk_email)
         """
@@ -1151,15 +1151,15 @@
         FromEmailAddressIdentityArn: str = ...,
         Destination: DestinationTypeDef = ...,
         ReplyToAddresses: Sequence[str] = ...,
         FeedbackForwardingEmailAddress: str = ...,
         FeedbackForwardingEmailAddressIdentityArn: str = ...,
         EmailTags: Sequence[MessageTagTypeDef] = ...,
         ConfigurationSetName: str = ...,
-        ListManagementOptions: ListManagementOptionsTypeDef = ...
+        ListManagementOptions: ListManagementOptionsTypeDef = ...,
     ) -> SendEmailResponseTypeDef:
         """
         Sends an email message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.send_email)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#send_email)
         """
@@ -1193,15 +1193,15 @@
         """
 
     async def update_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef
+        EventDestination: EventDestinationDefinitionTypeDef,
     ) -> Dict[str, Any]:
         """
         Update the configuration of an event destination for a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#update_configuration_set_event_destination)
         """
@@ -1209,15 +1209,15 @@
     async def update_contact(
         self,
         *,
         ContactListName: str,
         EmailAddress: str,
         TopicPreferences: Sequence[TopicPreferenceTypeDef] = ...,
         UnsubscribeAll: bool = ...,
-        AttributesData: str = ...
+        AttributesData: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a contact's preferences for a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#update_contact)
         """
@@ -1236,15 +1236,15 @@
         self,
         *,
         TemplateName: str,
         FromEmailAddress: str,
         TemplateSubject: str,
         TemplateContent: str,
         SuccessRedirectionURL: str,
-        FailureRedirectionURL: str
+        FailureRedirectionURL: str,
     ) -> Dict[str, Any]:
         """
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_custom_verification_email_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#update_custom_verification_email_template)
         """
```

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/client.pyi` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -190,29 +190,29 @@
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
         ReputationOptions: ReputationOptionsTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SuppressionOptions: SuppressionOptionsTypeDef = ...,
-        VdmOptions: VdmOptionsTypeDef = ...
+        VdmOptions: VdmOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_configuration_set)
         """
 
     async def create_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef
+        EventDestination: EventDestinationDefinitionTypeDef,
     ) -> Dict[str, Any]:
         """
         Create an event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_configuration_set_event_destination)
         """
@@ -220,15 +220,15 @@
     async def create_contact(
         self,
         *,
         ContactListName: str,
         EmailAddress: str,
         TopicPreferences: Sequence[TopicPreferenceTypeDef] = ...,
         UnsubscribeAll: bool = ...,
-        AttributesData: str = ...
+        AttributesData: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a contact, which is an end-user who is receiving the email, and adds
         them to a contact
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_contact)
@@ -237,15 +237,15 @@
 
     async def create_contact_list(
         self,
         *,
         ContactListName: str,
         Topics: Sequence[TopicTypeDef] = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a contact list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_contact_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_contact_list)
         """
@@ -254,15 +254,15 @@
         self,
         *,
         TemplateName: str,
         FromEmailAddress: str,
         TemplateSubject: str,
         TemplateContent: str,
         SuccessRedirectionURL: str,
-        FailureRedirectionURL: str
+        FailureRedirectionURL: str,
     ) -> Dict[str, Any]:
         """
         Creates a new custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_custom_verification_email_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_custom_verification_email_template)
         """
@@ -279,30 +279,30 @@
 
     async def create_deliverability_test_report(
         self,
         *,
         FromEmailAddress: str,
         Content: EmailContentTypeDef,
         ReportName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDeliverabilityTestReportResponseTypeDef:
         """
         Create a new predictive inbox placement test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_deliverability_test_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_deliverability_test_report)
         """
 
     async def create_email_identity(
         self,
         *,
         EmailIdentity: str,
         Tags: Sequence[TagTypeDef] = ...,
         DkimSigningAttributes: DkimSigningAttributesTypeDef = ...,
-        ConfigurationSetName: str = ...
+        ConfigurationSetName: str = ...,
     ) -> CreateEmailIdentityResponseTypeDef:
         """
         Starts the process of verifying an email identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_email_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_email_identity)
         """
@@ -329,28 +329,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_email_template)
         """
 
     async def create_export_job(
         self,
         *,
         ExportDataSource: ExportDataSourceTypeDef,
-        ExportDestination: ExportDestinationTypeDef
+        ExportDestination: ExportDestinationTypeDef,
     ) -> CreateExportJobResponseTypeDef:
         """
         Creates an export job for a data source and destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_export_job)
         """
 
     async def create_import_job(
         self,
         *,
         ImportDestination: ImportDestinationTypeDef,
-        ImportDataSource: ImportDataSourceTypeDef
+        ImportDataSource: ImportDataSourceTypeDef,
     ) -> CreateImportJobResponseTypeDef:
         """
         Creates an import job for a data destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_import_job)
         """
@@ -699,15 +699,15 @@
 
     async def list_contacts(
         self,
         *,
         ContactListName: str,
         Filter: ListContactsFilterTypeDef = ...,
         PageSize: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListContactsResponseTypeDef:
         """
         Lists the contacts present in a specific contact list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_contacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_contacts)
         """
@@ -751,15 +751,15 @@
     async def list_domain_deliverability_campaigns(
         self,
         *,
         StartDate: TimestampTypeDef,
         EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListDomainDeliverabilityCampaignsResponseTypeDef:
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_domain_deliverability_campaigns)
@@ -792,43 +792,43 @@
 
     async def list_export_jobs(
         self,
         *,
         NextToken: str = ...,
         PageSize: int = ...,
         ExportSourceType: ExportSourceTypeType = ...,
-        JobStatus: JobStatusType = ...
+        JobStatus: JobStatusType = ...,
     ) -> ListExportJobsResponseTypeDef:
         """
         Lists all of the export jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_export_jobs)
         """
 
     async def list_import_jobs(
         self,
         *,
         ImportDestinationType: ImportDestinationTypeType = ...,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListImportJobsResponseTypeDef:
         """
         Lists all of the import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_import_jobs)
         """
 
     async def list_recommendations(
         self,
         *,
         Filter: Mapping[ListRecommendationsFilterKeyType, str] = ...,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         Lists the recommendations present in your Amazon SES account in the current
         Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_recommendations)
@@ -838,15 +838,15 @@
     async def list_suppressed_destinations(
         self,
         *,
         Reasons: Sequence[SuppressionListReasonType] = ...,
         StartDate: TimestampTypeDef = ...,
         EndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListSuppressedDestinationsResponseTypeDef:
         """
         Retrieves a list of email addresses that are on the suppression list for your
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_suppressed_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_suppressed_destinations)
@@ -878,15 +878,15 @@
         self,
         *,
         MailType: MailTypeType,
         WebsiteURL: str,
         UseCaseDescription: str,
         ContactLanguage: ContactLanguageType = ...,
         AdditionalContactEmailAddresses: Sequence[str] = ...,
-        ProductionAccessEnabled: bool = ...
+        ProductionAccessEnabled: bool = ...,
     ) -> Dict[str, Any]:
         """
         Update your Amazon SES account details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_account_details)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_account_details)
         """
@@ -920,15 +920,15 @@
         """
 
     async def put_configuration_set_delivery_options(
         self,
         *,
         ConfigurationSetName: str,
         TlsPolicy: TlsPolicyType = ...,
-        SendingPoolName: str = ...
+        SendingPoolName: str = ...,
     ) -> Dict[str, Any]:
         """
         Associate a configuration set with a dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_delivery_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_configuration_set_delivery_options)
         """
@@ -957,15 +957,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_configuration_set_sending_options)
         """
 
     async def put_configuration_set_suppression_options(
         self,
         *,
         ConfigurationSetName: str,
-        SuppressedReasons: Sequence[SuppressionListReasonType] = ...
+        SuppressedReasons: Sequence[SuppressionListReasonType] = ...,
     ) -> Dict[str, Any]:
         """
         Specify the account suppression list preferences for a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_suppression_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_configuration_set_suppression_options)
         """
@@ -1023,15 +1023,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_dedicated_ip_warmup_attributes)
         """
 
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_deliverability_dashboard_option)
         """
@@ -1057,15 +1057,15 @@
         """
 
     async def put_email_identity_dkim_signing_attributes(
         self,
         *,
         EmailIdentity: str,
         SigningAttributesOrigin: DkimSigningAttributesOriginType,
-        SigningAttributes: DkimSigningAttributesTypeDef = ...
+        SigningAttributes: DkimSigningAttributesTypeDef = ...,
     ) -> PutEmailIdentityDkimSigningAttributesResponseTypeDef:
         """
         Used to configure or change the DKIM authentication settings for an email
         domain
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_dkim_signing_attributes)
@@ -1083,15 +1083,15 @@
         """
 
     async def put_email_identity_mail_from_attributes(
         self,
         *,
         EmailIdentity: str,
         MailFromDomain: str = ...,
-        BehaviorOnMxFailure: BehaviorOnMxFailureType = ...
+        BehaviorOnMxFailure: BehaviorOnMxFailureType = ...,
     ) -> Dict[str, Any]:
         """
         Used to enable or disable the custom Mail-From domain configuration for an
         email
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_mail_from_attributes)
@@ -1115,15 +1115,15 @@
         BulkEmailEntries: Sequence[BulkEmailEntryTypeDef],
         FromEmailAddress: str = ...,
         FromEmailAddressIdentityArn: str = ...,
         ReplyToAddresses: Sequence[str] = ...,
         FeedbackForwardingEmailAddress: str = ...,
         FeedbackForwardingEmailAddressIdentityArn: str = ...,
         DefaultEmailTags: Sequence[MessageTagTypeDef] = ...,
-        ConfigurationSetName: str = ...
+        ConfigurationSetName: str = ...,
     ) -> SendBulkEmailResponseTypeDef:
         """
         Composes an email message to multiple destinations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.send_bulk_email)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#send_bulk_email)
         """
@@ -1148,15 +1148,15 @@
         FromEmailAddressIdentityArn: str = ...,
         Destination: DestinationTypeDef = ...,
         ReplyToAddresses: Sequence[str] = ...,
         FeedbackForwardingEmailAddress: str = ...,
         FeedbackForwardingEmailAddressIdentityArn: str = ...,
         EmailTags: Sequence[MessageTagTypeDef] = ...,
         ConfigurationSetName: str = ...,
-        ListManagementOptions: ListManagementOptionsTypeDef = ...
+        ListManagementOptions: ListManagementOptionsTypeDef = ...,
     ) -> SendEmailResponseTypeDef:
         """
         Sends an email message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.send_email)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#send_email)
         """
@@ -1190,15 +1190,15 @@
         """
 
     async def update_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef
+        EventDestination: EventDestinationDefinitionTypeDef,
     ) -> Dict[str, Any]:
         """
         Update the configuration of an event destination for a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#update_configuration_set_event_destination)
         """
@@ -1206,15 +1206,15 @@
     async def update_contact(
         self,
         *,
         ContactListName: str,
         EmailAddress: str,
         TopicPreferences: Sequence[TopicPreferenceTypeDef] = ...,
         UnsubscribeAll: bool = ...,
-        AttributesData: str = ...
+        AttributesData: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a contact's preferences for a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#update_contact)
         """
@@ -1233,15 +1233,15 @@
         self,
         *,
         TemplateName: str,
         FromEmailAddress: str,
         TemplateSubject: str,
         TemplateContent: str,
         SuccessRedirectionURL: str,
-        FailureRedirectionURL: str
+        FailureRedirectionURL: str,
     ) -> Dict[str, Any]:
         """
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_custom_verification_email_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#update_custom_verification_email_template)
         """
```

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/literals.py` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/literals.py`

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
     "BehaviorOnMxFailureType",
     "BounceTypeType",
     "BulkEmailStatusType",
     "ContactLanguageType",
     "ContactListImportActionType",
     "DataFormatType",
@@ -63,15 +62,14 @@
     "WarmupStatusType",
     "SESV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BehaviorOnMxFailureType = Literal["REJECT_MESSAGE", "USE_DEFAULT_VALUE"]
 BounceTypeType = Literal["PERMANENT", "TRANSIENT", "UNDETERMINED"]
 BulkEmailStatusType = Literal[
     "ACCOUNT_DAILY_QUOTA_EXCEEDED",
     "ACCOUNT_SENDING_PAUSED",
     "ACCOUNT_SUSPENDED",
     "ACCOUNT_THROTTLED",
```

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/literals.pyi` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/type_defs.py` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ReviewDetailsTypeDef",
     "TimestampTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
     "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
```

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2/type_defs.pyi` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/PKG-INFO` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sesv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SESV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SESV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/
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
 
 <a id="types-aiobotocore-sesv2"></a>
 
 # types-aiobotocore-sesv2
 
 [![PyPI - types-aiobotocore-sesv2](https://img.shields.io/pypi/v/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sesv2)](https://pepy.tech/project/types-aiobotocore-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SESV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[aiobotocore.SESV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [types-aiobotocore-sesv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sesv2-2.9.0/types_aiobotocore_sesv2.egg-info/SOURCES.txt` & `types-aiobotocore-sesv2-2.9.1/types_aiobotocore_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

