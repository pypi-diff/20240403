# Comparing `tmp/types-aiobotocore-migration-hub-refactor-spaces-2.9.0.tar.gz` & `tmp/types-aiobotocore-migration-hub-refactor-spaces-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migration-hub-refactor-spaces-2.9.0.tar", last modified: Wed Dec 13 19:59:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-migration-hub-refactor-spaces-2.9.1.tar", last modified: Thu Jan 18 01:21:19 2024, max compression
```

## Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0.tar` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:57.597423 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2023-12-13 19:59:57.597423 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:57.597423 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:57.597423 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24651 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24647 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2023-12-13 19:50:33.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2023-12-13 19:50:33.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25286 2023-12-13 19:50:33.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25285 2023-12-13 19:50:33.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:32.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:57.597423 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2023-12-13 19:59:57.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-12-13 19:59:57.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:57.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:57.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:57.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-13 19:59:57.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:19.129168 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-01-18 01:21:19.129168 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:19.129168 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:19.125168 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24657 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24654 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25285 2024-01-18 01:12:15.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25285 2024-01-18 01:12:15.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:14.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:19.129168 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-01-18 01:21:19.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-01-18 01:21:19.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:19.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:19.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:19.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-18 01:21:19.000000 types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/LICENSE` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/PKG-INFO` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migration-hub-refactor-spaces
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/
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
 
 <a id="types-aiobotocore-migration-hub-refactor-spaces"></a>
 
 # types-aiobotocore-migration-hub-refactor-spaces
 
 [![PyPI - types-aiobotocore-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migration-hub-refactor-spaces)](https://pepy.tech/project/types-aiobotocore-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubRefactorSpaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[aiobotocore.MigrationHubRefactorSpaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [types-aiobotocore-migration-hub-refactor-spaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/README.md` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migration-hub-refactor-spaces)](https://pepy.tech/project/types-aiobotocore-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubRefactorSpaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[aiobotocore.MigrationHubRefactorSpaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [types-aiobotocore-migration-hub-refactor-spaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/setup.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,51 +7,50 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-migration-hub-refactor-spaces",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.9.1 service generated with"
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
         "aiobotocore migration-hub-refactor-spaces type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_migration_hub_refactor_spaces": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/__init__.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListEnvironmentVpcsPaginator,
     ListRoutesPaginator,
     ListServicesPaginator,
 )
 
 Client = MigrationHubRefactorSpacesClient
 
-
 __all__ = (
     "Client",
     "ListApplicationsPaginator",
     "ListEnvironmentVpcsPaginator",
     "ListEnvironmentsPaginator",
     "ListRoutesPaginator",
     "ListServicesPaginator",
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/__main__.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
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

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/client.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MigrationHubRefactorSpacesClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -129,15 +128,15 @@
         *,
         EnvironmentIdentifier: str,
         Name: str,
         ProxyType: Literal["API_GATEWAY"],
         VpcId: str,
         ApiGatewayProxy: ApiGatewayProxyInputTypeDef = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_application)
         """
@@ -145,15 +144,15 @@
     async def create_environment(
         self,
         *,
         Name: str,
         NetworkFabricType: NetworkFabricTypeType,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_environment)
         """
@@ -164,15 +163,15 @@
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteType: RouteTypeType,
         ServiceIdentifier: str,
         ClientToken: str = ...,
         DefaultRoute: DefaultRouteInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        UriPathRoute: UriPathRouteInputTypeDef = ...
+        UriPathRoute: UriPathRouteInputTypeDef = ...,
     ) -> CreateRouteResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_route)
         """
@@ -185,15 +184,15 @@
         EnvironmentIdentifier: str,
         Name: str,
         ClientToken: str = ...,
         Description: str = ...,
         LambdaEndpoint: LambdaEndpointInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         UrlEndpoint: UrlEndpointInputTypeDef = ...,
-        VpcId: str = ...
+        VpcId: str = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_service)
         """
@@ -344,15 +343,15 @@
 
     async def list_routes(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRoutesResponseTypeDef:
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces routes within
         an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_routes)
