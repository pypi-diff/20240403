# Comparing `tmp/types-aiobotocore-auditmanager-2.9.0.tar.gz` & `tmp/types-aiobotocore-auditmanager-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-auditmanager-2.9.0.tar", last modified: Wed Dec 13 19:58:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-auditmanager-2.9.1.tar", last modified: Thu Jan 18 01:20:06 2024, max compression
```

## Comparing `types-aiobotocore-auditmanager-2.9.0.tar` & `types-aiobotocore-auditmanager-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:38.346064 types-aiobotocore-auditmanager-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2023-12-13 19:58:38.346064 types-aiobotocore-auditmanager-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:38.346064 types-aiobotocore-auditmanager-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:38.346064 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45909 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    45906 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53391 2023-12-13 19:41:25.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53390 2023-12-13 19:41:25.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:24.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:38.346064 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2023-12-13 19:58:38.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 19:58:38.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:38.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:38.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:38.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:58:38.000000 types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.149502 types-aiobotocore-auditmanager-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:22.000000 types-aiobotocore-auditmanager-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-01-18 01:20:06.149502 types-aiobotocore-auditmanager-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-01-18 01:03:22.000000 types-aiobotocore-auditmanager-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:06.149502 types-aiobotocore-auditmanager-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:03:22.000000 types-aiobotocore-auditmanager-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.149502 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-18 01:03:22.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-18 01:03:22.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:03:22.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45924 2024-01-18 01:03:23.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45921 2024-01-18 01:03:23.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-01-18 01:03:23.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-01-18 01:03:23.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:22.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53390 2024-01-18 01:03:24.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53390 2024-01-18 01:03:24.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:22.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.149502 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-01-18 01:20:06.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:20:06.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:06.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:06.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:06.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:06.000000 types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/LICENSE` & `types-aiobotocore-auditmanager-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-auditmanager-2.9.0/PKG-INFO` & `types-aiobotocore-auditmanager-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-auditmanager
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AuditManager 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AuditManager 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/
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
 
 <a id="types-aiobotocore-auditmanager"></a>
 
 # types-aiobotocore-auditmanager
 
 [![PyPI - types-aiobotocore-auditmanager](https://img.shields.io/pypi/v/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AuditManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[aiobotocore.AuditManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [types-aiobotocore-auditmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/README.md` & `types-aiobotocore-auditmanager-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AuditManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[aiobotocore.AuditManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [types-aiobotocore-auditmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/setup.py` & `types-aiobotocore-auditmanager-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-auditmanager",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AuditManager 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AuditManager 2.9.1 service generated with"
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
     keywords="aiobotocore auditmanager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_auditmanager": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/__main__.py` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AuditManager 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AuditManager 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
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

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/client.py` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#batch_associate_assessment_report_evidence)
         """
 
     async def batch_create_delegation_by_assessment(
         self,
         *,
         createDelegationRequests: Sequence[CreateDelegationRequestTypeDef],
-        assessmentId: str
+        assessmentId: str,
     ) -> BatchCreateDelegationByAssessmentResponseTypeDef:
         """
         Creates a batch of delegations for an assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.batch_create_delegation_by_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#batch_create_delegation_by_assessment)
         """
@@ -192,15 +192,15 @@
 
     async def batch_import_evidence_to_assessment_control(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
-        manualEvidence: Sequence[ManualEvidenceTypeDef]
+        manualEvidence: Sequence[ManualEvidenceTypeDef],
     ) -> BatchImportEvidenceToAssessmentControlResponseTypeDef:
         """
         Adds one or more pieces of evidence to a control in an Audit Manager assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.batch_import_evidence_to_assessment_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#batch_import_evidence_to_assessment_control)
         """
@@ -226,15 +226,15 @@
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
         scope: ScopeTypeDef,
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.create_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#create_assessment)
         """
@@ -242,15 +242,15 @@
     async def create_assessment_framework(
         self,
         *,
         name: str,
         controlSets: Sequence[CreateAssessmentFrameworkControlSetTypeDef],
         description: str = ...,
         complianceType: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssessmentFrameworkResponseTypeDef:
         """
         Creates a custom framework in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.create_assessment_framework)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#create_assessment_framework)
         """
@@ -270,15 +270,15 @@
         *,
         name: str,
         controlMappingSources: Sequence[CreateControlMappingSourceTypeDef],
         description: str = ...,
         testingInformation: str = ...,
         actionPlanTitle: str = ...,
         actionPlanInstructions: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateControlResponseTypeDef:
         """
         Creates a new custom control in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.create_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#create_control)
         """
@@ -411,15 +411,15 @@
     async def get_change_logs(
         self,
         *,
         assessmentId: str,
         controlSetId: str = ...,
         controlId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetChangeLogsResponseTypeDef:
         """
         Gets a list of changelogs from Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_change_logs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#get_change_logs)
         """
@@ -455,15 +455,15 @@
     async def get_evidence_by_evidence_folder(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         evidenceFolderId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetEvidenceByEvidenceFolderResponseTypeDef:
         """
         Gets all evidence from a specified evidence folder in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_by_evidence_folder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#get_evidence_by_evidence_folder)
         """
@@ -502,15 +502,15 @@
     async def get_evidence_folders_by_assessment_control(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetEvidenceFoldersByAssessmentControlResponseTypeDef:
         """
         Gets a list of evidence folders that are associated with a specified control in
         an Audit Manager
         assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_folders_by_assessment_control)
@@ -565,15 +565,15 @@
 
     async def list_assessment_control_insights_by_control_domain(
         self,
         *,
         controlDomainId: str,
         assessmentId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentControlInsightsByControlDomainResponseTypeDef:
         """
         Lists the latest analytics data for controls within a specific control domain
         and a specific active
         assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.list_assessment_control_insights_by_control_domain)
@@ -722,15 +722,15 @@
 
     async def start_assessment_framework_share(
         self,
         *,
         frameworkId: str,
         destinationAccount: str,
         destinationRegion: str,
-        comment: str = ...
+        comment: str = ...,
     ) -> StartAssessmentFrameworkShareResponseTypeDef:
         """
         Creates a share request for a custom framework in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.start_assessment_framework_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#start_assessment_framework_share)
         """
@@ -755,15 +755,15 @@
         self,
         *,
         assessmentId: str,
         scope: ScopeTypeDef,
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
-        roles: Sequence[RoleTypeDef] = ...
+        roles: Sequence[RoleTypeDef] = ...,
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_assessment)
         """
@@ -771,15 +771,15 @@
     async def update_assessment_control(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
         controlStatus: ControlStatusType = ...,
-        commentBody: str = ...
+        commentBody: str = ...,
     ) -> UpdateAssessmentControlResponseTypeDef:
         """
         Updates a control within an assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_assessment_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_assessment_control)
         """
@@ -797,15 +797,15 @@
     async def update_assessment_framework(
         self,
         *,
         frameworkId: str,
         name: str,
         controlSets: Sequence[UpdateAssessmentFrameworkControlSetTypeDef],
         description: str = ...,
-        complianceType: str = ...
+        complianceType: str = ...,
     ) -> UpdateAssessmentFrameworkResponseTypeDef:
         """
         Updates a custom framework in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_assessment_framework)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_assessment_framework)
         """
@@ -835,15 +835,15 @@
         *,
         controlId: str,
         name: str,
         controlMappingSources: Sequence[ControlMappingSourceTypeDef],
         description: str = ...,
         testingInformation: str = ...,
         actionPlanTitle: str = ...,
-        actionPlanInstructions: str = ...
+        actionPlanInstructions: str = ...,
     ) -> UpdateControlResponseTypeDef:
         """
         Updates a custom control in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_control)
         """
@@ -853,15 +853,15 @@
         *,
         snsTopic: str = ...,
         defaultAssessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         defaultProcessOwners: Sequence[RoleTypeDef] = ...,
         kmsKey: str = ...,
         evidenceFinderEnabled: bool = ...,
         deregistrationPolicy: DeregistrationPolicyTypeDef = ...,
-        defaultExportDestination: DefaultExportDestinationTypeDef = ...
+        defaultExportDestination: DefaultExportDestinationTypeDef = ...,
     ) -> UpdateSettingsResponseTypeDef:
         """
         Updates Audit Manager settings for the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_settings)
         """
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/client.pyi` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#batch_associate_assessment_report_evidence)
         """
 
     async def batch_create_delegation_by_assessment(
         self,
         *,
         createDelegationRequests: Sequence[CreateDelegationRequestTypeDef],
-        assessmentId: str
+        assessmentId: str,
     ) -> BatchCreateDelegationByAssessmentResponseTypeDef:
         """
         Creates a batch of delegations for an assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.batch_create_delegation_by_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#batch_create_delegation_by_assessment)
         """
