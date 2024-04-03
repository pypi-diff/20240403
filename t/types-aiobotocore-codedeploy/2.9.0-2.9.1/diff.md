# Comparing `tmp/types-aiobotocore-codedeploy-2.9.0.tar.gz` & `tmp/types-aiobotocore-codedeploy-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codedeploy-2.9.0.tar", last modified: Wed Dec 13 19:58:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-codedeploy-2.9.1.tar", last modified: Thu Jan 18 01:20:20 2024, max compression
```

## Comparing `types-aiobotocore-codedeploy-2.9.0.tar` & `types-aiobotocore-codedeploy-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.089936 types-aiobotocore-codedeploy-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15267 2023-12-13 19:58:54.089936 types-aiobotocore-codedeploy-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:54.089936 types-aiobotocore-codedeploy-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.089936 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48778 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48774 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2023-12-13 19:42:52.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2023-12-13 19:42:52.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12618 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    48858 2023-12-13 19:42:53.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    48857 2023-12-13 19:42:53.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-12-13 19:42:51.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.089936 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15267 2023-12-13 19:58:54.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-13 19:58:54.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:54.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:54.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:54.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:54.000000 types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.481442 types-aiobotocore-codedeploy-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:47.000000 types-aiobotocore-codedeploy-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15287 2024-01-18 01:20:20.481442 types-aiobotocore-codedeploy-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-01-18 01:04:47.000000 types-aiobotocore-codedeploy-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:20.481442 types-aiobotocore-codedeploy-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:04:47.000000 types-aiobotocore-codedeploy-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.477442 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-01-18 01:04:47.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-01-18 01:04:47.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:04:47.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48788 2024-01-18 01:04:48.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48785 2024-01-18 01:04:48.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-01-18 01:04:49.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-01-18 01:04:49.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-01-18 01:04:48.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-01-18 01:04:48.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:47.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    48857 2024-01-18 01:04:50.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48857 2024-01-18 01:04:49.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:47.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-01-18 01:04:48.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-01-18 01:04:48.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.481442 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15287 2024-01-18 01:20:20.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-18 01:20:20.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:20.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:20.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:20.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:20.000000 types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/LICENSE` & `types-aiobotocore-codedeploy-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codedeploy-2.9.0/PKG-INFO` & `types-aiobotocore-codedeploy-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codedeploy
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeDeploy 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeDeploy 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/
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
 
 <a id="types-aiobotocore-codedeploy"></a>
 
 # types-aiobotocore-codedeploy
 
 [![PyPI - types-aiobotocore-codedeploy](https://img.shields.io/pypi/v/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [types-aiobotocore-codedeploy docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/README.md` & `types-aiobotocore-codedeploy-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [types-aiobotocore-codedeploy docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/setup.py` & `types-aiobotocore-codedeploy-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codedeploy",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeDeploy 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeDeploy 2.9.1 service generated with"
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
     keywords="aiobotocore codedeploy type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codedeploy": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/__init__.py` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     ListGitHubAccountTokenNamesPaginator,
     ListOnPremisesInstancesPaginator,
 )
 from .waiter import DeploymentSuccessfulWaiter
 
 Client = CodeDeployClient
 
-
 __all__ = (
     "Client",
     "CodeDeployClient",
     "DeploymentSuccessfulWaiter",
     "ListApplicationRevisionsPaginator",
     "ListApplicationsPaginator",
     "ListDeploymentConfigsPaginator",
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/__init__.pyi` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/__main__.py` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeDeploy 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeDeploy 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
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

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/client.py` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 from .waiter import DeploymentSuccessfulWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeDeployClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -365,15 +364,15 @@
         """
 
     async def create_application(
         self,
         *,
         applicationName: str,
         computePlatform: ComputePlatformType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationOutputTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_application)
         """
@@ -387,15 +386,15 @@
         deploymentConfigName: str = ...,
         description: str = ...,
         ignoreApplicationStopFailures: bool = ...,
         targetInstances: TargetInstancesTypeDef = ...,
         autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
         updateOutdatedInstancesOnly: bool = ...,
         fileExistsBehavior: FileExistsBehaviorType = ...,
-        overrideAlarmConfiguration: AlarmConfigurationTypeDef = ...
+        overrideAlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> CreateDeploymentOutputTypeDef:
         """
         Deploys an application revision through the specified deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment)
         """
@@ -403,15 +402,15 @@
     async def create_deployment_config(
         self,
         *,
         deploymentConfigName: str,
         minimumHealthyHosts: MinimumHealthyHostsTypeDef = ...,
         trafficRoutingConfig: TrafficRoutingConfigTypeDef = ...,
         computePlatform: ComputePlatformType = ...,
-        zonalConfig: ZonalConfigTypeDef = ...
+        zonalConfig: ZonalConfigTypeDef = ...,
     ) -> CreateDeploymentConfigOutputTypeDef:
         """
         Creates a deployment configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment_config)
         """
@@ -433,15 +432,15 @@
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
         loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
         ec2TagSet: EC2TagSetTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
         onPremisesTagSet: OnPremisesTagSetTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        terminationHookEnabled: bool = ...
+        terminationHookEnabled: bool = ...,
     ) -> CreateDeploymentGroupOutputTypeDef:
         """
         Creates a deployment group to which application revisions are deployed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment_group)
         """
@@ -597,15 +596,15 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationRevisionsOutputTypeDef:
         """
         Lists information about revisions for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_application_revisions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#list_application_revisions)
         """
@@ -643,29 +642,29 @@
 
     async def list_deployment_instances(
         self,
         *,
         deploymentId: str,
         nextToken: str = ...,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
-        instanceTypeFilter: Sequence[InstanceTypeType] = ...
+        instanceTypeFilter: Sequence[InstanceTypeType] = ...,
     ) -> ListDeploymentInstancesOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_deployment_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#list_deployment_instances)
         """
 
     async def list_deployment_targets(
         self,
         *,
         deploymentId: str,
         nextToken: str = ...,
-        targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...
+        targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
     ) -> ListDeploymentTargetsOutputTypeDef:
         """
         Returns an array of target IDs that are associated a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_deployment_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#list_deployment_targets)
         """
@@ -674,15 +673,15 @@
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsOutputTypeDef:
         """
         Lists the deployments in a deployment group for an application registered with
         the user or Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_deployments)