@@ -361,15 +360,15 @@
 
     async def list_services(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListServicesResponseTypeDef:
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces services within
         an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_services)
@@ -414,15 +413,15 @@
 
     async def update_route(
         self,
         *,
         ActivationState: RouteActivationStateType,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        RouteIdentifier: str
+        RouteIdentifier: str,
     ) -> UpdateRouteResponseTypeDef:
         """
         Updates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#update_route)
         """
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/client.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         *,
         EnvironmentIdentifier: str,
         Name: str,
         ProxyType: Literal["API_GATEWAY"],
         VpcId: str,
         ApiGatewayProxy: ApiGatewayProxyInputTypeDef = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_application)
         """
@@ -141,15 +141,15 @@
     async def create_environment(
         self,
         *,
         Name: str,
         NetworkFabricType: NetworkFabricTypeType,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_environment)
         """
@@ -160,15 +160,15 @@
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteType: RouteTypeType,
         ServiceIdentifier: str,
         ClientToken: str = ...,
         DefaultRoute: DefaultRouteInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        UriPathRoute: UriPathRouteInputTypeDef = ...
+        UriPathRoute: UriPathRouteInputTypeDef = ...,
     ) -> CreateRouteResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_route)
         """
@@ -181,15 +181,15 @@
         EnvironmentIdentifier: str,
         Name: str,
         ClientToken: str = ...,
         Description: str = ...,
         LambdaEndpoint: LambdaEndpointInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         UrlEndpoint: UrlEndpointInputTypeDef = ...,
-        VpcId: str = ...
+        VpcId: str = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_service)
         """
@@ -340,15 +340,15 @@
 
     async def list_routes(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRoutesResponseTypeDef:
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces routes within
         an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_routes)
@@ -357,15 +357,15 @@
 
     async def list_services(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListServicesResponseTypeDef:
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces services within
         an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_services)
@@ -410,15 +410,15 @@
 
     async def update_route(
         self,
         *,
         ActivationState: RouteActivationStateType,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        RouteIdentifier: str
+        RouteIdentifier: str,
     ) -> UpdateRouteResponseTypeDef:
         """
         Updates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#update_route)
         """
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/literals.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/literals.py`

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
     "ApiGatewayEndpointTypeType",
     "ApplicationStateType",
     "EnvironmentStateType",
     "ErrorCodeType",
     "ErrorResourceTypeType",
     "HttpMethodType",
@@ -41,15 +40,14 @@
     "ServiceStateType",
     "MigrationHubRefactorSpacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ApiGatewayEndpointTypeType = Literal["PRIVATE", "REGIONAL"]
 ApplicationStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 EnvironmentStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 ErrorCodeType = Literal[
     "INVALID_RESOURCE_STATE",
     "NOT_AUTHORIZED",
     "REQUEST_LIMIT_EXCEEDED",
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/paginator.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListApplicationsPaginator",
     "ListEnvironmentVpcsPaginator",
     "ListEnvironmentsPaginator",
     "ListRoutesPaginator",
     "ListServicesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -114,15 +113,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/paginators/#listroutespaginator)
         """
 
 
@@ -133,13 +132,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/paginators/#listservicespaginator)
         """
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/paginators/#listroutespaginator)
         """
 
 class ListServicesPaginator(AioPaginator):
@@ -126,13 +126,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/paginators/#listservicespaginator)
         """
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApiGatewayProxyConfigTypeDef",
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
     "ResponseMetadataTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migration-hub-refactor-spaces
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/
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
 
 <a id="types-aiobotocore-migration-hub-refactor-spaces"></a>
 
 # types-aiobotocore-migration-hub-refactor-spaces
 
 [![PyPI - types-aiobotocore-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migration-hub-refactor-spaces)](https://pepy.tech/project/types-aiobotocore-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubRefactorSpaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[aiobotocore.MigrationHubRefactorSpaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [types-aiobotocore-migration-hub-refactor-spaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.9.0/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `types-aiobotocore-migration-hub-refactor-spaces-2.9.1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

