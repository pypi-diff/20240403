# Comparing `tmp/types-aiobotocore-codeartifact-2.9.0.tar.gz` & `tmp/types-aiobotocore-codeartifact-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeartifact-2.9.0.tar", last modified: Wed Dec 13 19:58:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeartifact-2.9.1.tar", last modified: Thu Jan 18 01:20:19 2024, max compression
```

## Comparing `types-aiobotocore-codeartifact-2.9.0.tar` & `types-aiobotocore-codeartifact-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.581949 types-aiobotocore-codeartifact-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14020 2023-12-13 19:58:52.581949 types-aiobotocore-codeartifact-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:52.581949 types-aiobotocore-codeartifact-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.577949 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36422 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    36418 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35074 2023-12-13 19:42:41.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35073 2023-12-13 19:42:41.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:40.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.581949 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14020 2023-12-13 19:58:52.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:58:52.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:52.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:52.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:52.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:58:52.000000 types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.097449 types-aiobotocore-codeartifact-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-01-18 01:20:19.097449 types-aiobotocore-codeartifact-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:19.097449 types-aiobotocore-codeartifact-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:04:35.000000 types-aiobotocore-codeartifact-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.097449 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36440 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36437 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-01-18 01:04:37.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    35073 2024-01-18 01:04:38.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35073 2024-01-18 01:04:37.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:36.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.097449 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-01-18 01:20:19.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:19.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:19.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:19.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:19.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:19.000000 types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/LICENSE` & `types-aiobotocore-codeartifact-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codeartifact-2.9.0/PKG-INFO` & `types-aiobotocore-codeartifact-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeartifact
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeArtifact 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeArtifact 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/
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
 
 <a id="types-aiobotocore-codeartifact"></a>
 
 # types-aiobotocore-codeartifact
 
 [![PyPI - types-aiobotocore-codeartifact](https://img.shields.io/pypi/v/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeArtifact 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[aiobotocore.CodeArtifact 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [types-aiobotocore-codeartifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/README.md` & `types-aiobotocore-codeartifact-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeArtifact 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[aiobotocore.CodeArtifact 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [types-aiobotocore-codeartifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/setup.py` & `types-aiobotocore-codeartifact-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeartifact",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeArtifact 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeArtifact 2.9.1 service generated with"
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
     keywords="aiobotocore codeartifact type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codeartifact": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/__init__.py` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
 )
 
 Client = CodeArtifactClient
 
-
 __all__ = (
     "Client",
     "CodeArtifactClient",
     "ListDomainsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/__init__.pyi` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/__main__.py` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeArtifact 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeArtifact 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
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

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/client.py` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeArtifactClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -159,15 +158,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         versions: Sequence[str] = ...,
         versionRevisions: Mapping[str, str] = ...,
         allowOverwrite: bool = ...,
-        includeFromUpstream: bool = ...
+        includeFromUpstream: bool = ...,
     ) -> CopyPackageVersionsResultTypeDef:
         """
         Copies package versions from one repository to another repository in the same
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.copy_package_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#copy_package_versions)
@@ -187,15 +186,15 @@
         self,
         *,
         domain: str,
         repository: str,
         domainOwner: str = ...,
         description: str = ...,
         upstreams: Sequence[UpstreamRepositoryTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryResultTypeDef:
         """
         Creates a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#create_repository)
         """
@@ -224,15 +223,15 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DeletePackageResultTypeDef:
         """
         Deletes a package and all associated package versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#delete_package)
         """
@@ -243,15 +242,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         domainOwner: str = ...,
         namespace: str = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> DeletePackageVersionsResultTypeDef:
         """
         Deletes one or more versions of a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#delete_package_versions)
         """
@@ -293,15 +292,15 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DescribePackageResultTypeDef:
         """
         Returns a
         [PackageDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageDescription.html)
         object that contains information about the requested
         package.
 
@@ -314,15 +313,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DescribePackageVersionResultTypeDef:
         """
         Returns a
         [PackageVersionDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionDescription.html)
         object that contains information about the requested package
         version.
 
@@ -359,15 +358,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         domainOwner: str = ...,
         namespace: str = ...,
         versionRevisions: Mapping[str, str] = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> DisposePackageVersionsResultTypeDef:
         """
         Deletes the assets in package versions and sets the package versions' status to
         `Disposed`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.dispose_package_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#dispose_package_versions)
@@ -415,15 +414,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         asset: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        packageVersionRevision: str = ...
+        packageVersionRevision: str = ...,
     ) -> GetPackageVersionAssetResultTypeDef:
         """
         Returns an asset (or file) that is in a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_package_version_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#get_package_version_asset)
         """