@@ -189,15 +189,15 @@
 
     async def batch_import_evidence_to_assessment_control(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
-        manualEvidence: Sequence[ManualEvidenceTypeDef]
+        manualEvidence: Sequence[ManualEvidenceTypeDef],
     ) -> BatchImportEvidenceToAssessmentControlResponseTypeDef:
         """
         Adds one or more pieces of evidence to a control in an Audit Manager assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.batch_import_evidence_to_assessment_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#batch_import_evidence_to_assessment_control)
         """
@@ -223,15 +223,15 @@
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
         scope: ScopeTypeDef,
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.create_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#create_assessment)
         """
@@ -239,15 +239,15 @@
     async def create_assessment_framework(
         self,
         *,
         name: str,
         controlSets: Sequence[CreateAssessmentFrameworkControlSetTypeDef],
         description: str = ...,
         complianceType: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssessmentFrameworkResponseTypeDef:
         """
         Creates a custom framework in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.create_assessment_framework)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#create_assessment_framework)
         """
@@ -267,15 +267,15 @@
         *,
         name: str,
         controlMappingSources: Sequence[CreateControlMappingSourceTypeDef],
         description: str = ...,
         testingInformation: str = ...,
         actionPlanTitle: str = ...,
         actionPlanInstructions: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateControlResponseTypeDef:
         """
         Creates a new custom control in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.create_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#create_control)
         """
@@ -408,15 +408,15 @@
     async def get_change_logs(
         self,
         *,
         assessmentId: str,
         controlSetId: str = ...,
         controlId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetChangeLogsResponseTypeDef:
         """
         Gets a list of changelogs from Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_change_logs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#get_change_logs)
         """
@@ -452,15 +452,15 @@
     async def get_evidence_by_evidence_folder(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         evidenceFolderId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetEvidenceByEvidenceFolderResponseTypeDef:
         """
         Gets all evidence from a specified evidence folder in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_by_evidence_folder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#get_evidence_by_evidence_folder)
         """
@@ -499,15 +499,15 @@
     async def get_evidence_folders_by_assessment_control(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetEvidenceFoldersByAssessmentControlResponseTypeDef:
         """
         Gets a list of evidence folders that are associated with a specified control in
         an Audit Manager
         assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_folders_by_assessment_control)
