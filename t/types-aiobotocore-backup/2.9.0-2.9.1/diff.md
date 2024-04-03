# Comparing `tmp/types-aiobotocore-backup-2.9.0.tar.gz` & `tmp/types-aiobotocore-backup-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backup-2.9.0.tar", last modified: Wed Dec 13 19:58:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-backup-2.9.1.tar", last modified: Thu Jan 18 01:20:07 2024, max compression
```

## Comparing `types-aiobotocore-backup-2.9.0.tar` & `types-aiobotocore-backup-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.226048 types-aiobotocore-backup-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:32.000000 types-aiobotocore-backup-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15794 2023-12-13 19:58:40.226048 types-aiobotocore-backup-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14235 2023-12-13 19:41:32.000000 types-aiobotocore-backup-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:40.226048 types-aiobotocore-backup-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:41:32.000000 types-aiobotocore-backup-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.226048 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74739 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    74735 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14040 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14038 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22853 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22834 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:33.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    83254 2023-12-13 19:41:35.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    83253 2023-12-13 19:41:34.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:32.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.226048 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15794 2023-12-13 19:58:40.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:58:40.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:40.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:40.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:40.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:58:40.000000 types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.837497 types-aiobotocore-backup-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:30.000000 types-aiobotocore-backup-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15814 2024-01-18 01:20:07.837497 types-aiobotocore-backup-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-01-18 01:03:30.000000 types-aiobotocore-backup-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:07.837497 types-aiobotocore-backup-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:03:30.000000 types-aiobotocore-backup-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.837497 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-01-18 01:03:30.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-01-18 01:03:30.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:03:30.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74768 2024-01-18 01:03:31.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74765 2024-01-18 01:03:31.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-01-18 01:03:32.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-01-18 01:03:32.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22859 2024-01-18 01:03:32.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22841 2024-01-18 01:03:32.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:30.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    83253 2024-01-18 01:03:34.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83253 2024-01-18 01:03:33.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:30.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.837497 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15814 2024-01-18 01:20:07.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:20:07.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:07.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:07.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:07.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:20:07.000000 types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backup-2.9.0/LICENSE` & `types-aiobotocore-backup-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-backup-2.9.0/PKG-INFO` & `types-aiobotocore-backup-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Backup 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Backup 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/
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
 
 <a id="types-aiobotocore-backup"></a>
 
 # types-aiobotocore-backup
 
 [![PyPI - types-aiobotocore-backup](https://img.shields.io/pypi/v/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Backup 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[aiobotocore.Backup 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [types-aiobotocore-backup docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backup-2.9.0/README.md` & `types-aiobotocore-backup-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Backup 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[aiobotocore.Backup 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [types-aiobotocore-backup docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backup-2.9.0/setup.py` & `types-aiobotocore-backup-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backup",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Backup 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Backup 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore backup type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_backup": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/__init__.py` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     ListRestoreJobsPaginator,
     ListRestoreTestingPlansPaginator,
     ListRestoreTestingSelectionsPaginator,
 )
 
 Client = BackupClient
 
-
 __all__ = (
     "BackupClient",
     "Client",
     "ListBackupJobsPaginator",
     "ListBackupPlanTemplatesPaginator",
     "ListBackupPlanVersionsPaginator",
     "ListBackupPlansPaginator",
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/__init__.pyi` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/__main__.py` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Backup 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Backup 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
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

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/client.py` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BackupClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -212,29 +211,29 @@
         """
 
     async def create_backup_plan(
         self,
         *,
         BackupPlan: BackupPlanInputTypeDef,
         BackupPlanTags: Mapping[str, str] = ...,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateBackupPlanOutputTypeDef:
         """
         Creates a backup plan using a backup plan name and backup rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_plan)
         """
 
     async def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
         BackupSelection: BackupSelectionTypeDef,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_selection)
@@ -242,15 +241,15 @@
 
     async def create_backup_vault(
         self,
         *,
         BackupVaultName: str,
         BackupVaultTags: Mapping[str, str] = ...,
         EncryptionKeyArn: str = ...,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateBackupVaultOutputTypeDef:
         """
         Creates a logical container where backups are stored.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_vault)
         """
@@ -258,15 +257,15 @@
     async def create_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkControls: Sequence[FrameworkControlTypeDef],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
-        FrameworkTags: Mapping[str, str] = ...
+        FrameworkTags: Mapping[str, str] = ...,
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_framework)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_framework)
         """
@@ -274,15 +273,15 @@
     async def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
         RecoveryPointSelection: RecoveryPointSelectionTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_legal_hold)
         """
@@ -290,15 +289,15 @@
     async def create_logically_air_gapped_backup_vault(
         self,
         *,
         BackupVaultName: str,
         MinRetentionDays: int,
         MaxRetentionDays: int,
         BackupVaultTags: Mapping[str, str] = ...,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateLogicallyAirGappedBackupVaultOutputTypeDef:
         """
         This request creates a logical container to where backups may be copied.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_logically_air_gapped_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_logically_air_gapped_backup_vault)
         """
@@ -307,29 +306,29 @@
         self,
         *,
         ReportPlanName: str,
         ReportDeliveryChannel: ReportDeliveryChannelTypeDef,
         ReportSetting: ReportSettingTypeDef,
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_report_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_report_plan)
         """
 
     async def create_restore_testing_plan(
         self,
         *,
         RestoreTestingPlan: RestoreTestingPlanForCreateTypeDef,
         CreatorRequestId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateRestoreTestingPlanOutputTypeDef:
         """
         This is the first of two steps to create a restore testing plan; once this
         request is successful, finish the procedure with request
         CreateRestoreTestingSelection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_restore_testing_plan)
@@ -337,15 +336,15 @@
         """
 
     async def create_restore_testing_selection(
         self,
         *,
         RestoreTestingPlanName: str,
         RestoreTestingSelection: RestoreTestingSelectionForCreateTypeDef,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateRestoreTestingSelectionOutputTypeDef:
         """
         This request can be sent after CreateRestoreTestingPlan request returns
         successfully.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_restore_testing_selection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_restore_testing_selection)
@@ -745,15 +744,15 @@
         *,
         AccountId: str = ...,
         State: BackupJobStatusType = ...,
         ResourceType: str = ...,
         MessageCategory: str = ...,
         AggregationPeriod: AggregationPeriodType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListBackupJobSummariesOutputTypeDef:
         """
         This is a request for a summary of backup jobs created or running within the
         most recent 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_job_summaries)
@@ -771,15 +770,15 @@
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
-        ByMessageCategory: str = ...
+        ByMessageCategory: str = ...,
     ) -> ListBackupJobsOutputTypeDef:
         """
         Returns a list of existing backup jobs for an authenticated account for the
         last 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_jobs)
@@ -834,15 +833,15 @@
 
     async def list_backup_vaults(
         self,
         *,
         ByVaultType: VaultTypeType = ...,
         ByShared: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListBackupVaultsOutputTypeDef:
         """
         Returns a list of recovery point storage containers along with information
         about
         them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_vaults)
@@ -854,15 +853,15 @@
         *,
         AccountId: str = ...,
         State: CopyJobStatusType = ...,
         ResourceType: str = ...,
         MessageCategory: str = ...,
         AggregationPeriod: AggregationPeriodType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCopyJobSummariesOutputTypeDef:
         """
         This request obtains a list of copy jobs created or running within the the most
         recent 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_copy_job_summaries)
@@ -880,15 +879,15 @@
         ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
-        ByMessageCategory: str = ...
+        ByMessageCategory: str = ...,
     ) -> ListCopyJobsOutputTypeDef:
         """
         Returns metadata about your copy jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_copy_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_copy_jobs)
         """
@@ -930,15 +929,15 @@
 
     async def list_protected_resources_by_backup_vault(
         self,
         *,
         BackupVaultName: str,
         BackupVaultAccountId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProtectedResourcesByBackupVaultOutputTypeDef:
         """
         This request lists the protected resources corresponding to each backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_protected_resources_by_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_protected_resources_by_backup_vault)
         """
@@ -951,15 +950,15 @@
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
-        ByParentRecoveryPointArn: str = ...
+        ByParentRecoveryPointArn: str = ...,
     ) -> ListRecoveryPointsByBackupVaultOutputTypeDef:
         """
         Returns detailed information about the recovery points stored in a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_recovery_points_by_backup_vault)
         """
@@ -992,15 +991,15 @@
         self,
         *,
         ByReportPlanName: str = ...,
         ByCreationBefore: TimestampTypeDef = ...,
         ByCreationAfter: TimestampTypeDef = ...,
         ByStatus: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListReportJobsOutputTypeDef:
         """
         Returns details about your report jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_report_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_report_jobs)
         """
@@ -1019,15 +1018,15 @@
         self,
         *,
         AccountId: str = ...,
         State: RestoreJobStateType = ...,
         ResourceType: str = ...,
         AggregationPeriod: AggregationPeriodType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRestoreJobSummariesOutputTypeDef:
         """
         This request obtains a summary of restore jobs created or running within the
         the most recent 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_job_summaries)
@@ -1042,15 +1041,15 @@
         ByAccountId: str = ...,
         ByResourceType: str = ...,
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
-        ByRestoreTestingPlanArn: str = ...
+        ByRestoreTestingPlanArn: str = ...,
     ) -> ListRestoreJobsOutputTypeDef:
         """
         Returns a list of jobs that Backup initiated to restore a saved resource,
         including details about the recovery
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_jobs)
@@ -1061,15 +1060,15 @@
         self,
         *,
         ResourceArn: str,
         ByStatus: RestoreJobStatusType = ...,
         ByRecoveryPointCreationDateAfter: TimestampTypeDef = ...,
         ByRecoveryPointCreationDateBefore: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRestoreJobsByProtectedResourceOutputTypeDef:
         """
         This returns restore jobs that contain the specified protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_jobs_by_protected_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_restore_jobs_by_protected_resource)
         """
@@ -1120,15 +1119,15 @@
 
     async def put_backup_vault_lock_configuration(
         self,
         *,
         BackupVaultName: str,
         MinRetentionDays: int = ...,
         MaxRetentionDays: int = ...,
-        ChangeableForDays: int = ...
+        ChangeableForDays: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Applies Backup Vault Lock to a backup vault, preventing attempts to delete any
         recovery point stored in or created in a backup
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_lock_configuration)
@@ -1136,29 +1135,29 @@
         """
 
     async def put_backup_vault_notifications(
         self,
         *,
         BackupVaultName: str,
         SNSTopicArn: str,
-        BackupVaultEvents: Sequence[BackupVaultEventType]
+        BackupVaultEvents: Sequence[BackupVaultEventType],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Turns on notifications on a backup vault for the specified topic and events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_notifications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#put_backup_vault_notifications)
         """
 
     async def put_restore_validation_result(
         self,
         *,
         RestoreJobId: str,
         ValidationStatus: RestoreValidationStatusType,
-        ValidationStatusMessage: str = ...
+        ValidationStatusMessage: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This request allows you to send your independent self-run restore test
         validation
         results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_restore_validation_result)
@@ -1172,15 +1171,15 @@
         ResourceArn: str,
         IamRoleArn: str,
         IdempotencyToken: str = ...,
         StartWindowMinutes: int = ...,
         CompleteWindowMinutes: int = ...,
         Lifecycle: LifecycleTypeDef = ...,
         RecoveryPointTags: Mapping[str, str] = ...,
-        BackupOptions: Mapping[str, str] = ...
+        BackupOptions: Mapping[str, str] = ...,
     ) -> StartBackupJobOutputTypeDef:
         """
         Starts an on-demand backup job for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_backup_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#start_backup_job)
         """
@@ -1189,15 +1188,15 @@
         self,
         *,
         RecoveryPointArn: str,
         SourceBackupVaultName: str,
         DestinationBackupVaultArn: str,
         IamRoleArn: str,
         IdempotencyToken: str = ...,
-        Lifecycle: LifecycleTypeDef = ...
+        Lifecycle: LifecycleTypeDef = ...,
     ) -> StartCopyJobOutputTypeDef:
         """
         Starts a job to create a one-time copy of the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_copy_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#start_copy_job)
         """
@@ -1216,15 +1215,15 @@
         self,
         *,
         RecoveryPointArn: str,
         Metadata: Mapping[str, str],
         IamRoleArn: str = ...,
         IdempotencyToken: str = ...,
         ResourceType: str = ...,
-        CopySourceTagsToRestoredResource: bool = ...
+        CopySourceTagsToRestoredResource: bool = ...,
     ) -> StartRestoreJobOutputTypeDef:
         """
         Recovers the saved resource identified by an Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_restore_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#start_restore_job)
         """
@@ -1275,15 +1274,15 @@
 
     async def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
         FrameworkControls: Sequence[FrameworkControlTypeDef] = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON
         format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
@@ -1311,15 +1310,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_recovery_point_lifecycle)
         """
 
     async def update_region_settings(
         self,
         *,
         ResourceTypeOptInPreference: Mapping[str, bool] = ...,
-        ResourceTypeManagementPreference: Mapping[str, bool] = ...
+        ResourceTypeManagementPreference: Mapping[str, bool] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the current service opt-in settings for the Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_region_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_region_settings)
         """
@@ -1327,15 +1326,15 @@
     async def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
         ReportDeliveryChannel: ReportDeliveryChannelTypeDef = ...,
         ReportSetting: ReportSettingTypeDef = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON
         format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
@@ -1353,15 +1352,15 @@
         """
 
     async def update_restore_testing_selection(
         self,
         *,
         RestoreTestingPlanName: str,
         RestoreTestingSelection: RestoreTestingSelectionForUpdateTypeDef,
-        RestoreTestingSelectionName: str
+        RestoreTestingSelectionName: str,
     ) -> UpdateRestoreTestingSelectionOutputTypeDef:
         """
         Most elements except the `RestoreTestingSelectionName` can be updated with this
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_restore_testing_selection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_restore_testing_selection)
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/client.pyi` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -208,29 +208,29 @@
         """
 
     async def create_backup_plan(
         self,
         *,
         BackupPlan: BackupPlanInputTypeDef,
         BackupPlanTags: Mapping[str, str] = ...,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateBackupPlanOutputTypeDef:
         """
         Creates a backup plan using a backup plan name and backup rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_plan)
         """
 
     async def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
         BackupSelection: BackupSelectionTypeDef,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_selection)
@@ -238,15 +238,15 @@
 
     async def create_backup_vault(
         self,
         *,
         BackupVaultName: str,
         BackupVaultTags: Mapping[str, str] = ...,
         EncryptionKeyArn: str = ...,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateBackupVaultOutputTypeDef:
         """
         Creates a logical container where backups are stored.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_vault)
         """
@@ -254,15 +254,15 @@
     async def create_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkControls: Sequence[FrameworkControlTypeDef],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
-        FrameworkTags: Mapping[str, str] = ...
+        FrameworkTags: Mapping[str, str] = ...,
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_framework)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_framework)
         """
