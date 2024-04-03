# Comparing `tmp/types-aiobotocore-inspector-2.9.0.tar.gz` & `tmp/types-aiobotocore-inspector-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-inspector-2.9.0.tar", last modified: Wed Dec 13 19:59:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-inspector-2.9.1.tar", last modified: Thu Jan 18 01:20:52 2024, max compression
```

## Comparing `types-aiobotocore-inspector-2.9.0.tar` & `types-aiobotocore-inspector-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.821683 types-aiobotocore-inspector-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14313 2023-12-13 19:59:28.817683 types-aiobotocore-inspector-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12742 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:28.821683 types-aiobotocore-inspector-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.817683 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34174 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34170 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    32449 2023-12-13 19:47:30.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32448 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:29.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.817683 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14313 2023-12-13 19:59:28.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:59:28.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:28.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:28.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:28.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:28.000000 types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:52.593287 types-aiobotocore-inspector-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-01-18 01:20:52.593287 types-aiobotocore-inspector-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:52.593287 types-aiobotocore-inspector-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:52.589287 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34181 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34178 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    32448 2024-01-18 01:09:21.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32448 2024-01-18 01:09:21.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:20.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:52.589287 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-01-18 01:20:52.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:20:52.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:52.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:52.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:52.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:52.000000 types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-inspector-2.9.0/LICENSE` & `types-aiobotocore-inspector-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-inspector-2.9.0/PKG-INFO` & `types-aiobotocore-inspector-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-inspector
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Inspector 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Inspector 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/
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
 
 <a id="types-aiobotocore-inspector"></a>
 
 # types-aiobotocore-inspector
 
 [![PyPI - types-aiobotocore-inspector](https://img.shields.io/pypi/v/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector)](https://pepy.tech/project/types-aiobotocore-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Inspector 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[aiobotocore.Inspector 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [types-aiobotocore-inspector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-inspector-2.9.0/README.md` & `types-aiobotocore-inspector-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector)](https://pepy.tech/project/types-aiobotocore-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Inspector 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[aiobotocore.Inspector 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [types-aiobotocore-inspector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-inspector-2.9.0/setup.py` & `types-aiobotocore-inspector-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-inspector",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_inspector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Inspector 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Inspector 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore inspector type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_inspector": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/__init__.py` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     ListFindingsPaginator,
     ListRulesPackagesPaginator,
     PreviewAgentsPaginator,
 )
 
 Client = InspectorClient
 
-
 __all__ = (
     "Client",
     "InspectorClient",
     "ListAssessmentRunAgentsPaginator",
     "ListAssessmentRunsPaginator",
     "ListAssessmentTargetsPaginator",
     "ListAssessmentTemplatesPaginator",
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/__init__.pyi` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/__main__.py` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Inspector 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Inspector 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector\nOther"
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

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/client.py` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("InspectorClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -165,15 +164,15 @@
     async def create_assessment_template(
         self,
         *,
         assessmentTargetArn: str,
         assessmentTemplateName: str,
         durationInSeconds: int,
         rulesPackageArns: Sequence[str],
-        userAttributesForFindings: Sequence[AttributeTypeDef] = ...
+        userAttributesForFindings: Sequence[AttributeTypeDef] = ...,
     ) -> CreateAssessmentTemplateResponseTypeDef:
         """
         Creates an assessment template for the assessment target that is specified by
         the ARN of the assessment
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.create_assessment_template)
@@ -336,15 +335,15 @@
         """
 
     async def get_assessment_report(
         self,
         *,
         assessmentRunArn: str,
         reportFileFormat: ReportFileFormatType,
-        reportType: ReportTypeType
+        reportType: ReportTypeType,
     ) -> GetAssessmentReportResponseTypeDef:
         """
         Produces an assessment report that includes detailed and comprehensive results
         of a specified assessment
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.get_assessment_report)
@@ -354,15 +353,15 @@
     async def get_exclusions_preview(
         self,
         *,
         assessmentTemplateArn: str,
         previewToken: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        locale: Literal["EN_US"] = ...
+        locale: Literal["EN_US"] = ...,
     ) -> GetExclusionsPreviewResponseTypeDef:
         """
         Retrieves the exclusions preview (a list of ExclusionPreview objects) specified
         by the preview
         token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.get_exclusions_preview)
@@ -381,15 +380,15 @@
 
     async def list_assessment_run_agents(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentRunAgentsResponseTypeDef:
         """
         Lists the agents of the assessment runs that are specified by the ARNs of the
         assessment
         runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_assessment_run_agents)
@@ -398,15 +397,15 @@
 
     async def list_assessment_runs(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentRunsResponseTypeDef:
         """
         Lists the assessment runs that correspond to the assessment templates that are
         specified by the ARNs of the assessment
         templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_assessment_runs)
@@ -414,30 +413,30 @@
         """
 
     async def list_assessment_targets(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentTargetsResponseTypeDef:
         """
         Lists the ARNs of the assessment targets within this AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_assessment_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/client/#list_assessment_targets)
         """
 
     async def list_assessment_templates(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentTemplatesResponseTypeDef:
         """
         Lists the assessment templates that correspond to the assessment targets that
         are specified by the ARNs of the assessment
         targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_assessment_templates)
@@ -468,15 +467,15 @@
 
     async def list_findings(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings that are generated by the assessment runs that are specified by
         the ARNs of the assessment
         runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_findings)
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/client.pyi` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     async def create_assessment_template(
         self,
         *,
         assessmentTargetArn: str,
         assessmentTemplateName: str,
         durationInSeconds: int,
         rulesPackageArns: Sequence[str],
-        userAttributesForFindings: Sequence[AttributeTypeDef] = ...
+        userAttributesForFindings: Sequence[AttributeTypeDef] = ...,
     ) -> CreateAssessmentTemplateResponseTypeDef:
         """
         Creates an assessment template for the assessment target that is specified by
         the ARN of the assessment
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.create_assessment_template)
@@ -332,15 +332,15 @@
         """
 
     async def get_assessment_report(
         self,
         *,
         assessmentRunArn: str,
         reportFileFormat: ReportFileFormatType,
-        reportType: ReportTypeType
+        reportType: ReportTypeType,
     ) -> GetAssessmentReportResponseTypeDef:
         """
         Produces an assessment report that includes detailed and comprehensive results
         of a specified assessment
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.get_assessment_report)
@@ -350,15 +350,15 @@
     async def get_exclusions_preview(
         self,
         *,
         assessmentTemplateArn: str,
         previewToken: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        locale: Literal["EN_US"] = ...
+        locale: Literal["EN_US"] = ...,
     ) -> GetExclusionsPreviewResponseTypeDef:
         """
         Retrieves the exclusions preview (a list of ExclusionPreview objects) specified
         by the preview
         token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.get_exclusions_preview)
@@ -377,15 +377,15 @@
 
     async def list_assessment_run_agents(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentRunAgentsResponseTypeDef:
         """
         Lists the agents of the assessment runs that are specified by the ARNs of the
         assessment
         runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_assessment_run_agents)
@@ -394,15 +394,15 @@
 
     async def list_assessment_runs(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentRunsResponseTypeDef:
         """
         Lists the assessment runs that correspond to the assessment templates that are
         specified by the ARNs of the assessment
         templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_assessment_runs)
@@ -410,30 +410,30 @@
         """
 
     async def list_assessment_targets(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentTargetsResponseTypeDef:
         """
         Lists the ARNs of the assessment targets within this AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_assessment_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/client/#list_assessment_targets)
         """
 
     async def list_assessment_templates(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentTemplatesResponseTypeDef:
         """
         Lists the assessment templates that correspond to the assessment targets that
         are specified by the ARNs of the assessment
         targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_assessment_templates)