@@ -562,15 +562,15 @@
 
     async def list_assessment_control_insights_by_control_domain(
         self,
         *,
         controlDomainId: str,
         assessmentId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssessmentControlInsightsByControlDomainResponseTypeDef:
         """
         Lists the latest analytics data for controls within a specific control domain
         and a specific active
         assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.list_assessment_control_insights_by_control_domain)
@@ -719,15 +719,15 @@
 
     async def start_assessment_framework_share(
         self,
         *,
         frameworkId: str,
         destinationAccount: str,
         destinationRegion: str,
-        comment: str = ...
+        comment: str = ...,
     ) -> StartAssessmentFrameworkShareResponseTypeDef:
         """
         Creates a share request for a custom framework in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.start_assessment_framework_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#start_assessment_framework_share)
         """
@@ -752,15 +752,15 @@
         self,
         *,
         assessmentId: str,
         scope: ScopeTypeDef,
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
-        roles: Sequence[RoleTypeDef] = ...
+        roles: Sequence[RoleTypeDef] = ...,
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_assessment)
         """
@@ -768,15 +768,15 @@
     async def update_assessment_control(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
         controlStatus: ControlStatusType = ...,
-        commentBody: str = ...
+        commentBody: str = ...,
     ) -> UpdateAssessmentControlResponseTypeDef:
         """
         Updates a control within an assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_assessment_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_assessment_control)
         """
@@ -794,15 +794,15 @@
     async def update_assessment_framework(
         self,
         *,
         frameworkId: str,
         name: str,
         controlSets: Sequence[UpdateAssessmentFrameworkControlSetTypeDef],
         description: str = ...,
-        complianceType: str = ...
+        complianceType: str = ...,
     ) -> UpdateAssessmentFrameworkResponseTypeDef:
         """
         Updates a custom framework in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_assessment_framework)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_assessment_framework)
         """
@@ -832,15 +832,15 @@
         *,
         controlId: str,
         name: str,
         controlMappingSources: Sequence[ControlMappingSourceTypeDef],
         description: str = ...,
         testingInformation: str = ...,
         actionPlanTitle: str = ...,
-        actionPlanInstructions: str = ...
+        actionPlanInstructions: str = ...,
     ) -> UpdateControlResponseTypeDef:
         """
         Updates a custom control in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_control)
         """