@@ -433,15 +432,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> GetPackageVersionReadmeResultTypeDef:
         """
         Gets the readme file or descriptive text for a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_package_version_readme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#get_package_version_readme)
         """
@@ -487,15 +486,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionAssetsResultTypeDef:
         """
         Returns a list of
         [AssetSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_AssetSummary.html)
         objects for assets in a package
         version.
 
@@ -509,15 +508,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionDependenciesResultTypeDef:
         """
         Returns the direct dependencies for a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_package_version_dependencies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#list_package_version_dependencies)
         """
@@ -531,15 +530,15 @@
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        originType: PackageVersionOriginTypeType = ...
+        originType: PackageVersionOriginTypeType = ...,
     ) -> ListPackageVersionsResultTypeDef:
         """
         Returns a list of
         [PackageVersionSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionSummary.html)
         objects for package versions in a repository that match the request
         parameters.
 
@@ -555,15 +554,15 @@
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         publish: AllowPublishType = ...,
-        upstream: AllowUpstreamType = ...
+        upstream: AllowUpstreamType = ...,
     ) -> ListPackagesResultTypeDef:
         """
         Returns a list of
         [PackageSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageSummary.html)
         objects for packages in a repository that match the request
         parameters.
 
@@ -587,15 +586,15 @@
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRepositoriesInDomainResultTypeDef:
         """
         Returns a list of
         [RepositorySummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_RepositorySummary.html)
         objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_repositories_in_domain)
@@ -621,15 +620,15 @@
         package: str,
         packageVersion: str,
         assetContent: BlobTypeDef,
         assetName: str,
         assetSHA256: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        unfinished: bool = ...
+        unfinished: bool = ...,
     ) -> PublishPackageVersionResultTypeDef:
         """
         Creates a new package version containing one or more assets (or files).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.publish_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#publish_package_version)
         """
@@ -649,15 +648,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         restrictions: PackageOriginRestrictionsTypeDef,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> PutPackageOriginConfigurationResultTypeDef:
         """
         Sets the package origin configuration for a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.put_package_origin_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#put_package_origin_configuration)
         """