@@ -700,15 +699,15 @@
         """
 
     async def list_on_premises_instances(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListOnPremisesInstancesOutputTypeDef:
         """
         Gets a list of names for one or more on-premises instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_on_premises_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#list_on_premises_instances)
         """
@@ -726,15 +725,15 @@
         """
 
     async def put_lifecycle_event_hook_execution_status(
         self,
         *,
         deploymentId: str = ...,
         lifecycleEventHookExecutionId: str = ...,
-        status: LifecycleEventStatusType = ...
+        status: LifecycleEventStatusType = ...,
     ) -> PutLifecycleEventHookExecutionStatusOutputTypeDef:
         """
         Sets the result of a Lambda validation function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.put_lifecycle_event_hook_execution_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#put_lifecycle_event_hook_execution_status)
         """
@@ -836,15 +835,15 @@
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
         loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
         ec2TagSet: EC2TagSetTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
         onPremisesTagSet: OnPremisesTagSetTypeDef = ...,
-        terminationHookEnabled: bool = ...
+        terminationHookEnabled: bool = ...,
     ) -> UpdateDeploymentGroupOutputTypeDef:
         """
         Changes information about a deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.update_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#update_deployment_group)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/client.pyi` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -361,15 +361,15 @@
         """
 
     async def create_application(
         self,
         *,
         applicationName: str,
         computePlatform: ComputePlatformType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationOutputTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_application)
         """
@@ -383,15 +383,15 @@
         deploymentConfigName: str = ...,
         description: str = ...,
         ignoreApplicationStopFailures: bool = ...,
         targetInstances: TargetInstancesTypeDef = ...,
         autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
         updateOutdatedInstancesOnly: bool = ...,
         fileExistsBehavior: FileExistsBehaviorType = ...,
-        overrideAlarmConfiguration: AlarmConfigurationTypeDef = ...
+        overrideAlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> CreateDeploymentOutputTypeDef:
         """
         Deploys an application revision through the specified deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment)
         """
@@ -399,15 +399,15 @@
     async def create_deployment_config(
         self,
         *,
         deploymentConfigName: str,
         minimumHealthyHosts: MinimumHealthyHostsTypeDef = ...,
         trafficRoutingConfig: TrafficRoutingConfigTypeDef = ...,
         computePlatform: ComputePlatformType = ...,
-        zonalConfig: ZonalConfigTypeDef = ...
+        zonalConfig: ZonalConfigTypeDef = ...,
     ) -> CreateDeploymentConfigOutputTypeDef:
         """
         Creates a deployment configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment_config)
         """
@@ -429,15 +429,15 @@
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
         loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
         ec2TagSet: EC2TagSetTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
         onPremisesTagSet: OnPremisesTagSetTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        terminationHookEnabled: bool = ...
+        terminationHookEnabled: bool = ...,
     ) -> CreateDeploymentGroupOutputTypeDef:
         """
         Creates a deployment group to which application revisions are deployed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment_group)
         """
@@ -593,15 +593,15 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationRevisionsOutputTypeDef:
         """
         Lists information about revisions for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_application_revisions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#list_application_revisions)
         """
@@ -639,29 +639,29 @@
 
     async def list_deployment_instances(
         self,
         *,
         deploymentId: str,
         nextToken: str = ...,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
-        instanceTypeFilter: Sequence[InstanceTypeType] = ...
+        instanceTypeFilter: Sequence[InstanceTypeType] = ...,
     ) -> ListDeploymentInstancesOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_deployment_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#list_deployment_instances)
         """
 
     async def list_deployment_targets(
         self,
         *,
         deploymentId: str,
         nextToken: str = ...,
-        targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...
+        targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
     ) -> ListDeploymentTargetsOutputTypeDef:
         """
         Returns an array of target IDs that are associated a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_deployment_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#list_deployment_targets)
         """