@@ -270,15 +270,15 @@
     async def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
         RecoveryPointSelection: RecoveryPointSelectionTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_legal_hold)
         """
@@ -286,15 +286,15 @@
     async def create_logically_air_gapped_backup_vault(
         self,
         *,
         BackupVaultName: str,
         MinRetentionDays: int,
         MaxRetentionDays: int,
         BackupVaultTags: Mapping[str, str] = ...,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateLogicallyAirGappedBackupVaultOutputTypeDef:
         """
         This request creates a logical container to where backups may be copied.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_logically_air_gapped_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_logically_air_gapped_backup_vault)
         """
@@ -303,29 +303,29 @@
         self,
         *,
         ReportPlanName: str,
         ReportDeliveryChannel: ReportDeliveryChannelTypeDef,
         ReportSetting: ReportSettingTypeDef,
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_report_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_report_plan)
         """
 
     async def create_restore_testing_plan(
         self,
         *,
         RestoreTestingPlan: RestoreTestingPlanForCreateTypeDef,
         CreatorRequestId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateRestoreTestingPlanOutputTypeDef:
         """
         This is the first of two steps to create a restore testing plan; once this
         request is successful, finish the procedure with request
         CreateRestoreTestingSelection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_restore_testing_plan)
@@ -333,15 +333,15 @@
         """
 
     async def create_restore_testing_selection(
         self,
         *,
         RestoreTestingPlanName: str,
         RestoreTestingSelection: RestoreTestingSelectionForCreateTypeDef,
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> CreateRestoreTestingSelectionOutputTypeDef:
         """
         This request can be sent after CreateRestoreTestingPlan request returns
         successfully.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_restore_testing_selection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_restore_testing_selection)
@@ -741,15 +741,15 @@
         *,
         AccountId: str = ...,
         State: BackupJobStatusType = ...,
         ResourceType: str = ...,
         MessageCategory: str = ...,
         AggregationPeriod: AggregationPeriodType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListBackupJobSummariesOutputTypeDef:
         """
         This is a request for a summary of backup jobs created or running within the
         most recent 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_job_summaries)
@@ -767,15 +767,15 @@
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
-        ByMessageCategory: str = ...
+        ByMessageCategory: str = ...,
     ) -> ListBackupJobsOutputTypeDef:
         """
         Returns a list of existing backup jobs for an authenticated account for the
         last 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_jobs)
@@ -830,15 +830,15 @@
 
     async def list_backup_vaults(
         self,
         *,
         ByVaultType: VaultTypeType = ...,
         ByShared: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListBackupVaultsOutputTypeDef:
         """
         Returns a list of recovery point storage containers along with information
         about
         them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_vaults)