@@ -464,15 +464,15 @@
 
     async def list_findings(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings that are generated by the assessment runs that are specified by
         the ARNs of the assessment
         runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Client.list_findings)
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/literals.py` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/literals.py`

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
     "AgentHealthCodeType",
     "AgentHealthType",
     "AssessmentRunNotificationSnsStatusCodeType",
     "AssessmentRunStateType",
     "AssetTypeType",
     "FailedItemErrorCodeType",
@@ -48,15 +47,14 @@
     "InspectorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AgentHealthCodeType = Literal["IDLE", "RUNNING", "SHUTDOWN", "THROTTLED", "UNHEALTHY", "UNKNOWN"]
 AgentHealthType = Literal["HEALTHY", "UNHEALTHY", "UNKNOWN"]
 AssessmentRunNotificationSnsStatusCodeType = Literal[
     "ACCESS_DENIED", "INTERNAL_ERROR", "SUCCESS", "TOPIC_DOES_NOT_EXIST"
 ]
 AssessmentRunStateType = Literal[
     "CANCELED",
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/literals.pyi` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/paginator.py` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     "ListEventSubscriptionsPaginator",
     "ListExclusionsPaginator",
     "ListFindingsPaginator",
     "ListRulesPackagesPaginator",
     "PreviewAgentsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -90,15 +89,15 @@
     """
 
     def paginate(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssessmentRunAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunagentspaginator)
         """
 
 
@@ -109,15 +108,15 @@
     """
 
     def paginate(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssessmentRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunspaginator)
         """
 
 
@@ -127,15 +126,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssessmentTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttargetspaginator)
         """
 
 
@@ -146,15 +145,15 @@
     """
 
     def paginate(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssessmentTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttemplatespaginator)
         """
 
 
@@ -195,15 +194,15 @@
     """
 
     def paginate(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listfindingspaginator)
         """
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/paginator.pyi` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     """
 
     def paginate(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssessmentRunAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunagentspaginator)
         """
 
 class ListAssessmentRunsPaginator(AioPaginator):
@@ -105,15 +105,15 @@
     """
 
     def paginate(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssessmentRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunspaginator)
         """
 
 class ListAssessmentTargetsPaginator(AioPaginator):
@@ -122,15 +122,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssessmentTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttargetspaginator)
         """
 
 class ListAssessmentTemplatesPaginator(AioPaginator):
@@ -140,15 +140,15 @@
     """
 
     def paginate(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssessmentTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttemplatespaginator)
         """
 
 class ListEventSubscriptionsPaginator(AioPaginator):
@@ -186,15 +186,15 @@
     """
 
     def paginate(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listfindingspaginator)
         """
 
 class ListRulesPackagesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/type_defs.py` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector/type_defs.pyi` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/PKG-INFO` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-inspector
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Inspector 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Inspector 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/
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
 
 <a id="types-aiobotocore-inspector"></a>
 
 # types-aiobotocore-inspector
 
 [![PyPI - types-aiobotocore-inspector](https://img.shields.io/pypi/v/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector)](https://pepy.tech/project/types-aiobotocore-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Inspector 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[aiobotocore.Inspector 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [types-aiobotocore-inspector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-inspector-2.9.0/types_aiobotocore_inspector.egg-info/SOURCES.txt` & `types-aiobotocore-inspector-2.9.1/types_aiobotocore_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

