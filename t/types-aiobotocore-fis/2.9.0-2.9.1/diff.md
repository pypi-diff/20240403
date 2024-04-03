# Comparing `tmp/types-aiobotocore-fis-2.9.0.tar.gz` & `tmp/types-aiobotocore-fis-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fis-2.9.0.tar", last modified: Wed Dec 13 19:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-fis-2.9.1.tar", last modified: Thu Jan 18 01:20:44 2024, max compression
```

## Comparing `types-aiobotocore-fis-2.9.0.tar` & `types-aiobotocore-fis-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.781746 types-aiobotocore-fis-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2023-12-13 19:59:19.781746 types-aiobotocore-fis-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:19.781746 types-aiobotocore-fis-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.777746 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19578 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19575 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    29599 2023-12-13 19:46:17.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29598 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:16.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.781746 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2023-12-13 19:59:19.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-13 19:59:19.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:19.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:19.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:19.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:19.000000 types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.205326 types-aiobotocore-fis-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-01-18 01:20:44.205326 types-aiobotocore-fis-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:44.205326 types-aiobotocore-fis-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.201326 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19583 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19580 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29598 2024-01-18 01:08:11.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29598 2024-01-18 01:08:11.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:10.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.205326 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-01-18 01:20:44.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-18 01:20:44.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:44.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:44.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:44.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:44.000000 types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fis-2.9.0/LICENSE` & `types-aiobotocore-fis-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-fis-2.9.0/PKG-INFO` & `types-aiobotocore-fis-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fis
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FIS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FIS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/
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
 
 <a id="types-aiobotocore-fis"></a>
 
 # types-aiobotocore-fis
 
 [![PyPI - types-aiobotocore-fis](https://img.shields.io/pypi/v/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fis)](https://pepy.tech/project/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [types-aiobotocore-fis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fis-2.9.0/README.md` & `types-aiobotocore-fis-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fis)](https://pepy.tech/project/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [types-aiobotocore-fis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fis-2.9.0/setup.py` & `types-aiobotocore-fis-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fis",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_fis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FIS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.FIS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore fis type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_fis": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/__main__.py` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FIS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.FIS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS\nOther"
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

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/client.py` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         description: str,
         stopConditions: Sequence[CreateExperimentTemplateStopConditionInputTypeDef],
         actions: Mapping[str, CreateExperimentTemplateActionInputTypeDef],
         roleArn: str,
         targets: Mapping[str, CreateExperimentTemplateTargetInputTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         logConfiguration: CreateExperimentTemplateLogConfigurationInputTypeDef = ...,
-        experimentOptions: CreateExperimentTemplateExperimentOptionsInputTypeDef = ...
+        experimentOptions: CreateExperimentTemplateExperimentOptionsInputTypeDef = ...,
     ) -> CreateExperimentTemplateResponseTypeDef:
         """
         Creates an experiment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.create_experiment_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#create_experiment_template)
         """
@@ -130,15 +130,15 @@
     async def create_target_account_configuration(
         self,
         *,
         experimentTemplateId: str,
         accountId: str,
         roleArn: str,
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateTargetAccountConfigurationResponseTypeDef:
         """
         Creates a target account configuration for the experiment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.create_target_account_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#create_target_account_configuration)
         """
@@ -246,15 +246,15 @@
 
     async def list_experiment_resolved_targets(
         self,
         *,
         experimentId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        targetName: str = ...
+        targetName: str = ...,
     ) -> ListExperimentResolvedTargetsResponseTypeDef:
         """
         Lists the resolved targets information of the specified experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.list_experiment_resolved_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#list_experiment_resolved_targets)
         """
@@ -361,30 +361,30 @@
         id: str,
         description: str = ...,
         stopConditions: Sequence[UpdateExperimentTemplateStopConditionInputTypeDef] = ...,
         targets: Mapping[str, UpdateExperimentTemplateTargetInputTypeDef] = ...,
         actions: Mapping[str, UpdateExperimentTemplateActionInputItemTypeDef] = ...,
         roleArn: str = ...,
         logConfiguration: UpdateExperimentTemplateLogConfigurationInputTypeDef = ...,
-        experimentOptions: UpdateExperimentTemplateExperimentOptionsInputTypeDef = ...
+        experimentOptions: UpdateExperimentTemplateExperimentOptionsInputTypeDef = ...,
     ) -> UpdateExperimentTemplateResponseTypeDef:
         """
         Updates the specified experiment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.update_experiment_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#update_experiment_template)
         """
 
     async def update_target_account_configuration(
         self,
         *,
         experimentTemplateId: str,
         accountId: str,
         roleArn: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateTargetAccountConfigurationResponseTypeDef:
         """
         Updates the target account configuration for the specified experiment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.update_target_account_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#update_target_account_configuration)
         """
```

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/client.pyi` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         description: str,
         stopConditions: Sequence[CreateExperimentTemplateStopConditionInputTypeDef],
         actions: Mapping[str, CreateExperimentTemplateActionInputTypeDef],
         roleArn: str,
         targets: Mapping[str, CreateExperimentTemplateTargetInputTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         logConfiguration: CreateExperimentTemplateLogConfigurationInputTypeDef = ...,
-        experimentOptions: CreateExperimentTemplateExperimentOptionsInputTypeDef = ...
+        experimentOptions: CreateExperimentTemplateExperimentOptionsInputTypeDef = ...,
     ) -> CreateExperimentTemplateResponseTypeDef:
         """
         Creates an experiment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.create_experiment_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#create_experiment_template)
         """
@@ -127,15 +127,15 @@
     async def create_target_account_configuration(
         self,
         *,
         experimentTemplateId: str,
         accountId: str,
         roleArn: str,
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateTargetAccountConfigurationResponseTypeDef:
         """
         Creates a target account configuration for the experiment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.create_target_account_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#create_target_account_configuration)
         """
@@ -243,15 +243,15 @@
 
     async def list_experiment_resolved_targets(
         self,
         *,
         experimentId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        targetName: str = ...
+        targetName: str = ...,
     ) -> ListExperimentResolvedTargetsResponseTypeDef:
         """
         Lists the resolved targets information of the specified experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.list_experiment_resolved_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#list_experiment_resolved_targets)
         """
@@ -358,30 +358,30 @@
         id: str,
         description: str = ...,
         stopConditions: Sequence[UpdateExperimentTemplateStopConditionInputTypeDef] = ...,
         targets: Mapping[str, UpdateExperimentTemplateTargetInputTypeDef] = ...,
         actions: Mapping[str, UpdateExperimentTemplateActionInputItemTypeDef] = ...,
         roleArn: str = ...,
         logConfiguration: UpdateExperimentTemplateLogConfigurationInputTypeDef = ...,
-        experimentOptions: UpdateExperimentTemplateExperimentOptionsInputTypeDef = ...
+        experimentOptions: UpdateExperimentTemplateExperimentOptionsInputTypeDef = ...,
     ) -> UpdateExperimentTemplateResponseTypeDef:
         """
         Updates the specified experiment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.update_experiment_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#update_experiment_template)
         """
 
     async def update_target_account_configuration(
         self,
         *,
         experimentTemplateId: str,
         accountId: str,
         roleArn: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateTargetAccountConfigurationResponseTypeDef:
         """
         Updates the target account configuration for the specified experiment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.update_target_account_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/client/#update_target_account_configuration)
         """
```

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/literals.py` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountTargetingType",
     "EmptyTargetResolutionModeType",
     "ExperimentActionStatusType",
     "ExperimentStatusType",
     "FISServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 AccountTargetingType = Literal["multi-account", "single-account"]
 EmptyTargetResolutionModeType = Literal["fail", "skip"]
 ExperimentActionStatusType = Literal[
     "cancelled",
     "completed",
     "failed",
     "initiating",
```

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/literals.pyi` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/type_defs.py` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionParameterTypeDef",
     "ActionTargetTypeDef",
     "CreateExperimentTemplateActionInputTypeDef",
     "CreateExperimentTemplateExperimentOptionsInputTypeDef",
     "ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef",
     "ExperimentTemplateS3LogConfigurationInputTypeDef",
```

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis/type_defs.pyi` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/PKG-INFO` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fis
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FIS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FIS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/
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
 
 <a id="types-aiobotocore-fis"></a>
 
 # types-aiobotocore-fis
 
 [![PyPI - types-aiobotocore-fis](https://img.shields.io/pypi/v/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fis)](https://pepy.tech/project/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [types-aiobotocore-fis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fis-2.9.0/types_aiobotocore_fis.egg-info/SOURCES.txt` & `types-aiobotocore-fis-2.9.1/types_aiobotocore_fis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