@@ -850,15 +850,15 @@
         *,
         snsTopic: str = ...,
         defaultAssessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         defaultProcessOwners: Sequence[RoleTypeDef] = ...,
         kmsKey: str = ...,
         evidenceFinderEnabled: bool = ...,
         deregistrationPolicy: DeregistrationPolicyTypeDef = ...,
-        defaultExportDestination: DefaultExportDestinationTypeDef = ...
+        defaultExportDestination: DefaultExportDestinationTypeDef = ...,
     ) -> UpdateSettingsResponseTypeDef:
         """
         Updates Audit Manager settings for the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#update_settings)
         """
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/literals.py` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/literals.py`

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
     "ActionEnumType",
     "AssessmentReportDestinationTypeType",
     "AssessmentReportStatusType",
     "AssessmentStatusType",
     "ControlResponseType",
@@ -48,15 +47,14 @@
     "SourceTypeType",
     "AuditManagerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AccountStatusType = Literal["ACTIVE", "INACTIVE", "PENDING_ACTIVATION"]
 ActionEnumType = Literal[
     "ACTIVE",
     "CREATE",
     "DELETE",
     "IMPORT_EVIDENCE",
     "INACTIVE",
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/literals.pyi` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/type_defs.py` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AWSAccountTypeDef",
     "AWSServiceTypeDef",
     "DelegationTypeDef",
     "RoleTypeDef",
     "ControlCommentTypeDef",
     "AssessmentEvidenceFolderTypeDef",
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager/type_defs.pyi` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/PKG-INFO` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-auditmanager
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AuditManager 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AuditManager 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/
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
 
 <a id="types-aiobotocore-auditmanager"></a>
 
 # types-aiobotocore-auditmanager
 
 [![PyPI - types-aiobotocore-auditmanager](https://img.shields.io/pypi/v/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AuditManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[aiobotocore.AuditManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [types-aiobotocore-auditmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-auditmanager-2.9.0/types_aiobotocore_auditmanager.egg-info/SOURCES.txt` & `types-aiobotocore-auditmanager-2.9.1/types_aiobotocore_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

