# Comparing `tmp/types-aiobotocore-serverlessrepo-2.9.0.tar.gz` & `tmp/types-aiobotocore-serverlessrepo-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-serverlessrepo-2.9.0.tar", last modified: Wed Dec 13 20:00:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-serverlessrepo-2.9.1.tar", last modified: Thu Jan 18 01:21:47 2024, max compression
```

## Comparing `types-aiobotocore-serverlessrepo-2.9.0.tar` & `types-aiobotocore-serverlessrepo-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.129149 types-aiobotocore-serverlessrepo-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13965 2023-12-13 20:00:29.125149 types-aiobotocore-serverlessrepo-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12357 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:29.129149 types-aiobotocore-serverlessrepo-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.125149 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16564 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16560 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-12-13 19:56:16.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15085 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:15.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.125149 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13965 2023-12-13 20:00:29.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:29.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:29.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:29.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:29.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:29.000000 types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:47.673040 types-aiobotocore-serverlessrepo-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-01-18 01:21:47.673040 types-aiobotocore-serverlessrepo-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:47.673040 types-aiobotocore-serverlessrepo-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:47.673040 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:45.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:47.673040 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-01-18 01:21:47.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:47.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:47.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:47.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:47.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:47.000000 types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/LICENSE` & `types-aiobotocore-serverlessrepo-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/PKG-INFO` & `types-aiobotocore-serverlessrepo-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-serverlessrepo
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/
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
 
 <a id="types-aiobotocore-serverlessrepo"></a>
 
 # types-aiobotocore-serverlessrepo
 
 [![PyPI - types-aiobotocore-serverlessrepo](https://img.shields.io/pypi/v/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServerlessApplicationRepository 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[aiobotocore.ServerlessApplicationRepository 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/README.md` & `types-aiobotocore-serverlessrepo-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServerlessApplicationRepository 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[aiobotocore.ServerlessApplicationRepository 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/setup.py` & `types-aiobotocore-serverlessrepo-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-serverlessrepo",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ServerlessApplicationRepository 2.9.0 service generated"
-        " with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ServerlessApplicationRepository 2.9.1 service generated"
+        " with mypy-boto3-builder 7.23.1"
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
     keywords="aiobotocore serverlessrepo type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_serverlessrepo": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/__init__.py` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 
 Client = ServerlessApplicationRepositoryClient
 
-
 __all__ = (
     "Client",
     "ListApplicationDependenciesPaginator",
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
     "ServerlessApplicationRepositoryClient",
 )
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/__init__.pyi` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/client.py` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ServerlessApplicationRepositoryClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -119,15 +118,15 @@
         ReadmeBody: str = ...,
         ReadmeUrl: str = ...,
         SemanticVersion: str = ...,
         SourceCodeArchiveUrl: str = ...,
         SourceCodeUrl: str = ...,
         SpdxLicenseId: str = ...,
         TemplateBody: str = ...,
-        TemplateUrl: str = ...
+        TemplateUrl: str = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application, optionally including an AWS SAM file to create the
         first application version in the same
         call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_application)
@@ -138,15 +137,15 @@
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str,
         SourceCodeArchiveUrl: str = ...,
         SourceCodeUrl: str = ...,
         TemplateBody: str = ...,
-        TemplateUrl: str = ...
+        TemplateUrl: str = ...,
     ) -> CreateApplicationVersionResponseTypeDef:
         """
         Creates an application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_application_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#create_application_version)
         """
@@ -162,15 +161,15 @@
         Description: str = ...,
         NotificationArns: Sequence[str] = ...,
         ParameterOverrides: Sequence[ParameterValueTypeDef] = ...,
         ResourceTypes: Sequence[str] = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         SemanticVersion: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TemplateId: str = ...
+        TemplateId: str = ...,
     ) -> CreateCloudFormationChangeSetResponseTypeDef:
         """
         Creates an AWS CloudFormation change set for the given application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_cloud_formation_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#create_cloud_formation_change_set)
         """
@@ -239,15 +238,15 @@
 
     async def list_application_dependencies(
         self,
         *,
         ApplicationId: str,
         MaxItems: int = ...,
         NextToken: str = ...,
-        SemanticVersion: str = ...
+        SemanticVersion: str = ...,
     ) -> ListApplicationDependenciesResponseTypeDef:
         """
         Retrieves the list of applications nested in the containing application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_application_dependencies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#list_application_dependencies)
         """
@@ -297,15 +296,15 @@
         *,
         ApplicationId: str,
         Author: str = ...,
         Description: str = ...,
         HomePageUrl: str = ...,
         Labels: Sequence[str] = ...,
         ReadmeBody: str = ...,
-        ReadmeUrl: str = ...
+        ReadmeUrl: str = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#update_application)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/client.pyi` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         ReadmeBody: str = ...,
         ReadmeUrl: str = ...,
         SemanticVersion: str = ...,
         SourceCodeArchiveUrl: str = ...,
         SourceCodeUrl: str = ...,
         SpdxLicenseId: str = ...,
         TemplateBody: str = ...,
-        TemplateUrl: str = ...
+        TemplateUrl: str = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application, optionally including an AWS SAM file to create the
         first application version in the same
         call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_application)
@@ -134,15 +134,15 @@
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str,
         SourceCodeArchiveUrl: str = ...,
         SourceCodeUrl: str = ...,
         TemplateBody: str = ...,
-        TemplateUrl: str = ...
+        TemplateUrl: str = ...,
     ) -> CreateApplicationVersionResponseTypeDef:
         """
         Creates an application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_application_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#create_application_version)
         """