@@ -670,15 +670,15 @@
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsOutputTypeDef:
         """
         Lists the deployments in a deployment group for an application registered with
         the user or Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_deployments)
@@ -696,15 +696,15 @@
         """
 
     async def list_on_premises_instances(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListOnPremisesInstancesOutputTypeDef:
         """
         Gets a list of names for one or more on-premises instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.list_on_premises_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#list_on_premises_instances)
         """
@@ -722,15 +722,15 @@
         """
 
     async def put_lifecycle_event_hook_execution_status(
         self,
         *,
         deploymentId: str = ...,
         lifecycleEventHookExecutionId: str = ...,
-        status: LifecycleEventStatusType = ...
+        status: LifecycleEventStatusType = ...,
     ) -> PutLifecycleEventHookExecutionStatusOutputTypeDef:
         """
         Sets the result of a Lambda validation function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.put_lifecycle_event_hook_execution_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#put_lifecycle_event_hook_execution_status)
         """
@@ -832,15 +832,15 @@
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
         loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
         ec2TagSet: EC2TagSetTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
         onPremisesTagSet: OnPremisesTagSetTypeDef = ...,
-        terminationHookEnabled: bool = ...
+        terminationHookEnabled: bool = ...,
     ) -> UpdateDeploymentGroupOutputTypeDef:
         """
         Changes information about a deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.update_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#update_deployment_group)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/literals.py` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/literals.py`

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
     "ApplicationRevisionSortByType",
     "AutoRollbackEventType",
     "BundleTypeType",
     "ComputePlatformType",
     "DeploymentCreatorType",
     "DeploymentOptionType",
@@ -69,15 +68,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ApplicationRevisionSortByType = Literal["firstUsedTime", "lastUsedTime", "registerTime"]
 AutoRollbackEventType = Literal[
     "DEPLOYMENT_FAILURE", "DEPLOYMENT_STOP_ON_ALARM", "DEPLOYMENT_STOP_ON_REQUEST"
 ]
 BundleTypeType = Literal["JSON", "YAML", "tar", "tgz", "zip"]
 ComputePlatformType = Literal["ECS", "Lambda", "Server"]
 DeploymentCreatorType = Literal[
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/literals.pyi` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/paginator.py` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     "ListDeploymentInstancesPaginator",
     "ListDeploymentTargetsPaginator",
     "ListDeploymentsPaginator",
     "ListGitHubAccountTokenNamesPaginator",
     "ListOnPremisesInstancesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -101,15 +100,15 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationrevisionspaginator)
         """
 
 
@@ -166,15 +165,15 @@
 
     def paginate(
         self,
         *,
         deploymentId: str,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
         instanceTypeFilter: Sequence[InstanceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentinstancespaginator)
         """
 
 
@@ -185,15 +184,15 @@
     """
 
     def paginate(
         self,
         *,
         deploymentId: str,
         targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymenttargetspaginator)
         """
 
 
@@ -207,15 +206,15 @@
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentspaginator)
         """
 
 
@@ -241,13 +240,13 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOnPremisesInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listonpremisesinstancespaginator)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/paginator.pyi` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationrevisionspaginator)
         """
 
 class ListApplicationsPaginator(AioPaginator):
@@ -159,15 +159,15 @@
 
     def paginate(
         self,
         *,
         deploymentId: str,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
         instanceTypeFilter: Sequence[InstanceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentinstancespaginator)
         """
 
 class ListDeploymentTargetsPaginator(AioPaginator):
@@ -177,15 +177,15 @@
     """
 
     def paginate(
         self,
         *,
         deploymentId: str,
         targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymenttargetspaginator)
         """
 
 class ListDeploymentsPaginator(AioPaginator):
@@ -198,15 +198,15 @@
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentspaginator)
         """
 
 class ListGitHubAccountTokenNamesPaginator(AioPaginator):
@@ -230,13 +230,13 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOnPremisesInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listonpremisesinstancespaginator)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/type_defs.py` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/type_defs.pyi` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/waiter.py` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy/waiter.pyi` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/PKG-INFO` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codedeploy
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeDeploy 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeDeploy 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/
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
 
 <a id="types-aiobotocore-codedeploy"></a>
 
 # types-aiobotocore-codedeploy
 
 [![PyPI - types-aiobotocore-codedeploy](https://img.shields.io/pypi/v/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [types-aiobotocore-codedeploy docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codedeploy-2.9.0/types_aiobotocore_codedeploy.egg-info/SOURCES.txt` & `types-aiobotocore-codedeploy-2.9.1/types_aiobotocore_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

