# Comparing `tmp/types-aiobotocore-apprunner-2.9.0.tar.gz` & `tmp/types-aiobotocore-apprunner-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apprunner-2.9.0.tar", last modified: Wed Dec 13 19:58:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-apprunner-2.9.1.tar", last modified: Thu Jan 18 01:20:04 2024, max compression
```

## Comparing `types-aiobotocore-apprunner-2.9.0.tar` & `types-aiobotocore-apprunner-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.462080 types-aiobotocore-apprunner-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12409 2023-12-13 19:58:36.462080 types-aiobotocore-apprunner-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:36.462080 types-aiobotocore-apprunner-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.462080 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28981 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10786 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    33720 2023-12-13 19:41:13.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33719 2023-12-13 19:41:13.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:12.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.462080 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12409 2023-12-13 19:58:36.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-13 19:58:36.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:36.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:36.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:36.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:58:36.000000 types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.405508 types-aiobotocore-apprunner-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:10.000000 types-aiobotocore-apprunner-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-01-18 01:20:04.405508 types-aiobotocore-apprunner-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-01-18 01:03:10.000000 types-aiobotocore-apprunner-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:04.405508 types-aiobotocore-apprunner-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:03:10.000000 types-aiobotocore-apprunner-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.405508 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-18 01:03:10.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-18 01:03:10.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:03:10.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28995 2024-01-18 01:03:11.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28992 2024-01-18 01:03:11.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-01-18 01:03:11.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-01-18 01:03:11.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:10.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-01-18 01:03:12.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-01-18 01:03:12.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:10.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.405508 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-01-18 01:20:04.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-01-18 01:20:04.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:04.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:04.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:04.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:04.000000 types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apprunner-2.9.0/LICENSE` & `types-aiobotocore-apprunner-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-apprunner-2.9.0/PKG-INFO` & `types-aiobotocore-apprunner-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apprunner
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppRunner 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppRunner 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/
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
 
 <a id="types-aiobotocore-apprunner"></a>
 
 # types-aiobotocore-apprunner
 
 [![PyPI - types-aiobotocore-apprunner](https://img.shields.io/pypi/v/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apprunner)](https://pepy.tech/project/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [types-aiobotocore-apprunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apprunner-2.9.0/README.md` & `types-aiobotocore-apprunner-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apprunner)](https://pepy.tech/project/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [types-aiobotocore-apprunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apprunner-2.9.0/setup.py` & `types-aiobotocore-apprunner-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apprunner",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_apprunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppRunner 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.AppRunner 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore apprunner type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_apprunner": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/__main__.py` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppRunner 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AppRunner 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner\nOther"
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

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/client.py` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,43 +137,43 @@
     async def create_auto_scaling_configuration(
         self,
         *,
         AutoScalingConfigurationName: str,
         MaxConcurrency: int = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAutoScalingConfigurationResponseTypeDef:
         """
         Create an App Runner automatic scaling configuration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_auto_scaling_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_auto_scaling_configuration)
         """
 
     async def create_connection(
         self,
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateConnectionResponseTypeDef:
         """
         Create an App Runner connection resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_connection)
         """
 
     async def create_observability_configuration(
         self,
         *,
         ObservabilityConfigurationName: str,
         TraceConfiguration: TraceConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateObservabilityConfigurationResponseTypeDef:
         """
         Create an App Runner observability configuration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_observability_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_observability_configuration)
         """
@@ -185,45 +185,45 @@
         SourceConfiguration: SourceConfigurationTypeDef,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
-        ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
+        ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Create an App Runner service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_service)
         """
 
     async def create_vpc_connector(
         self,
         *,
         VpcConnectorName: str,
         Subnets: Sequence[str],
         SecurityGroups: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVpcConnectorResponseTypeDef:
         """
         Create an App Runner VPC connector resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_vpc_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_vpc_connector)
         """
 
     async def create_vpc_ingress_connection(
         self,
         *,
         ServiceArn: str,
         VpcIngressConnectionName: str,
         IngressVpcConfiguration: IngressVpcConfigurationTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVpcIngressConnectionResponseTypeDef:
         """
         Create an App Runner VPC Ingress Connection resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_vpc_ingress_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_vpc_ingress_connection)
         """
@@ -373,15 +373,15 @@
 
     async def list_auto_scaling_configurations(
         self,
         *,
         AutoScalingConfigurationName: str = ...,
         LatestOnly: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAutoScalingConfigurationsResponseTypeDef:
         """
         Returns a list of active App Runner automatic scaling configurations in your
         Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.list_auto_scaling_configurations)
@@ -402,15 +402,15 @@
 
     async def list_observability_configurations(
         self,
         *,
         ObservabilityConfigurationName: str = ...,
         LatestOnly: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListObservabilityConfigurationsResponseTypeDef:
         """
         Returns a list of active App Runner observability configurations in your Amazon
         Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.list_observability_configurations)
@@ -470,15 +470,15 @@
         """
 
     async def list_vpc_ingress_connections(
         self,
         *,
         Filter: ListVpcIngressConnectionsFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListVpcIngressConnectionsResponseTypeDef:
         """
         Return a list of App Runner VPC Ingress Connections in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.list_vpc_ingress_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#list_vpc_ingress_connections)
@@ -541,28 +541,28 @@
         *,
         ServiceArn: str,
         SourceConfiguration: SourceConfigurationTypeDef = ...,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
-        ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
+        ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...,
     ) -> UpdateServiceResponseTypeDef:
         """
         Update an App Runner service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.update_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#update_service)
         """
 
     async def update_vpc_ingress_connection(
         self,
         *,
         VpcIngressConnectionArn: str,
-        IngressVpcConfiguration: IngressVpcConfigurationTypeDef
+        IngressVpcConfiguration: IngressVpcConfigurationTypeDef,
     ) -> UpdateVpcIngressConnectionResponseTypeDef:
         """
         Update an existing App Runner VPC Ingress Connection resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.update_vpc_ingress_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#update_vpc_ingress_connection)
         """
```

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/client.pyi` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -134,43 +134,43 @@
     async def create_auto_scaling_configuration(
         self,
         *,
         AutoScalingConfigurationName: str,
         MaxConcurrency: int = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAutoScalingConfigurationResponseTypeDef:
         """
         Create an App Runner automatic scaling configuration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_auto_scaling_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_auto_scaling_configuration)
         """
 
     async def create_connection(
         self,
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateConnectionResponseTypeDef:
         """
         Create an App Runner connection resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_connection)
         """
 
     async def create_observability_configuration(
         self,
         *,
         ObservabilityConfigurationName: str,
         TraceConfiguration: TraceConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateObservabilityConfigurationResponseTypeDef:
         """
         Create an App Runner observability configuration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_observability_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_observability_configuration)
         """
@@ -182,45 +182,45 @@
         SourceConfiguration: SourceConfigurationTypeDef,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
-        ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
+        ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Create an App Runner service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_service)
         """
 
     async def create_vpc_connector(
         self,
         *,
         VpcConnectorName: str,
         Subnets: Sequence[str],
         SecurityGroups: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVpcConnectorResponseTypeDef:
         """
         Create an App Runner VPC connector resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_vpc_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_vpc_connector)
         """
 
     async def create_vpc_ingress_connection(
         self,
         *,
         ServiceArn: str,
         VpcIngressConnectionName: str,
         IngressVpcConfiguration: IngressVpcConfigurationTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVpcIngressConnectionResponseTypeDef:
         """
         Create an App Runner VPC Ingress Connection resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_vpc_ingress_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#create_vpc_ingress_connection)
         """
@@ -370,15 +370,15 @@
 
     async def list_auto_scaling_configurations(
         self,
         *,
         AutoScalingConfigurationName: str = ...,
         LatestOnly: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAutoScalingConfigurationsResponseTypeDef:
         """
         Returns a list of active App Runner automatic scaling configurations in your
         Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.list_auto_scaling_configurations)
@@ -399,15 +399,15 @@
 
     async def list_observability_configurations(
         self,
         *,
         ObservabilityConfigurationName: str = ...,
         LatestOnly: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListObservabilityConfigurationsResponseTypeDef:
         """
         Returns a list of active App Runner observability configurations in your Amazon
         Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.list_observability_configurations)
@@ -467,15 +467,15 @@
         """
 
     async def list_vpc_ingress_connections(
         self,
         *,
         Filter: ListVpcIngressConnectionsFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListVpcIngressConnectionsResponseTypeDef:
         """
         Return a list of App Runner VPC Ingress Connections in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.list_vpc_ingress_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#list_vpc_ingress_connections)
@@ -538,28 +538,28 @@
         *,
         ServiceArn: str,
         SourceConfiguration: SourceConfigurationTypeDef = ...,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
-        ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
+        ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...,
     ) -> UpdateServiceResponseTypeDef:
         """
         Update an App Runner service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.update_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#update_service)
         """
 
     async def update_vpc_ingress_connection(
         self,
         *,
         VpcIngressConnectionArn: str,
-        IngressVpcConfiguration: IngressVpcConfigurationTypeDef
+        IngressVpcConfiguration: IngressVpcConfigurationTypeDef,
     ) -> UpdateVpcIngressConnectionResponseTypeDef:
         """
         Update an existing App Runner VPC Ingress Connection resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.update_vpc_ingress_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/client/#update_vpc_ingress_connection)
         """
```

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/literals.py` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AutoScalingConfigurationStatusType",
     "CertificateValidationRecordStatusType",
     "ConfigurationSourceType",
     "ConnectionStatusType",
     "CustomDomainAssociationStatusType",
     "EgressTypeType",
@@ -42,15 +41,14 @@
     "VpcIngressConnectionStatusType",
     "AppRunnerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AutoScalingConfigurationStatusType = Literal["ACTIVE", "INACTIVE"]
 CertificateValidationRecordStatusType = Literal["FAILED", "PENDING_VALIDATION", "SUCCESS"]
 ConfigurationSourceType = Literal["API", "REPOSITORY"]
 ConnectionStatusType = Literal["AVAILABLE", "DELETED", "ERROR", "PENDING_HANDSHAKE"]
 CustomDomainAssociationStatusType = Literal[
     "ACTIVE",
     "BINDING_CERTIFICATE",
```

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/literals.pyi` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/type_defs.py` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "VpcDNSTargetTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
```

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner/type_defs.pyi` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/PKG-INFO` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apprunner
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppRunner 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppRunner 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/
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
 
 <a id="types-aiobotocore-apprunner"></a>
 
 # types-aiobotocore-apprunner
 
 [![PyPI - types-aiobotocore-apprunner](https://img.shields.io/pypi/v/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apprunner)](https://pepy.tech/project/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [types-aiobotocore-apprunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apprunner-2.9.0/types_aiobotocore_apprunner.egg-info/SOURCES.txt` & `types-aiobotocore-apprunner-2.9.1/types_aiobotocore_apprunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

