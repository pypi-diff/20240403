# Comparing `tmp/types-aiobotocore-migrationhuborchestrator-2.9.0.tar.gz` & `tmp/types-aiobotocore-migrationhuborchestrator-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migrationhuborchestrator-2.9.0.tar", last modified: Wed Dec 13 19:59:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-migrationhuborchestrator-2.9.1.tar", last modified: Thu Jan 18 01:21:19 2024, max compression
```

## Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0.tar` & `types-aiobotocore-migrationhuborchestrator-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:58.345416 types-aiobotocore-migrationhuborchestrator-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14822 2023-12-13 19:59:58.345416 types-aiobotocore-migrationhuborchestrator-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13191 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:58.345416 types-aiobotocore-migrationhuborchestrator-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:58.345416 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27087 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27083 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10556 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9802 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28152 2023-12-13 19:50:35.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28151 2023-12-13 19:50:35.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:34.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:58.345416 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14822 2023-12-13 19:59:58.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-12-13 19:59:58.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:58.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:58.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:58.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-13 19:59:58.000000 types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:19.793165 types-aiobotocore-migrationhuborchestrator-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-01-18 01:21:19.793165 types-aiobotocore-migrationhuborchestrator-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:19.793165 types-aiobotocore-migrationhuborchestrator-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-01-18 01:12:15.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:19.793165 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27093 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27090 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-01-18 01:12:18.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28151 2024-01-18 01:12:19.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28151 2024-01-18 01:12:19.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:16.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:19.793165 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-01-18 01:21:19.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-18 01:21:19.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:19.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:19.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:19.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-18 01:21:19.000000 types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/LICENSE` & `types-aiobotocore-migrationhuborchestrator-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/PKG-INFO` & `types-aiobotocore-migrationhuborchestrator-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhuborchestrator
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MigrationHubOrchestrator 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MigrationHubOrchestrator 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/
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
 
 <a id="types-aiobotocore-migrationhuborchestrator"></a>
 
 # types-aiobotocore-migrationhuborchestrator
 
 [![PyPI - types-aiobotocore-migrationhuborchestrator](https://img.shields.io/pypi/v/types-aiobotocore-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhuborchestrator)](https://pepy.tech/project/types-aiobotocore-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubOrchestrator 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[aiobotocore.MigrationHubOrchestrator 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [types-aiobotocore-migrationhuborchestrator docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/README.md` & `types-aiobotocore-migrationhuborchestrator-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhuborchestrator)](https://pepy.tech/project/types-aiobotocore-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubOrchestrator 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[aiobotocore.MigrationHubOrchestrator 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [types-aiobotocore-migrationhuborchestrator docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/setup.py` & `types-aiobotocore-migrationhuborchestrator-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-migrationhuborchestrator",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_migrationhuborchestrator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MigrationHubOrchestrator 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MigrationHubOrchestrator 2.9.1 service generated with"
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
         "aiobotocore migrationhuborchestrator type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_migrationhuborchestrator": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/__init__.py` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ListWorkflowsPaginator,
     ListWorkflowStepGroupsPaginator,
     ListWorkflowStepsPaginator,
 )
 
 Client = MigrationHubOrchestratorClient
 
-
 __all__ = (
     "Client",
     "ListPluginsPaginator",
     "ListTemplateStepGroupsPaginator",
     "ListTemplateStepsPaginator",
     "ListTemplatesPaginator",
     "ListWorkflowStepGroupsPaginator",
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/__init__.pyi` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/__main__.py` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHubOrchestrator 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MigrationHubOrchestrator 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator\nOther"
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

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/client.py` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MigrationHubOrchestratorClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -125,15 +124,15 @@
         *,
         name: str,
         templateId: str,
         applicationConfigurationId: str,
         inputParameters: Mapping[str, StepInputTypeDef],
         description: str = ...,
         stepTargets: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateMigrationWorkflowResponseTypeDef:
         """
         Create a workflow to orchestrate your migrations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#create_workflow)
         """
@@ -146,15 +145,15 @@
         workflowId: str,
         stepActionType: StepActionTypeType,
         description: str = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
         outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
         previous: Sequence[str] = ...,
-        next: Sequence[str] = ...
+        next: Sequence[str] = ...,
     ) -> CreateWorkflowStepResponseTypeDef:
         """
         Create a step in the migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#create_workflow_step)
         """
@@ -162,15 +161,15 @@
     async def create_workflow_step_group(
         self,
         *,
         workflowId: str,
         name: str,
         description: str = ...,
         next: Sequence[str] = ...,
-        previous: Sequence[str] = ...
+        previous: Sequence[str] = ...,
     ) -> CreateWorkflowStepGroupResponseTypeDef:
         """
         Create a step group in a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#create_workflow_step_group)
         """
@@ -347,15 +346,15 @@
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         templateId: str = ...,
         adsApplicationConfigurationName: str = ...,
         status: MigrationWorkflowStatusEnumType = ...,
-        name: str = ...
+        name: str = ...,
     ) -> ListMigrationWorkflowsResponseTypeDef:
         """
         List the migration workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#list_workflows)
         """
@@ -405,15 +404,15 @@
     async def update_workflow(
         self,
         *,
         id: str,
         name: str = ...,
         description: str = ...,
         inputParameters: Mapping[str, StepInputTypeDef] = ...,
-        stepTargets: Sequence[str] = ...
+        stepTargets: Sequence[str] = ...,
     ) -> UpdateMigrationWorkflowResponseTypeDef:
         """
         Update a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#update_workflow)
         """
@@ -428,15 +427,15 @@
         description: str = ...,
         stepActionType: StepActionTypeType = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
         outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...,
-        status: StepStatusType = ...
+        status: StepStatusType = ...,
     ) -> UpdateWorkflowStepResponseTypeDef:
         """
         Update a step in a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow_step)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#update_workflow_step)
         """
@@ -445,15 +444,15 @@
         self,
         *,
         workflowId: str,
         id: str,
         name: str = ...,
         description: str = ...,
         next: Sequence[str] = ...,
-        previous: Sequence[str] = ...
+        previous: Sequence[str] = ...,
     ) -> UpdateWorkflowStepGroupResponseTypeDef:
         """
         Update the step group in a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow_step_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#update_workflow_step_group)
         """
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/client.pyi` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         *,
         name: str,
         templateId: str,
         applicationConfigurationId: str,
         inputParameters: Mapping[str, StepInputTypeDef],
         description: str = ...,
         stepTargets: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateMigrationWorkflowResponseTypeDef:
         """
         Create a workflow to orchestrate your migrations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#create_workflow)
         """
@@ -142,15 +142,15 @@
         workflowId: str,
         stepActionType: StepActionTypeType,
         description: str = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
         outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
         previous: Sequence[str] = ...,
-        next: Sequence[str] = ...
+        next: Sequence[str] = ...,
     ) -> CreateWorkflowStepResponseTypeDef:
         """
         Create a step in the migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#create_workflow_step)
         """