@@ -665,15 +664,15 @@
     async def put_repository_permissions_policy(
         self,
         *,
         domain: str,
         repository: str,
         policyDocument: str,
         domainOwner: str = ...,
-        policyRevision: str = ...
+        policyRevision: str = ...,
     ) -> PutRepositoryPermissionsPolicyResultTypeDef:
         """
         Sets the resource policy on a repository that specifies permissions to access
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.put_repository_permissions_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#put_repository_permissions_policy)
@@ -703,15 +702,15 @@
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         targetStatus: PackageVersionStatusType,
         domainOwner: str = ...,
         namespace: str = ...,
         versionRevisions: Mapping[str, str] = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> UpdatePackageVersionsStatusResultTypeDef:
         """
         Updates the status of one or more versions of a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_package_versions_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#update_package_versions_status)
         """
@@ -719,15 +718,15 @@
     async def update_repository(
         self,
         *,
         domain: str,
         repository: str,
         domainOwner: str = ...,
         description: str = ...,
-        upstreams: Sequence[UpstreamRepositoryTypeDef] = ...
+        upstreams: Sequence[UpstreamRepositoryTypeDef] = ...,
     ) -> UpdateRepositoryResultTypeDef:
         """
         Update the properties of a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#update_repository)
         """
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/client.pyi` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         versions: Sequence[str] = ...,
         versionRevisions: Mapping[str, str] = ...,
         allowOverwrite: bool = ...,
-        includeFromUpstream: bool = ...
+        includeFromUpstream: bool = ...,
     ) -> CopyPackageVersionsResultTypeDef:
         """
         Copies package versions from one repository to another repository in the same
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.copy_package_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#copy_package_versions)
@@ -183,15 +183,15 @@
         self,
         *,
         domain: str,
         repository: str,
         domainOwner: str = ...,
         description: str = ...,
         upstreams: Sequence[UpstreamRepositoryTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryResultTypeDef:
         """
         Creates a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#create_repository)
         """
@@ -220,15 +220,15 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DeletePackageResultTypeDef:
         """
         Deletes a package and all associated package versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#delete_package)
         """
@@ -239,15 +239,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         domainOwner: str = ...,
         namespace: str = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> DeletePackageVersionsResultTypeDef:
         """
         Deletes one or more versions of a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#delete_package_versions)
         """
@@ -289,15 +289,15 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DescribePackageResultTypeDef:
         """
         Returns a
         [PackageDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageDescription.html)
         object that contains information about the requested
         package.
 
@@ -310,15 +310,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DescribePackageVersionResultTypeDef:
         """
         Returns a
         [PackageVersionDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionDescription.html)
         object that contains information about the requested package
         version.
 
@@ -355,15 +355,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         domainOwner: str = ...,
         namespace: str = ...,
         versionRevisions: Mapping[str, str] = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> DisposePackageVersionsResultTypeDef:
         """
         Deletes the assets in package versions and sets the package versions' status to
         `Disposed`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.dispose_package_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#dispose_package_versions)
@@ -411,15 +411,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         asset: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        packageVersionRevision: str = ...
+        packageVersionRevision: str = ...,
     ) -> GetPackageVersionAssetResultTypeDef:
         """
         Returns an asset (or file) that is in a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_package_version_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#get_package_version_asset)
         """
@@ -429,15 +429,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> GetPackageVersionReadmeResultTypeDef:
         """
         Gets the readme file or descriptive text for a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_package_version_readme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#get_package_version_readme)
         """
@@ -483,15 +483,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionAssetsResultTypeDef:
         """
         Returns a list of
         [AssetSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_AssetSummary.html)
         objects for assets in a package
         version.
 
@@ -505,15 +505,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionDependenciesResultTypeDef:
         """
         Returns the direct dependencies for a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_package_version_dependencies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#list_package_version_dependencies)
         """
@@ -527,15 +527,15 @@
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        originType: PackageVersionOriginTypeType = ...
+        originType: PackageVersionOriginTypeType = ...,
     ) -> ListPackageVersionsResultTypeDef:
         """
         Returns a list of
         [PackageVersionSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionSummary.html)
         objects for package versions in a repository that match the request
         parameters.
 
@@ -551,15 +551,15 @@
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         publish: AllowPublishType = ...,
-        upstream: AllowUpstreamType = ...
+        upstream: AllowUpstreamType = ...,
     ) -> ListPackagesResultTypeDef:
         """
         Returns a list of
         [PackageSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageSummary.html)
         objects for packages in a repository that match the request
         parameters.
 
