# Comparing `tmp/types-aiobotocore-kendra-2.9.0.tar.gz` & `tmp/types-aiobotocore-kendra-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kendra-2.9.0.tar", last modified: Wed Dec 13 19:59:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-kendra-2.9.1.tar", last modified: Thu Jan 18 01:21:01 2024, max compression
```

## Comparing `types-aiobotocore-kendra-2.9.0.tar` & `types-aiobotocore-kendra-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.137587 types-aiobotocore-kendra-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2023-12-13 19:59:38.137587 types-aiobotocore-kendra-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:38.137587 types-aiobotocore-kendra-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.137587 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50876 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    50873 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16027 2023-12-13 19:48:27.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16025 2023-12-13 19:48:27.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    95451 2023-12-13 19:48:28.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    95450 2023-12-13 19:48:28.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:26.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.137587 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.157249 types-aiobotocore-kendra-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-01-18 01:21:01.157249 types-aiobotocore-kendra-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:01.157249 types-aiobotocore-kendra-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.153249 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50902 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50899 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    95450 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95450 2024-01-18 01:10:16.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:15.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.157249 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kendra-2.9.0/LICENSE` & `types-aiobotocore-kendra-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kendra-2.9.0/PKG-INFO` & `types-aiobotocore-kendra-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kendra
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.kendra 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.kendra 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/
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
 
 <a id="types-aiobotocore-kendra"></a>
 
 # types-aiobotocore-kendra
 
 [![PyPI - types-aiobotocore-kendra](https://img.shields.io/pypi/v/types-aiobotocore-kendra.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra)](https://pepy.tech/project/types-aiobotocore-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.kendra 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[aiobotocore.kendra 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [types-aiobotocore-kendra docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kendra-2.9.0/README.md` & `types-aiobotocore-kendra-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra)](https://pepy.tech/project/types-aiobotocore-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.kendra 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[aiobotocore.kendra 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [types-aiobotocore-kendra docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kendra-2.9.0/setup.py` & `types-aiobotocore-kendra-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kendra",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.kendra 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.kendra 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore kendra type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kendra": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/__main__.py` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.kendra 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.kendra 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
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

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/client.py` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         """
 
     async def batch_delete_document(
         self,
         *,
         IndexId: str,
         DocumentIdList: Sequence[str],
-        DataSourceSyncJobMetricTarget: DataSourceSyncJobMetricTargetTypeDef = ...
+        DataSourceSyncJobMetricTarget: DataSourceSyncJobMetricTargetTypeDef = ...,
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Removes one or more documents from an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_delete_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#batch_delete_document)
         """
@@ -220,15 +220,15 @@
 
     async def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...,
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#batch_put_document)
         """
@@ -261,15 +261,15 @@
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
         HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_access_control_configuration)
         """
@@ -284,15 +284,15 @@
         VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_data_source)
@@ -302,15 +302,15 @@
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
         Configuration: ExperienceConfigurationTypeDef = ...,
         Description: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_experience)
         """
@@ -322,15 +322,15 @@
         Name: str,
         S3Path: S3PathTypeDef,
         RoleArn: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FileFormat: FaqFileFormatType = ...,
         ClientToken: str = ...,
-        LanguageCode: str = ...
+        LanguageCode: str = ...,
     ) -> CreateFaqResponseTypeDef:
         """
         Creates a set of frequently ask questions (FAQs) using a specified FAQ file
         stored in an Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_faq)
@@ -343,15 +343,15 @@
         IndexId: str,
         FeaturedResultsSetName: str,
         Description: str = ...,
         ClientToken: str = ...,
         Status: FeaturedResultsSetStatusType = ...,
         QueryTexts: Sequence[str] = ...,
         FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFeaturedResultsSetResponseTypeDef:
         """
         Creates a set of featured results to display at the top of the search results
         page.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_featured_results_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_featured_results_set)
@@ -365,15 +365,15 @@
         Edition: IndexEditionType = ...,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         Description: str = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
-        UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
+        UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...,
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_index)
         """
@@ -383,15 +383,15 @@
         *,
         IndexId: str,
         Name: str,
         SourceS3Path: S3PathTypeDef,
         RoleArn: str,
         Description: str = ...,
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateQuerySuggestionsBlockListResponseTypeDef:
         """
         Creates a block list to exlcude certain queries from suggestions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_query_suggestions_block_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_query_suggestions_block_list)
         """
@@ -401,15 +401,15 @@
         *,
         IndexId: str,
         Name: str,
         RoleArn: str,
         SourceS3Path: S3PathTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateThesaurusResponseTypeDef:
         """
         Creates a thesaurus for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_thesaurus)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_thesaurus)
         """
@@ -628,15 +628,15 @@
     async def get_query_suggestions(
         self,
         *,
         IndexId: str,
         QueryText: str,
         MaxSuggestionsCount: int = ...,
         SuggestionTypes: Sequence[SuggestionTypeType] = ...,
-        AttributeSuggestionsConfig: AttributeSuggestionsGetConfigTypeDef = ...
+        AttributeSuggestionsConfig: AttributeSuggestionsGetConfigTypeDef = ...,
     ) -> GetQuerySuggestionsResponseTypeDef:
         """
         Fetches the queries that are suggested to your users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.get_query_suggestions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#get_query_suggestions)
         """
@@ -644,15 +644,15 @@
     async def get_snapshots(
         self,
         *,
         IndexId: str,
         Interval: IntervalType,
         MetricType: MetricTypeType,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetSnapshotsResponseTypeDef:
         """
         Retrieves search metrics data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.get_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#get_snapshots)
         """
@@ -671,15 +671,15 @@
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         StartTimeFilter: TimeRangeTypeDef = ...,
-        StatusFilter: DataSourceSyncJobStatusType = ...
+        StatusFilter: DataSourceSyncJobStatusType = ...,
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#list_data_source_sync_jobs)
         """
@@ -751,15 +751,15 @@
     async def list_groups_older_than_ordering_id(
         self,
         *,
         IndexId: str,
         OrderingId: int,
         DataSourceId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListGroupsOlderThanOrderingIdResponseTypeDef:
         """
         Provides a list of groups that are mapped to users before a given ordering or
         timestamp
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_groups_older_than_ordering_id)
@@ -810,15 +810,15 @@
         self,
         *,
         IndexId: str,
         GroupId: str,
         GroupMembers: GroupMembersTypeDef,
         DataSourceId: str = ...,
         OrderingId: int = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Maps users to their groups so that you only need to provide the user ID when
         you issue the
         query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.put_principal_mapping)
@@ -840,15 +840,15 @@
         PageNumber: int = ...,
         PageSize: int = ...,
         SortingConfiguration: SortingConfigurationTypeDef = ...,
         SortingConfigurations: Sequence[SortingConfigurationTypeDef] = ...,
         UserContext: UserContextTypeDef = ...,
         VisitorId: str = ...,
         SpellCorrectionConfiguration: SpellCorrectionConfigurationTypeDef = ...,
-        CollapseConfiguration: CollapseConfigurationTypeDef = ...
+        CollapseConfiguration: CollapseConfigurationTypeDef = ...,
     ) -> QueryResultTypeDef:
         """
         Searches an index given an input query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#query)
         """
@@ -861,15 +861,15 @@
         AttributeFilter: "AttributeFilterTypeDef" = ...,
         RequestedDocumentAttributes: Sequence[str] = ...,
         DocumentRelevanceOverrideConfigurations: Sequence[
             DocumentRelevanceConfigurationTypeDef
         ] = ...,
         PageNumber: int = ...,
         PageSize: int = ...,
-        UserContext: UserContextTypeDef = ...
+        UserContext: UserContextTypeDef = ...,
     ) -> RetrieveResultTypeDef:
         """
         Retrieves relevant passages or text excerpts given an input query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.retrieve)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#retrieve)
         """
@@ -896,15 +896,15 @@
 
     async def submit_feedback(
         self,
         *,
         IndexId: str,
         QueryId: str,
         ClickFeedbackItems: Sequence[ClickFeedbackTypeDef] = ...,
-        RelevanceFeedbackItems: Sequence[RelevanceFeedbackTypeDef] = ...
+        RelevanceFeedbackItems: Sequence[RelevanceFeedbackTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables you to provide feedback to Amazon Kendra to improve the performance of
         your
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.submit_feedback)
@@ -931,15 +931,15 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_access_control_configuration)
         """
@@ -952,15 +952,15 @@
         Name: str = ...,
         Configuration: DataSourceConfigurationTypeDef = ...,
         VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_data_source)
         """
@@ -969,15 +969,15 @@
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
         Configuration: ExperienceConfigurationTypeDef = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_experience)
         """
@@ -987,15 +987,15 @@
         *,
         IndexId: str,
         FeaturedResultsSetId: str,
         FeaturedResultsSetName: str = ...,
         Description: str = ...,
         Status: FeaturedResultsSetStatusType = ...,
         QueryTexts: Sequence[str] = ...,
-        FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...
+        FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...,
     ) -> UpdateFeaturedResultsSetResponseTypeDef:
         """
         Updates a set of featured results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_featured_results_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_featured_results_set)
         """
@@ -1007,15 +1007,15 @@
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
         DocumentMetadataConfigurationUpdates: Sequence[DocumentMetadataConfigurationTypeDef] = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
-        UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
+        UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_index)
         """
@@ -1024,15 +1024,15 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         SourceS3Path: S3PathTypeDef = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a block list used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_query_suggestions_block_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_query_suggestions_block_list)
         """
@@ -1042,15 +1042,15 @@
         *,
         IndexId: str,
         Mode: ModeType = ...,
         QueryLogLookBackWindowInDays: int = ...,
         IncludeQueriesWithoutUserInformation: bool = ...,
         MinimumNumberOfQueryingUsers: int = ...,
         MinimumQueryCount: int = ...,
-        AttributeSuggestionsConfig: AttributeSuggestionsUpdateConfigTypeDef = ...
+        AttributeSuggestionsConfig: AttributeSuggestionsUpdateConfigTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_query_suggestions_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_query_suggestions_config)
         """
@@ -1059,15 +1059,15 @@
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         Description: str = ...,
         RoleArn: str = ...,
-        SourceS3Path: S3PathTypeDef = ...
+        SourceS3Path: S3PathTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a thesaurus for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_thesaurus)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_thesaurus)
         """
```

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/client.pyi` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         """
 
     async def batch_delete_document(
         self,
         *,
         IndexId: str,
         DocumentIdList: Sequence[str],
-        DataSourceSyncJobMetricTarget: DataSourceSyncJobMetricTargetTypeDef = ...
+        DataSourceSyncJobMetricTarget: DataSourceSyncJobMetricTargetTypeDef = ...,
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Removes one or more documents from an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_delete_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#batch_delete_document)
         """
@@ -217,15 +217,15 @@
 
     async def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...,
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#batch_put_document)
         """
@@ -258,15 +258,15 @@
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
         HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_access_control_configuration)
         """
@@ -281,15 +281,15 @@
         VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_data_source)
@@ -299,15 +299,15 @@
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
         Configuration: ExperienceConfigurationTypeDef = ...,
         Description: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_experience)
         """
@@ -319,15 +319,15 @@
         Name: str,
         S3Path: S3PathTypeDef,
         RoleArn: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FileFormat: FaqFileFormatType = ...,
         ClientToken: str = ...,
-        LanguageCode: str = ...
+        LanguageCode: str = ...,
     ) -> CreateFaqResponseTypeDef:
         """
         Creates a set of frequently ask questions (FAQs) using a specified FAQ file
         stored in an Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_faq)
@@ -340,15 +340,15 @@
         IndexId: str,
         FeaturedResultsSetName: str,
         Description: str = ...,
         ClientToken: str = ...,
         Status: FeaturedResultsSetStatusType = ...,
         QueryTexts: Sequence[str] = ...,
         FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFeaturedResultsSetResponseTypeDef:
         """
         Creates a set of featured results to display at the top of the search results
         page.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_featured_results_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_featured_results_set)
@@ -362,15 +362,15 @@
         Edition: IndexEditionType = ...,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         Description: str = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
-        UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
+        UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...,
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_index)
         """
@@ -380,15 +380,15 @@
         *,
         IndexId: str,
         Name: str,
         SourceS3Path: S3PathTypeDef,
         RoleArn: str,
         Description: str = ...,
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateQuerySuggestionsBlockListResponseTypeDef:
         """
         Creates a block list to exlcude certain queries from suggestions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_query_suggestions_block_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_query_suggestions_block_list)
         """
@@ -398,15 +398,15 @@
         *,
         IndexId: str,
         Name: str,
         RoleArn: str,
         SourceS3Path: S3PathTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateThesaurusResponseTypeDef:
         """
         Creates a thesaurus for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_thesaurus)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_thesaurus)
         """
@@ -625,15 +625,15 @@
     async def get_query_suggestions(
         self,
         *,
         IndexId: str,
         QueryText: str,
         MaxSuggestionsCount: int = ...,
         SuggestionTypes: Sequence[SuggestionTypeType] = ...,
-        AttributeSuggestionsConfig: AttributeSuggestionsGetConfigTypeDef = ...
+        AttributeSuggestionsConfig: AttributeSuggestionsGetConfigTypeDef = ...,
     ) -> GetQuerySuggestionsResponseTypeDef:
         """
         Fetches the queries that are suggested to your users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.get_query_suggestions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#get_query_suggestions)
         """
@@ -641,15 +641,15 @@
     async def get_snapshots(
         self,
         *,
         IndexId: str,
         Interval: IntervalType,
         MetricType: MetricTypeType,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetSnapshotsResponseTypeDef:
         """
         Retrieves search metrics data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.get_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#get_snapshots)
         """
@@ -668,15 +668,15 @@
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         StartTimeFilter: TimeRangeTypeDef = ...,
-        StatusFilter: DataSourceSyncJobStatusType = ...
+        StatusFilter: DataSourceSyncJobStatusType = ...,
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#list_data_source_sync_jobs)
         """
@@ -748,15 +748,15 @@
     async def list_groups_older_than_ordering_id(
         self,
         *,
         IndexId: str,
         OrderingId: int,
         DataSourceId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListGroupsOlderThanOrderingIdResponseTypeDef:
         """
         Provides a list of groups that are mapped to users before a given ordering or
         timestamp
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_groups_older_than_ordering_id)
@@ -807,15 +807,15 @@
         self,
         *,
         IndexId: str,
         GroupId: str,
         GroupMembers: GroupMembersTypeDef,
         DataSourceId: str = ...,
         OrderingId: int = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Maps users to their groups so that you only need to provide the user ID when
         you issue the
         query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.put_principal_mapping)
@@ -837,15 +837,15 @@
         PageNumber: int = ...,
         PageSize: int = ...,
         SortingConfiguration: SortingConfigurationTypeDef = ...,
         SortingConfigurations: Sequence[SortingConfigurationTypeDef] = ...,
         UserContext: UserContextTypeDef = ...,
         VisitorId: str = ...,
         SpellCorrectionConfiguration: SpellCorrectionConfigurationTypeDef = ...,
-        CollapseConfiguration: CollapseConfigurationTypeDef = ...
+        CollapseConfiguration: CollapseConfigurationTypeDef = ...,
     ) -> QueryResultTypeDef:
         """
         Searches an index given an input query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#query)
         """
@@ -858,15 +858,15 @@
         AttributeFilter: "AttributeFilterTypeDef" = ...,
         RequestedDocumentAttributes: Sequence[str] = ...,
         DocumentRelevanceOverrideConfigurations: Sequence[
             DocumentRelevanceConfigurationTypeDef
         ] = ...,
         PageNumber: int = ...,
         PageSize: int = ...,
-        UserContext: UserContextTypeDef = ...
+        UserContext: UserContextTypeDef = ...,
     ) -> RetrieveResultTypeDef:
         """
         Retrieves relevant passages or text excerpts given an input query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.retrieve)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#retrieve)
         """
@@ -893,15 +893,15 @@
 
     async def submit_feedback(
         self,
         *,
         IndexId: str,
         QueryId: str,
         ClickFeedbackItems: Sequence[ClickFeedbackTypeDef] = ...,
-        RelevanceFeedbackItems: Sequence[RelevanceFeedbackTypeDef] = ...
+        RelevanceFeedbackItems: Sequence[RelevanceFeedbackTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables you to provide feedback to Amazon Kendra to improve the performance of
         your
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.submit_feedback)
@@ -928,15 +928,15 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_access_control_configuration)
         """
@@ -949,15 +949,15 @@
         Name: str = ...,
         Configuration: DataSourceConfigurationTypeDef = ...,
         VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_data_source)
         """
@@ -966,15 +966,15 @@
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
         Configuration: ExperienceConfigurationTypeDef = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_experience)
         """
@@ -984,15 +984,15 @@
         *,
         IndexId: str,
         FeaturedResultsSetId: str,
         FeaturedResultsSetName: str = ...,
         Description: str = ...,
         Status: FeaturedResultsSetStatusType = ...,
         QueryTexts: Sequence[str] = ...,
-        FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...
+        FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...,
     ) -> UpdateFeaturedResultsSetResponseTypeDef:
         """
         Updates a set of featured results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_featured_results_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_featured_results_set)
         """
@@ -1004,15 +1004,15 @@
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
         DocumentMetadataConfigurationUpdates: Sequence[DocumentMetadataConfigurationTypeDef] = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
-        UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
+        UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_index)
         """
@@ -1021,15 +1021,15 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         SourceS3Path: S3PathTypeDef = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a block list used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_query_suggestions_block_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_query_suggestions_block_list)
         """
@@ -1039,15 +1039,15 @@
         *,
         IndexId: str,
         Mode: ModeType = ...,
         QueryLogLookBackWindowInDays: int = ...,
         IncludeQueriesWithoutUserInformation: bool = ...,
         MinimumNumberOfQueryingUsers: int = ...,
         MinimumQueryCount: int = ...,
-        AttributeSuggestionsConfig: AttributeSuggestionsUpdateConfigTypeDef = ...
+        AttributeSuggestionsConfig: AttributeSuggestionsUpdateConfigTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_query_suggestions_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_query_suggestions_config)
         """
@@ -1056,15 +1056,15 @@
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         Description: str = ...,
         RoleArn: str = ...,
-        SourceS3Path: S3PathTypeDef = ...
+        SourceS3Path: S3PathTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a thesaurus for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_thesaurus)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_thesaurus)
         """
```

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/literals.py` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/literals.py`

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
     "AdditionalResultAttributeValueTypeType",
     "AlfrescoEntityType",
     "AttributeSuggestionsModeType",
     "ConditionOperatorType",
     "ConfluenceAttachmentFieldNameType",
     "ConfluenceAuthenticationTypeType",
@@ -85,15 +84,14 @@
     "WebCrawlerModeType",
     "kendraServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AdditionalResultAttributeValueTypeType = Literal["TEXT_WITH_HIGHLIGHTS_VALUE"]
 AlfrescoEntityType = Literal["blog", "documentLibrary", "wiki"]
 AttributeSuggestionsModeType = Literal["ACTIVE", "INACTIVE"]
 ConditionOperatorType = Literal[
     "BeginsWith",
     "Contains",
     "Equals",
```

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/literals.pyi` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/type_defs.py` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessControlConfigurationSummaryTypeDef",
     "AccessControlListConfigurationTypeDef",
     "AclConfigurationTypeDef",
     "DataSourceToIndexFieldMappingTypeDef",
     "DataSourceVpcConfigurationTypeDef",
     "S3PathTypeDef",
```

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra/type_defs.pyi` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/PKG-INFO` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kendra
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.kendra 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.kendra 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/
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
 
 <a id="types-aiobotocore-kendra"></a>
 
 # types-aiobotocore-kendra
 
 [![PyPI - types-aiobotocore-kendra](https://img.shields.io/pypi/v/types-aiobotocore-kendra.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra)](https://pepy.tech/project/types-aiobotocore-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.kendra 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[aiobotocore.kendra 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [types-aiobotocore-kendra docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kendra-2.9.0/types_aiobotocore_kendra.egg-info/SOURCES.txt` & `types-aiobotocore-kendra-2.9.1/types_aiobotocore_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