@@ -158,15 +158,15 @@
         Description: str = ...,
         NotificationArns: Sequence[str] = ...,
         ParameterOverrides: Sequence[ParameterValueTypeDef] = ...,
         ResourceTypes: Sequence[str] = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         SemanticVersion: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TemplateId: str = ...
+        TemplateId: str = ...,
     ) -> CreateCloudFormationChangeSetResponseTypeDef:
         """
         Creates an AWS CloudFormation change set for the given application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_cloud_formation_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#create_cloud_formation_change_set)
         """
@@ -235,15 +235,15 @@
 
     async def list_application_dependencies(
         self,
         *,
         ApplicationId: str,
         MaxItems: int = ...,
         NextToken: str = ...,
-        SemanticVersion: str = ...
+        SemanticVersion: str = ...,
     ) -> ListApplicationDependenciesResponseTypeDef:
         """
         Retrieves the list of applications nested in the containing application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_application_dependencies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#list_application_dependencies)
         """
@@ -293,15 +293,15 @@
         *,
         ApplicationId: str,
         Author: str = ...,
         Description: str = ...,
         HomePageUrl: str = ...,
         Labels: Sequence[str] = ...,
         ReadmeBody: str = ...,
-        ReadmeUrl: str = ...
+        ReadmeUrl: str = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#update_application)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/literals.py` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CapabilityType",
     "ListApplicationDependenciesPaginatorName",
     "ListApplicationVersionsPaginatorName",
     "ListApplicationsPaginatorName",
     "StatusType",
     "ServerlessApplicationRepositoryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CapabilityType = Literal[
     "CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM", "CAPABILITY_RESOURCE_POLICY"
 ]
 ListApplicationDependenciesPaginatorName = Literal["list_application_dependencies"]
 ListApplicationVersionsPaginatorName = Literal["list_application_versions"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 StatusType = Literal["ACTIVE", "EXPIRED", "PREPARING"]
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/literals.pyi` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/paginator.py` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 __all__ = (
     "ListApplicationDependenciesPaginator",
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -61,15 +60,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationDependenciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationdependenciespaginator)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/paginator.pyi` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationDependenciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/paginators/#listapplicationdependenciespaginator)
         """
 
 class ListApplicationVersionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/type_defs.py` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo/type_defs.pyi` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-serverlessrepo
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/
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
 
 <a id="types-aiobotocore-serverlessrepo"></a>
 
 # types-aiobotocore-serverlessrepo
 
 [![PyPI - types-aiobotocore-serverlessrepo](https://img.shields.io/pypi/v/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServerlessApplicationRepository 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[aiobotocore.ServerlessApplicationRepository 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-serverlessrepo-2.9.0/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt` & `types-aiobotocore-serverlessrepo-2.9.1/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