@@ -850,15 +850,15 @@
         *,
         AccountId: str = ...,
         State: CopyJobStatusType = ...,
         ResourceType: str = ...,
         MessageCategory: str = ...,
         AggregationPeriod: AggregationPeriodType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCopyJobSummariesOutputTypeDef:
         """
         This request obtains a list of copy jobs created or running within the the most
         recent 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_copy_job_summaries)
@@ -876,15 +876,15 @@
         ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
-        ByMessageCategory: str = ...
+        ByMessageCategory: str = ...,
     ) -> ListCopyJobsOutputTypeDef:
         """
         Returns metadata about your copy jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_copy_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_copy_jobs)
         """
@@ -926,15 +926,15 @@
 
     async def list_protected_resources_by_backup_vault(
         self,
         *,
         BackupVaultName: str,
         BackupVaultAccountId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProtectedResourcesByBackupVaultOutputTypeDef:
         """
         This request lists the protected resources corresponding to each backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_protected_resources_by_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_protected_resources_by_backup_vault)
         """
@@ -947,15 +947,15 @@
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
-        ByParentRecoveryPointArn: str = ...
+        ByParentRecoveryPointArn: str = ...,
     ) -> ListRecoveryPointsByBackupVaultOutputTypeDef:
         """
         Returns detailed information about the recovery points stored in a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_recovery_points_by_backup_vault)
         """
@@ -988,15 +988,15 @@
         self,
         *,
         ByReportPlanName: str = ...,
         ByCreationBefore: TimestampTypeDef = ...,
         ByCreationAfter: TimestampTypeDef = ...,
         ByStatus: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListReportJobsOutputTypeDef:
         """
         Returns details about your report jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_report_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_report_jobs)
         """
@@ -1015,15 +1015,15 @@
         self,
         *,
         AccountId: str = ...,
         State: RestoreJobStateType = ...,
         ResourceType: str = ...,
         AggregationPeriod: AggregationPeriodType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRestoreJobSummariesOutputTypeDef:
         """
         This request obtains a summary of restore jobs created or running within the
         the most recent 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_job_summaries)