@@ -158,15 +158,15 @@
     async def create_workflow_step_group(
         self,
         *,
         workflowId: str,
         name: str,
         description: str = ...,
         next: Sequence[str] = ...,
-        previous: Sequence[str] = ...
+        previous: Sequence[str] = ...,
     ) -> CreateWorkflowStepGroupResponseTypeDef:
         """
         Create a step group in a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#create_workflow_step_group)
         """
@@ -343,15 +343,15 @@
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         templateId: str = ...,
         adsApplicationConfigurationName: str = ...,
         status: MigrationWorkflowStatusEnumType = ...,
-        name: str = ...
+        name: str = ...,
     ) -> ListMigrationWorkflowsResponseTypeDef:
         """
         List the migration workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#list_workflows)
         """
@@ -401,15 +401,15 @@
     async def update_workflow(
         self,
         *,
         id: str,
         name: str = ...,
         description: str = ...,
         inputParameters: Mapping[str, StepInputTypeDef] = ...,
-        stepTargets: Sequence[str] = ...
+        stepTargets: Sequence[str] = ...,
     ) -> UpdateMigrationWorkflowResponseTypeDef:
         """
         Update a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#update_workflow)
         """
@@ -424,15 +424,15 @@
         description: str = ...,
         stepActionType: StepActionTypeType = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
         outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...,
-        status: StepStatusType = ...
+        status: StepStatusType = ...,
     ) -> UpdateWorkflowStepResponseTypeDef:
         """
         Update a step in a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow_step)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#update_workflow_step)
         """
@@ -441,15 +441,15 @@
         self,
         *,
         workflowId: str,
         id: str,
         name: str = ...,
         description: str = ...,
         next: Sequence[str] = ...,
-        previous: Sequence[str] = ...
+        previous: Sequence[str] = ...,
     ) -> UpdateWorkflowStepGroupResponseTypeDef:
         """
         Update the step group in a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow_step_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#update_workflow_step_group)
         """
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/literals.py` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/literals.py`

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
     "DataTypeType",
     "ListPluginsPaginatorName",
     "ListTemplateStepGroupsPaginatorName",
     "ListTemplateStepsPaginatorName",
     "ListTemplatesPaginatorName",
     "ListWorkflowStepGroupsPaginatorName",
@@ -41,15 +40,14 @@
     "MigrationHubOrchestratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DataTypeType = Literal["INTEGER", "STRING", "STRINGLIST", "STRINGMAP"]
 ListPluginsPaginatorName = Literal["list_plugins"]
 ListTemplateStepGroupsPaginatorName = Literal["list_template_step_groups"]
 ListTemplateStepsPaginatorName = Literal["list_template_steps"]
 ListTemplatesPaginatorName = Literal["list_templates"]
 ListWorkflowStepGroupsPaginatorName = Literal["list_workflow_step_groups"]
 ListWorkflowStepsPaginatorName = Literal["list_workflow_steps"]
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/literals.pyi` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/paginator.py` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     "ListTemplateStepsPaginator",
     "ListTemplatesPaginator",
     "ListWorkflowStepGroupsPaginator",
     "ListWorkflowStepsPaginator",
     "ListWorkflowsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -170,13 +169,13 @@
     def paginate(
         self,
         *,
         templateId: str = ...,
         adsApplicationConfigurationName: str = ...,
         status: MigrationWorkflowStatusEnumType = ...,
         name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMigrationWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/paginator.pyi` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -161,13 +161,13 @@
     def paginate(
         self,
         *,
         templateId: str = ...,
         adsApplicationConfigurationName: str = ...,
         status: MigrationWorkflowStatusEnumType = ...,
         name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMigrationWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/type_defs.py` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "StepInputTypeDef",
     "ResponseMetadataTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator/type_defs.pyi` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhuborchestrator
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MigrationHubOrchestrator 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MigrationHubOrchestrator 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/
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
 
 <a id="types-aiobotocore-migrationhuborchestrator"></a>
 
 # types-aiobotocore-migrationhuborchestrator
 
 [![PyPI - types-aiobotocore-migrationhuborchestrator](https://img.shields.io/pypi/v/types-aiobotocore-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhuborchestrator)](https://pepy.tech/project/types-aiobotocore-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubOrchestrator 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[aiobotocore.MigrationHubOrchestrator 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [types-aiobotocore-migrationhuborchestrator docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.9.0/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt` & `types-aiobotocore-migrationhuborchestrator-2.9.1/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

