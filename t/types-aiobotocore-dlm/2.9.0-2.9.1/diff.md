# Comparing `tmp/types-aiobotocore-dlm-2.9.0.tar.gz` & `tmp/types-aiobotocore-dlm-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dlm-2.9.0.tar", last modified: Wed Dec 13 19:59:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-dlm-2.9.1.tar", last modified: Thu Jan 18 01:20:32 2024, max compression
```

## Comparing `types-aiobotocore-dlm-2.9.0.tar` & `types-aiobotocore-dlm-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.201829 types-aiobotocore-dlm-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2023-12-13 19:59:07.201829 types-aiobotocore-dlm-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10502 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:07.201829 types-aiobotocore-dlm-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.201829 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2023-12-13 19:44:12.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13418 2023-12-13 19:44:12.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13417 2023-12-13 19:44:12.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:11.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.201829 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2023-12-13 19:59:07.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-13 19:59:07.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:07.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:07.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:07.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:07.000000 types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.549383 types-aiobotocore-dlm-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-01-18 01:20:32.549383 types-aiobotocore-dlm-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:32.549383 types-aiobotocore-dlm-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:06:05.000000 types-aiobotocore-dlm-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.549383 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-01-18 01:06:07.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:06.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.549383 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-01-18 01:20:32.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-18 01:20:32.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:32.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:32.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:32.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:32.000000 types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dlm-2.9.0/LICENSE` & `types-aiobotocore-dlm-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-dlm-2.9.0/PKG-INFO` & `types-aiobotocore-dlm-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dlm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DLM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DLM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/
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
 
 <a id="types-aiobotocore-dlm"></a>
 
 # types-aiobotocore-dlm
 
 [![PyPI - types-aiobotocore-dlm](https://img.shields.io/pypi/v/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DLM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[aiobotocore.DLM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [types-aiobotocore-dlm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dlm-2.9.0/README.md` & `types-aiobotocore-dlm-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DLM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[aiobotocore.DLM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [types-aiobotocore-dlm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dlm-2.9.0/setup.py` & `types-aiobotocore-dlm-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dlm",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DLM 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.DLM 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore dlm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dlm": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/__main__.py` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DLM 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DLM 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM\nOther"
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

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/client.py` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         Tags: Mapping[str, str] = ...,
         DefaultPolicy: DefaultPolicyTypeValuesType = ...,
         CreateInterval: int = ...,
         RetainInterval: int = ...,
         CopyTags: bool = ...,
         ExtendDeletion: bool = ...,
         CrossRegionCopyTargets: Sequence[CrossRegionCopyTargetTypeDef] = ...,
-        Exclusions: ExclusionsTypeDef = ...
+        Exclusions: ExclusionsTypeDef = ...,
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates an Amazon Data Lifecycle Manager lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#create_lifecycle_policy)
         """
@@ -140,15 +140,15 @@
         self,
         *,
         PolicyIds: Sequence[str] = ...,
         State: GettablePolicyStateValuesType = ...,
         ResourceTypes: Sequence[ResourceTypeValuesType] = ...,
         TargetTags: Sequence[str] = ...,
         TagsToAdd: Sequence[str] = ...,
-        DefaultPolicyType: DefaultPoliciesTypeValuesType = ...
+        DefaultPolicyType: DefaultPoliciesTypeValuesType = ...,
     ) -> GetLifecyclePoliciesResponseTypeDef:
         """
         Gets summary information about all or the specified data lifecycle policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.get_lifecycle_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#get_lifecycle_policies)
         """
@@ -196,15 +196,15 @@
         Description: str = ...,
         PolicyDetails: PolicyDetailsTypeDef = ...,
         CreateInterval: int = ...,
         RetainInterval: int = ...,
         CopyTags: bool = ...,
         ExtendDeletion: bool = ...,
         CrossRegionCopyTargets: Sequence[CrossRegionCopyTargetTypeDef] = ...,
-        Exclusions: ExclusionsTypeDef = ...
+        Exclusions: ExclusionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/client.pyi` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         Tags: Mapping[str, str] = ...,
         DefaultPolicy: DefaultPolicyTypeValuesType = ...,
         CreateInterval: int = ...,
         RetainInterval: int = ...,
         CopyTags: bool = ...,
         ExtendDeletion: bool = ...,
         CrossRegionCopyTargets: Sequence[CrossRegionCopyTargetTypeDef] = ...,
-        Exclusions: ExclusionsTypeDef = ...
+        Exclusions: ExclusionsTypeDef = ...,
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates an Amazon Data Lifecycle Manager lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#create_lifecycle_policy)
         """
@@ -137,15 +137,15 @@
         self,
         *,
         PolicyIds: Sequence[str] = ...,
         State: GettablePolicyStateValuesType = ...,
         ResourceTypes: Sequence[ResourceTypeValuesType] = ...,
         TargetTags: Sequence[str] = ...,
         TagsToAdd: Sequence[str] = ...,
-        DefaultPolicyType: DefaultPoliciesTypeValuesType = ...
+        DefaultPolicyType: DefaultPoliciesTypeValuesType = ...,
     ) -> GetLifecyclePoliciesResponseTypeDef:
         """
         Gets summary information about all or the specified data lifecycle policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.get_lifecycle_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#get_lifecycle_policies)
         """
@@ -193,15 +193,15 @@
         Description: str = ...,
         PolicyDetails: PolicyDetailsTypeDef = ...,
         CreateInterval: int = ...,
         RetainInterval: int = ...,
         CopyTags: bool = ...,
         ExtendDeletion: bool = ...,
         CrossRegionCopyTargets: Sequence[CrossRegionCopyTargetTypeDef] = ...,
-        Exclusions: ExclusionsTypeDef = ...
+        Exclusions: ExclusionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/literals.py` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/literals.py`

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
     "DefaultPoliciesTypeValuesType",
     "DefaultPolicyTypeValuesType",
     "EventSourceValuesType",
     "EventTypeValuesType",
     "ExecutionHandlerServiceValuesType",
     "GettablePolicyStateValuesType",
@@ -38,15 +37,14 @@
     "StageValuesType",
     "DLMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DefaultPoliciesTypeValuesType = Literal["ALL", "INSTANCE", "VOLUME"]
 DefaultPolicyTypeValuesType = Literal["INSTANCE", "VOLUME"]
 EventSourceValuesType = Literal["MANAGED_CWE"]
 EventTypeValuesType = Literal["shareSnapshot"]
 ExecutionHandlerServiceValuesType = Literal["AWS_SYSTEMS_MANAGER"]
 GettablePolicyStateValuesType = Literal["DISABLED", "ENABLED", "ERROR"]
 IntervalUnitValuesType = Literal["HOURS"]
```

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/literals.pyi` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/type_defs.py` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "RetentionArchiveTierTypeDef",
     "CrossRegionCopyTargetTypeDef",
     "ResponseMetadataTypeDef",
     "ScriptTypeDef",
     "CrossRegionCopyRetainRuleTypeDef",
     "EncryptionConfigurationTypeDef",
```

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm/type_defs.pyi` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/PKG-INFO` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dlm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DLM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DLM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/
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
 
 <a id="types-aiobotocore-dlm"></a>
 
 # types-aiobotocore-dlm
 
 [![PyPI - types-aiobotocore-dlm](https://img.shields.io/pypi/v/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DLM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[aiobotocore.DLM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [types-aiobotocore-dlm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dlm-2.9.0/types_aiobotocore_dlm.egg-info/SOURCES.txt` & `types-aiobotocore-dlm-2.9.1/types_aiobotocore_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