@@ -1038,15 +1038,15 @@
         ByAccountId: str = ...,
         ByResourceType: str = ...,
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
-        ByRestoreTestingPlanArn: str = ...
+        ByRestoreTestingPlanArn: str = ...,
     ) -> ListRestoreJobsOutputTypeDef:
         """
         Returns a list of jobs that Backup initiated to restore a saved resource,
         including details about the recovery
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_jobs)
@@ -1057,15 +1057,15 @@
         self,
         *,
         ResourceArn: str,
         ByStatus: RestoreJobStatusType = ...,
         ByRecoveryPointCreationDateAfter: TimestampTypeDef = ...,
         ByRecoveryPointCreationDateBefore: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRestoreJobsByProtectedResourceOutputTypeDef:
         """
         This returns restore jobs that contain the specified protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_jobs_by_protected_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_restore_jobs_by_protected_resource)
         """
@@ -1116,15 +1116,15 @@
 
     async def put_backup_vault_lock_configuration(
         self,
         *,
         BackupVaultName: str,
         MinRetentionDays: int = ...,
         MaxRetentionDays: int = ...,
-        ChangeableForDays: int = ...
+        ChangeableForDays: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Applies Backup Vault Lock to a backup vault, preventing attempts to delete any
         recovery point stored in or created in a backup
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_lock_configuration)
@@ -1132,29 +1132,29 @@
         """
 
     async def put_backup_vault_notifications(
         self,
         *,
         BackupVaultName: str,
         SNSTopicArn: str,
-        BackupVaultEvents: Sequence[BackupVaultEventType]
+        BackupVaultEvents: Sequence[BackupVaultEventType],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Turns on notifications on a backup vault for the specified topic and events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_notifications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#put_backup_vault_notifications)
         """
 
     async def put_restore_validation_result(
         self,
         *,
         RestoreJobId: str,
         ValidationStatus: RestoreValidationStatusType,
-        ValidationStatusMessage: str = ...
+        ValidationStatusMessage: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This request allows you to send your independent self-run restore test
         validation
         results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_restore_validation_result)
@@ -1168,15 +1168,15 @@
         ResourceArn: str,
         IamRoleArn: str,
         IdempotencyToken: str = ...,
         StartWindowMinutes: int = ...,
         CompleteWindowMinutes: int = ...,
         Lifecycle: LifecycleTypeDef = ...,
         RecoveryPointTags: Mapping[str, str] = ...,
-        BackupOptions: Mapping[str, str] = ...
+        BackupOptions: Mapping[str, str] = ...,
     ) -> StartBackupJobOutputTypeDef:
         """
         Starts an on-demand backup job for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_backup_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#start_backup_job)
         """
@@ -1185,15 +1185,15 @@
         self,
         *,
         RecoveryPointArn: str,
         SourceBackupVaultName: str,
         DestinationBackupVaultArn: str,
         IamRoleArn: str,
         IdempotencyToken: str = ...,
-        Lifecycle: LifecycleTypeDef = ...
+        Lifecycle: LifecycleTypeDef = ...,
     ) -> StartCopyJobOutputTypeDef:
         """
         Starts a job to create a one-time copy of the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_copy_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#start_copy_job)
         """
@@ -1212,15 +1212,15 @@
         self,
         *,
         RecoveryPointArn: str,
         Metadata: Mapping[str, str],
         IamRoleArn: str = ...,
         IdempotencyToken: str = ...,
         ResourceType: str = ...,
-        CopySourceTagsToRestoredResource: bool = ...
+        CopySourceTagsToRestoredResource: bool = ...,
     ) -> StartRestoreJobOutputTypeDef:
         """
         Recovers the saved resource identified by an Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_restore_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#start_restore_job)
         """
@@ -1271,15 +1271,15 @@
 
     async def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
         FrameworkControls: Sequence[FrameworkControlTypeDef] = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON
         format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
@@ -1307,15 +1307,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_recovery_point_lifecycle)
         """
 
     async def update_region_settings(
         self,
         *,
         ResourceTypeOptInPreference: Mapping[str, bool] = ...,
-        ResourceTypeManagementPreference: Mapping[str, bool] = ...
+        ResourceTypeManagementPreference: Mapping[str, bool] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the current service opt-in settings for the Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_region_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_region_settings)
         """
@@ -1323,15 +1323,15 @@
     async def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
         ReportDeliveryChannel: ReportDeliveryChannelTypeDef = ...,
         ReportSetting: ReportSettingTypeDef = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON
         format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
@@ -1349,15 +1349,15 @@
         """
 
     async def update_restore_testing_selection(
         self,
         *,
         RestoreTestingPlanName: str,
         RestoreTestingSelection: RestoreTestingSelectionForUpdateTypeDef,
-        RestoreTestingSelectionName: str
+        RestoreTestingSelectionName: str,
     ) -> UpdateRestoreTestingSelectionOutputTypeDef:
         """
         Most elements except the `RestoreTestingSelectionName` can be updated with this
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_restore_testing_selection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_restore_testing_selection)
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/literals.py` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/literals.py`

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
     "AggregationPeriodType",
     "BackupJobStateType",
     "BackupJobStatusType",
     "BackupVaultEventType",
     "ConditionTypeType",
     "CopyJobStateType",
@@ -59,15 +58,14 @@
     "BackupServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AggregationPeriodType = Literal["FOURTEEN_DAYS", "ONE_DAY", "SEVEN_DAYS"]
 BackupJobStateType = Literal[
     "ABORTED",
     "ABORTING",
     "COMPLETED",
     "CREATED",
     "EXPIRED",
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/literals.pyi` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/paginator.py` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     "ListRecoveryPointsByResourcePaginator",
     "ListRestoreJobsPaginator",
     "ListRestoreJobsByProtectedResourcePaginator",
     "ListRestoreTestingPlansPaginator",
     "ListRestoreTestingSelectionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -128,15 +127,15 @@
         ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
         ByMessageCategory: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupjobspaginator)
         """
 
 
@@ -207,15 +206,15 @@
     """
 
     def paginate(
         self,
         *,
         ByVaultType: VaultTypeType = ...,
         ByShared: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBackupVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupvaultspaginator)
         """
 
 
@@ -235,15 +234,15 @@
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
         ByMessageCategory: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listcopyjobspaginator)
         """
 
 
@@ -284,15 +283,15 @@
     """
 
     def paginate(
         self,
         *,
         BackupVaultName: str,
         BackupVaultAccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProtectedResourcesByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResourcesByBackupVault.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listprotectedresourcesbybackupvaultpaginator)
         """
 
 
@@ -309,15 +308,15 @@
         BackupVaultAccountId: str = ...,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
 
 
@@ -364,15 +363,15 @@
         ByResourceType: str = ...,
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByRestoreTestingPlanArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrestorejobspaginator)
         """
 
 