@@ -583,15 +583,15 @@
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRepositoriesInDomainResultTypeDef:
         """
         Returns a list of
         [RepositorySummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_RepositorySummary.html)
         objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_repositories_in_domain)
@@ -617,15 +617,15 @@
         package: str,
         packageVersion: str,
         assetContent: BlobTypeDef,
         assetName: str,
         assetSHA256: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        unfinished: bool = ...
+        unfinished: bool = ...,
     ) -> PublishPackageVersionResultTypeDef:
         """
         Creates a new package version containing one or more assets (or files).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.publish_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#publish_package_version)
         """
@@ -645,15 +645,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         restrictions: PackageOriginRestrictionsTypeDef,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> PutPackageOriginConfigurationResultTypeDef:
         """
         Sets the package origin configuration for a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.put_package_origin_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#put_package_origin_configuration)
         """
@@ -661,15 +661,15 @@
     async def put_repository_permissions_policy(
         self,
         *,
         domain: str,
         repository: str,
         policyDocument: str,
         domainOwner: str = ...,
-        policyRevision: str = ...
+        policyRevision: str = ...,
     ) -> PutRepositoryPermissionsPolicyResultTypeDef:
         """
         Sets the resource policy on a repository that specifies permissions to access
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.put_repository_permissions_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#put_repository_permissions_policy)
@@ -699,15 +699,15 @@
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         targetStatus: PackageVersionStatusType,
         domainOwner: str = ...,
         namespace: str = ...,
         versionRevisions: Mapping[str, str] = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> UpdatePackageVersionsStatusResultTypeDef:
         """
         Updates the status of one or more versions of a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_package_versions_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#update_package_versions_status)
         """
@@ -715,15 +715,15 @@
     async def update_repository(
         self,
         *,
         domain: str,
         repository: str,
         domainOwner: str = ...,
         description: str = ...,
-        upstreams: Sequence[UpstreamRepositoryTypeDef] = ...
+        upstreams: Sequence[UpstreamRepositoryTypeDef] = ...,
     ) -> UpdateRepositoryResultTypeDef:
         """
         Update the properties of a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/client/#update_repository)
         """
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/literals.py` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/literals.py`

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
     "AllowPublishType",
     "AllowUpstreamType",
     "DomainStatusType",
     "ExternalConnectionStatusType",
     "HashAlgorithmType",
     "ListDomainsPaginatorName",
@@ -40,15 +39,14 @@
     "CodeArtifactServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AllowPublishType = Literal["ALLOW", "BLOCK"]
 AllowUpstreamType = Literal["ALLOW", "BLOCK"]
 DomainStatusType = Literal["Active", "Deleted"]
 ExternalConnectionStatusType = Literal["Available"]
 HashAlgorithmType = Literal["MD5", "SHA-1", "SHA-256", "SHA-512"]
 ListDomainsPaginatorName = Literal["list_domains"]
 ListPackageVersionAssetsPaginatorName = Literal["list_package_version_assets"]
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/literals.pyi` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/paginator.py` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,25 +55,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDomainsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesPaginator",
     "ListRepositoriesInDomainPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -107,15 +105,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
 
@@ -133,15 +131,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionspaginator)
         """
 
 
@@ -158,15 +156,15 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackagespaginator)
         """
 
 
@@ -194,13 +192,13 @@
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/paginator.pyi` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
 class ListPackageVersionsPaginator(AioPaginator):
@@ -127,15 +127,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackageversionspaginator)
         """
 
 class ListPackagesPaginator(AioPaginator):
@@ -151,15 +151,15 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listpackagespaginator)
         """
 
 class ListRepositoriesPaginator(AioPaginator):
@@ -185,13 +185,13 @@
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/type_defs.py` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BlobTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact/type_defs.pyi` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/PKG-INFO` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeartifact
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeArtifact 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeArtifact 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/
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
 
 <a id="types-aiobotocore-codeartifact"></a>
 
 # types-aiobotocore-codeartifact
 
 [![PyPI - types-aiobotocore-codeartifact](https://img.shields.io/pypi/v/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeArtifact 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[aiobotocore.CodeArtifact 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [types-aiobotocore-codeartifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeartifact-2.9.0/types_aiobotocore_codeartifact.egg-info/SOURCES.txt` & `types-aiobotocore-codeartifact-2.9.1/types_aiobotocore_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

