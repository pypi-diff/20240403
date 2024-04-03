# Comparing `tmp/types-aiobotocore-codeguru-reviewer-2.9.0.tar.gz` & `tmp/types-aiobotocore-codeguru-reviewer-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.9.0.tar", last modified: Wed Dec 13 19:58:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.9.1.tar", last modified: Thu Jan 18 01:20:20 2024, max compression
```

## Comparing `types-aiobotocore-codeguru-reviewer-2.9.0.tar` & `types-aiobotocore-codeguru-reviewer-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.473933 types-aiobotocore-codeguru-reviewer-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2023-12-13 19:58:54.473933 types-aiobotocore-codeguru-reviewer-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12961 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:54.473933 types-aiobotocore-codeguru-reviewer-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.473933 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16593 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18691 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18690 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:53.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.473933 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.829441 types-aiobotocore-codeguru-reviewer-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-01-18 01:20:20.829441 types-aiobotocore-codeguru-reviewer-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:20.829441 types-aiobotocore-codeguru-reviewer-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.825441 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16601 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16598 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18690 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18690 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-01-18 01:04:50.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.829441 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-01-18 01:20:20.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-18 01:20:20.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:20.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:20.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:20.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:20.000000 types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/LICENSE` & `types-aiobotocore-codeguru-reviewer-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
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
 
 <a id="types-aiobotocore-codeguru-reviewer"></a>
 
 # types-aiobotocore-codeguru-reviewer
 
 [![PyPI - types-aiobotocore-codeguru-reviewer](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/README.md` & `types-aiobotocore-codeguru-reviewer-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/setup.py` & `types-aiobotocore-codeguru-reviewer-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-reviewer",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeGuruReviewer 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeGuruReviewer 2.9.1 service generated with"
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
     keywords="aiobotocore codeguru-reviewer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codeguru_reviewer": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/__init__.py` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 from .client import CodeGuruReviewerClient
 from .paginator import ListRepositoryAssociationsPaginator
 from .waiter import CodeReviewCompletedWaiter, RepositoryAssociationSucceededWaiter
 
 Client = CodeGuruReviewerClient
 
-
 __all__ = (
     "Client",
     "CodeGuruReviewerClient",
     "CodeReviewCompletedWaiter",
     "ListRepositoryAssociationsPaginator",
     "RepositoryAssociationSucceededWaiter",
 )
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/__init__.pyi` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/__main__.py` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeGuruReviewer 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeGuruReviewer 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer\nOther"
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

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/client.py` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 from .waiter import CodeReviewCompletedWaiter, RepositoryAssociationSucceededWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeGuruReviewerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -94,15 +93,15 @@
 
     async def associate_repository(
         self,
         *,
         Repository: RepositoryTypeDef,
         ClientRequestToken: str = ...,
         Tags: Mapping[str, str] = ...,
-        KMSKeyDetails: KMSKeyDetailsTypeDef = ...
+        KMSKeyDetails: KMSKeyDetailsTypeDef = ...,
     ) -> AssociateRepositoryResponseTypeDef:
         """
         Use to associate an Amazon Web Services CodeCommit repository or a repository
         managed by Amazon Web Services CodeStar Connections with Amazon CodeGuru
         Reviewer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.associate_repository)
@@ -127,15 +126,15 @@
 
     async def create_code_review(
         self,
         *,
         Name: str,
         RepositoryAssociationArn: str,
         Type: CodeReviewTypeTypeDef,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateCodeReviewResponseTypeDef:
         """
         Use to create a code review with a
         [CodeReviewType](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CodeReviewType.html)
         of
         `RepositoryAnalysis`.
 
@@ -204,15 +203,15 @@
         self,
         *,
         Type: TypeType,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[JobStateType] = ...,
         RepositoryNames: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCodeReviewsResponseTypeDef:
         """
         Lists all the code reviews that the customer has created in the past 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_code_reviews)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/client/#list_code_reviews)
         """
@@ -220,15 +219,15 @@
     async def list_recommendation_feedback(
         self,
         *,
         CodeReviewArn: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         UserIds: Sequence[str] = ...,
-        RecommendationIds: Sequence[str] = ...
+        RecommendationIds: Sequence[str] = ...,
     ) -> ListRecommendationFeedbackResponseTypeDef:
         """
         Returns a list of
         [RecommendationFeedbackSummary](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RecommendationFeedbackSummary.html)
         objects that contain customer recommendation feedback for all CodeGuru Reviewer
         users.
 
@@ -250,15 +249,15 @@
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRepositoryAssociationsResponseTypeDef:
         """
         Returns a list of
         [RepositoryAssociationSummary](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RepositoryAssociationSummary.html)
         objects that contain summary information about a repository
         association.
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/client.pyi` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     async def associate_repository(
         self,
         *,
         Repository: RepositoryTypeDef,
         ClientRequestToken: str = ...,
         Tags: Mapping[str, str] = ...,
-        KMSKeyDetails: KMSKeyDetailsTypeDef = ...
+        KMSKeyDetails: KMSKeyDetailsTypeDef = ...,
     ) -> AssociateRepositoryResponseTypeDef:
         """
         Use to associate an Amazon Web Services CodeCommit repository or a repository
         managed by Amazon Web Services CodeStar Connections with Amazon CodeGuru
         Reviewer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.associate_repository)
@@ -123,15 +123,15 @@
 
     async def create_code_review(
         self,
         *,
         Name: str,
         RepositoryAssociationArn: str,
         Type: CodeReviewTypeTypeDef,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateCodeReviewResponseTypeDef:
         """
         Use to create a code review with a
         [CodeReviewType](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CodeReviewType.html)
         of
         `RepositoryAnalysis`.
 
@@ -200,15 +200,15 @@
         self,
         *,
         Type: TypeType,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[JobStateType] = ...,
         RepositoryNames: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCodeReviewsResponseTypeDef:
         """
         Lists all the code reviews that the customer has created in the past 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_code_reviews)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/client/#list_code_reviews)
         """
@@ -216,15 +216,15 @@
     async def list_recommendation_feedback(
         self,
         *,
         CodeReviewArn: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         UserIds: Sequence[str] = ...,
-        RecommendationIds: Sequence[str] = ...
+        RecommendationIds: Sequence[str] = ...,
     ) -> ListRecommendationFeedbackResponseTypeDef:
         """
         Returns a list of
         [RecommendationFeedbackSummary](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RecommendationFeedbackSummary.html)
         objects that contain customer recommendation feedback for all CodeGuru Reviewer
         users.
 
@@ -246,15 +246,15 @@
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRepositoryAssociationsResponseTypeDef:
         """
         Returns a list of
         [RepositoryAssociationSummary](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RepositoryAssociationSummary.html)
         objects that contain summary information about a repository
         association.
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/literals.py` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/literals.py`

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
     "AnalysisTypeType",
     "CodeReviewCompletedWaiterName",
     "ConfigFileStateType",
     "EncryptionOptionType",
     "JobStateType",
     "ListRepositoryAssociationsPaginatorName",
@@ -39,15 +38,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AnalysisTypeType = Literal["CodeQuality", "Security"]
 CodeReviewCompletedWaiterName = Literal["code_review_completed"]
 ConfigFileStateType = Literal["Absent", "Present", "PresentWithErrors"]
 EncryptionOptionType = Literal["AWS_OWNED_CMK", "CUSTOMER_MANAGED_CMK"]
 JobStateType = Literal["Completed", "Deleting", "Failed", "Pending"]
 ListRepositoryAssociationsPaginatorName = Literal["list_repository_associations"]
 ProviderTypeType = Literal[
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/literals.pyi` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/paginator.py` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from botocore.paginate import PageIterator
 
 from .literals import ProviderTypeType, RepositoryAssociationStateType
 from .type_defs import ListRepositoryAssociationsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListRepositoryAssociationsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -51,13 +50,13 @@
     def paginate(
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRepositoryAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/paginators/#listrepositoryassociationspaginator)
         """
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/paginator.pyi` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     def paginate(
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRepositoryAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/paginators/#listrepositoryassociationspaginator)
         """
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/type_defs.py` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "KMSKeyDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/type_defs.pyi` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/waiter.py` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer/waiter.pyi` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
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
 
 <a id="types-aiobotocore-codeguru-reviewer"></a>
 
 # types-aiobotocore-codeguru-reviewer
 
 [![PyPI - types-aiobotocore-codeguru-reviewer](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.9.0/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-reviewer-2.9.1/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