@@ -385,15 +384,15 @@
     def paginate(
         self,
         *,
         ResourceArn: str,
         ByStatus: RestoreJobStatusType = ...,
         ByRecoveryPointCreationDateAfter: TimestampTypeDef = ...,
         ByRecoveryPointCreationDateBefore: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRestoreJobsByProtectedResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobsByProtectedResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrestorejobsbyprotectedresourcepaginator)
         """
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/paginator.pyi` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
         ByMessageCategory: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupjobspaginator)
         """
 
 class ListBackupPlanTemplatesPaginator(AioPaginator):
@@ -199,15 +199,15 @@
     """
 
     def paginate(
         self,
         *,
         ByVaultType: VaultTypeType = ...,
         ByShared: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBackupVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupvaultspaginator)
         """
 
 class ListCopyJobsPaginator(AioPaginator):
@@ -226,15 +226,15 @@
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
         ByMessageCategory: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listcopyjobspaginator)
         """
 
 class ListLegalHoldsPaginator(AioPaginator):
@@ -272,15 +272,15 @@
     """
 
     def paginate(
         self,
         *,
         BackupVaultName: str,
         BackupVaultAccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProtectedResourcesByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResourcesByBackupVault.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listprotectedresourcesbybackupvaultpaginator)
         """
 
 class ListRecoveryPointsByBackupVaultPaginator(AioPaginator):
@@ -296,15 +296,15 @@
         BackupVaultAccountId: str = ...,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
 
 class ListRecoveryPointsByLegalHoldPaginator(AioPaginator):
@@ -348,15 +348,15 @@
         ByResourceType: str = ...,
         ByCreatedBefore: TimestampTypeDef = ...,
         ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
         ByCompleteBefore: TimestampTypeDef = ...,
         ByCompleteAfter: TimestampTypeDef = ...,
         ByRestoreTestingPlanArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrestorejobspaginator)
         """
 
 class ListRestoreJobsByProtectedResourcePaginator(AioPaginator):
@@ -368,15 +368,15 @@
     def paginate(
         self,
         *,
         ResourceArn: str,
         ByStatus: RestoreJobStatusType = ...,
         ByRecoveryPointCreationDateAfter: TimestampTypeDef = ...,
         ByRecoveryPointCreationDateBefore: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRestoreJobsByProtectedResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobsByProtectedResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrestorejobsbyprotectedresourcepaginator)
         """
 
 class ListRestoreTestingPlansPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/type_defs.py` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/type_defs.py`

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
     "AdvancedBackupSettingPaginatorTypeDef",
     "AdvancedBackupSettingTypeDef",
     "BackupJobSummaryTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup/type_defs.pyi` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/PKG-INFO` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Backup 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Backup 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/
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
 
 <a id="types-aiobotocore-backup"></a>
 
 # types-aiobotocore-backup
 
 [![PyPI - types-aiobotocore-backup](https://img.shields.io/pypi/v/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Backup 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[aiobotocore.Backup 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [types-aiobotocore-backup docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backup-2.9.0/types_aiobotocore_backup.egg-info/SOURCES.txt` & `types-aiobotocore-backup-2.9.1/types_aiobotocore_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

