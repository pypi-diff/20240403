# Comparing `tmp/types-aiobotocore-elasticbeanstalk-2.9.0.tar.gz` & `tmp/types-aiobotocore-elasticbeanstalk-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elasticbeanstalk-2.9.0.tar", last modified: Wed Dec 13 19:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-elasticbeanstalk-2.9.1.tar", last modified: Thu Jan 18 01:20:39 2024, max compression
```

## Comparing `types-aiobotocore-elasticbeanstalk-2.9.0.tar` & `types-aiobotocore-elasticbeanstalk-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.557768 types-aiobotocore-elasticbeanstalk-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2023-12-13 19:59:14.557768 types-aiobotocore-elasticbeanstalk-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13755 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:14.557768 types-aiobotocore-elasticbeanstalk-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.557768 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45137 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    45133 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12366 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    50651 2023-12-13 19:45:46.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50650 2023-12-13 19:45:45.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2023-12-13 19:45:43.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.557768 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2023-12-13 19:59:14.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-13 19:59:14.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:14.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:14.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:14.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:59:14.000000 types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.405349 types-aiobotocore-elasticbeanstalk-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-01-18 01:20:39.405349 types-aiobotocore-elasticbeanstalk-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:39.405349 types-aiobotocore-elasticbeanstalk-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.405349 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45161 2024-01-18 01:07:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45158 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-01-18 01:07:40.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-01-18 01:07:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-01-18 01:07:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-01-18 01:07:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    50650 2024-01-18 01:07:41.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50650 2024-01-18 01:07:41.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:38.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-01-18 01:07:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-01-18 01:07:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.405349 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-01-18 01:20:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-01-18 01:20:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:20:39.000000 types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/LICENSE` & `types-aiobotocore-elasticbeanstalk-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/PKG-INFO` & `types-aiobotocore-elasticbeanstalk-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticbeanstalk
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/
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
 
 <a id="types-aiobotocore-elasticbeanstalk"></a>
 
 # types-aiobotocore-elasticbeanstalk
 
 [![PyPI - types-aiobotocore-elasticbeanstalk](https://img.shields.io/pypi/v/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticBeanstalk 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[aiobotocore.ElasticBeanstalk 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [types-aiobotocore-elasticbeanstalk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/README.md` & `types-aiobotocore-elasticbeanstalk-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticBeanstalk 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[aiobotocore.ElasticBeanstalk 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [types-aiobotocore-elasticbeanstalk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/setup.py` & `types-aiobotocore-elasticbeanstalk-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elasticbeanstalk",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_elasticbeanstalk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticBeanstalk 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ElasticBeanstalk 2.9.1 service generated with"
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
     keywords="aiobotocore elasticbeanstalk type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elasticbeanstalk": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/__init__.py` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     DescribeEventsPaginator,
     ListPlatformVersionsPaginator,
 )
 from .waiter import EnvironmentExistsWaiter, EnvironmentTerminatedWaiter, EnvironmentUpdatedWaiter
 
 Client = ElasticBeanstalkClient
 
-
 __all__ = (
     "Client",
     "DescribeApplicationVersionsPaginator",
     "DescribeEnvironmentManagedActionHistoryPaginator",
     "DescribeEnvironmentsPaginator",
     "DescribeEventsPaginator",
     "ElasticBeanstalkClient",
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/__init__.pyi` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/__main__.py` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticBeanstalk 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ElasticBeanstalk 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk\nOther"
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

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/client.py` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 from .waiter import EnvironmentExistsWaiter, EnvironmentTerminatedWaiter, EnvironmentUpdatedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ElasticBeanstalkClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -196,15 +195,15 @@
         """
 
     async def compose_environments(
         self,
         *,
         ApplicationName: str = ...,
         GroupName: str = ...,
-        VersionLabels: Sequence[str] = ...
+        VersionLabels: Sequence[str] = ...,
     ) -> EnvironmentDescriptionsMessageTypeDef:
         """
         Create or update a group of environments that each run a separate component of
         a single
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.compose_environments)
@@ -213,15 +212,15 @@
 
     async def create_application(
         self,
         *,
         ApplicationName: str,
         Description: str = ...,
         ResourceLifecycleConfig: ApplicationResourceLifecycleConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ApplicationDescriptionMessageTypeDef:
         """
         Creates an application that has one configuration template named `default` and
         no application
         versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_application)
@@ -235,15 +234,15 @@
         VersionLabel: str,
         Description: str = ...,
         SourceBuildInformation: SourceBuildInformationTypeDef = ...,
         SourceBundle: S3LocationTypeDef = ...,
         BuildConfiguration: BuildConfigurationTypeDef = ...,
         AutoCreateApplication: bool = ...,
         Process: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ApplicationVersionDescriptionMessageTypeDef:
         """
         Creates an application version for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_application_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#create_application_version)
         """
@@ -255,15 +254,15 @@
         TemplateName: str,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         SourceConfiguration: SourceConfigurationTypeDef = ...,
         EnvironmentId: str = ...,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Creates an AWS Elastic Beanstalk configuration template, associated with a
         specific Elastic Beanstalk
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_configuration_template)
@@ -282,15 +281,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
-        OperationsRole: str = ...
+        OperationsRole: str = ...,
     ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Launches an AWS Elastic Beanstalk environment for the specified application
         using the specified
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_environment)
@@ -301,15 +300,15 @@
         self,
         *,
         PlatformName: str,
         PlatformVersion: str,
         PlatformDefinitionBundle: S3LocationTypeDef,
         EnvironmentName: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePlatformVersionResultTypeDef:
         """
         Create a new version of your custom platform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_platform_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#create_platform_version)
         """
@@ -387,15 +386,15 @@
 
     async def describe_application_versions(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ApplicationVersionDescriptionsMessageTypeDef:
         """
         Retrieve a list of application versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_application_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_application_versions)
         """
@@ -414,15 +413,15 @@
         self,
         *,
         ApplicationName: str = ...,
         TemplateName: str = ...,
         EnvironmentName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
-        Options: Sequence[OptionSpecificationTypeDef] = ...
+        Options: Sequence[OptionSpecificationTypeDef] = ...,
     ) -> ConfigurationOptionsDescriptionTypeDef:
         """
         Describes the configuration options that are used in a particular configuration
         template or environment, or that a specified solution stack
         defines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_configuration_options)
@@ -443,44 +442,44 @@
         """
 
     async def describe_environment_health(
         self,
         *,
         EnvironmentName: str = ...,
         EnvironmentId: str = ...,
-        AttributeNames: Sequence[EnvironmentHealthAttributeType] = ...
+        AttributeNames: Sequence[EnvironmentHealthAttributeType] = ...,
     ) -> DescribeEnvironmentHealthResultTypeDef:
         """
         Returns information about the overall health of the specified environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environment_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_environment_health)
         """
 
     async def describe_environment_managed_action_history(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         NextToken: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> DescribeEnvironmentManagedActionHistoryResultTypeDef:
         """
         Lists an environment's completed and failed managed actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environment_managed_action_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_environment_managed_action_history)
         """
 
     async def describe_environment_managed_actions(
         self,
         *,
         EnvironmentName: str = ...,
         EnvironmentId: str = ...,
-        Status: ActionStatusType = ...
+        Status: ActionStatusType = ...,
     ) -> DescribeEnvironmentManagedActionsResultTypeDef:
         """
         Lists an environment's upcoming and in-progress managed actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environment_managed_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_environment_managed_actions)
         """
@@ -501,15 +500,15 @@
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> EnvironmentDescriptionsMessageTypeDef:
         """
         Returns descriptions for existing environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_environments)
         """
@@ -524,30 +523,30 @@
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> EventDescriptionsMessageTypeDef:
         """
         Returns list of event descriptions matching criteria up to the last 6 weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_events)
         """
 
     async def describe_instances_health(
         self,
         *,
         EnvironmentName: str = ...,
         EnvironmentId: str = ...,
         AttributeNames: Sequence[InstancesHealthAttributeType] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeInstancesHealthResultTypeDef:
         """
         Retrieves detailed information about the health of instances in your AWS
         Elastic
         Beanstalk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_instances_health)
@@ -601,29 +600,29 @@
         """
 
     async def list_platform_branches(
         self,
         *,
         Filters: Sequence[SearchFilterTypeDef] = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPlatformBranchesResultTypeDef:
         """
         Lists the platform branches available for your account in an AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.list_platform_branches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#list_platform_branches)
         """
 
     async def list_platform_versions(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPlatformVersionsResultTypeDef:
         """
         Lists the platform versions available for your account in an AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.list_platform_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#list_platform_versions)
         """
@@ -651,15 +650,15 @@
         """
 
     async def request_environment_info(
         self,
         *,
         InfoType: EnvironmentInfoTypeType,
         EnvironmentId: str = ...,
-        EnvironmentName: str = ...
+        EnvironmentName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Initiates a request to compile the specified type of information of the
         deployed
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.request_environment_info)
@@ -679,45 +678,45 @@
         """
 
     async def retrieve_environment_info(
         self,
         *,
         InfoType: EnvironmentInfoTypeType,
         EnvironmentId: str = ...,
-        EnvironmentName: str = ...
+        EnvironmentName: str = ...,
     ) -> RetrieveEnvironmentInfoResultMessageTypeDef:
         """
         Retrieves the compiled information from a  RequestEnvironmentInfo request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.retrieve_environment_info)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#retrieve_environment_info)
         """
 
     async def swap_environment_cnames(
         self,
         *,
         SourceEnvironmentId: str = ...,
         SourceEnvironmentName: str = ...,
         DestinationEnvironmentId: str = ...,
-        DestinationEnvironmentName: str = ...
+        DestinationEnvironmentName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Swaps the CNAMEs of two environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.swap_environment_cnames)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#swap_environment_cnames)
         """
 
     async def terminate_environment(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         TerminateResources: bool = ...,
-        ForceTerminate: bool = ...
+        ForceTerminate: bool = ...,
     ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Terminates the specified environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.terminate_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#terminate_environment)
         """
@@ -732,15 +731,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_application)
         """
 
     async def update_application_resource_lifecycle(
         self,
         *,
         ApplicationName: str,
-        ResourceLifecycleConfig: ApplicationResourceLifecycleConfigTypeDef
+        ResourceLifecycleConfig: ApplicationResourceLifecycleConfigTypeDef,
     ) -> ApplicationResourceLifecycleDescriptionMessageTypeDef:
         """
         Modifies lifecycle settings for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_application_resource_lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_application_resource_lifecycle)
         """
@@ -758,15 +757,15 @@
     async def update_configuration_template(
         self,
         *,
         ApplicationName: str,
         TemplateName: str,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
-        OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
+        OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
     ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Updates the specified configuration template to have the specified properties
         or configuration option
         values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_configuration_template)
@@ -783,15 +782,15 @@
         Description: str = ...,
         Tier: EnvironmentTierTypeDef = ...,
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
-        OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
+        OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
     ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Updates the environment description, deploys a new application version, updates
         the configuration settings to an entirely new configuration template, or
         updates select configuration option values in the running
         environment.
 
@@ -800,30 +799,30 @@
         """
 
     async def update_tags_for_resource(
         self,
         *,
         ResourceArn: str,
         TagsToAdd: Sequence[TagTypeDef] = ...,
-        TagsToRemove: Sequence[str] = ...
+        TagsToRemove: Sequence[str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update the list of tags applied to an AWS Elastic Beanstalk resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_tags_for_resource)
         """
 
     async def validate_configuration_settings(
         self,
         *,
         ApplicationName: str,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef],
         TemplateName: str = ...,
-        EnvironmentName: str = ...
+        EnvironmentName: str = ...,
     ) -> ConfigurationSettingsValidationMessagesTypeDef:
         """
         Takes a set of configuration settings and either a configuration template or
         environment, and determines whether those values are
         valid.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.validate_configuration_settings)
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/client.pyi` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         """
 
     async def compose_environments(
         self,
         *,
         ApplicationName: str = ...,
         GroupName: str = ...,
-        VersionLabels: Sequence[str] = ...
+        VersionLabels: Sequence[str] = ...,
     ) -> EnvironmentDescriptionsMessageTypeDef:
         """
         Create or update a group of environments that each run a separate component of
         a single
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.compose_environments)
@@ -209,15 +209,15 @@
 
     async def create_application(
         self,
         *,
         ApplicationName: str,
         Description: str = ...,
         ResourceLifecycleConfig: ApplicationResourceLifecycleConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ApplicationDescriptionMessageTypeDef:
         """
         Creates an application that has one configuration template named `default` and
         no application
         versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_application)
@@ -231,15 +231,15 @@
         VersionLabel: str,
         Description: str = ...,
         SourceBuildInformation: SourceBuildInformationTypeDef = ...,
         SourceBundle: S3LocationTypeDef = ...,
         BuildConfiguration: BuildConfigurationTypeDef = ...,
         AutoCreateApplication: bool = ...,
         Process: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ApplicationVersionDescriptionMessageTypeDef:
         """
         Creates an application version for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_application_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#create_application_version)
         """
@@ -251,15 +251,15 @@
         TemplateName: str,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         SourceConfiguration: SourceConfigurationTypeDef = ...,
         EnvironmentId: str = ...,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Creates an AWS Elastic Beanstalk configuration template, associated with a
         specific Elastic Beanstalk
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_configuration_template)
@@ -278,15 +278,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
-        OperationsRole: str = ...
+        OperationsRole: str = ...,
     ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Launches an AWS Elastic Beanstalk environment for the specified application
         using the specified
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_environment)
@@ -297,15 +297,15 @@
         self,
         *,
         PlatformName: str,
         PlatformVersion: str,
         PlatformDefinitionBundle: S3LocationTypeDef,
         EnvironmentName: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePlatformVersionResultTypeDef:
         """
         Create a new version of your custom platform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_platform_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#create_platform_version)
         """
@@ -383,15 +383,15 @@
 
     async def describe_application_versions(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ApplicationVersionDescriptionsMessageTypeDef:
         """
         Retrieve a list of application versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_application_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_application_versions)
         """
@@ -410,15 +410,15 @@
         self,
         *,
         ApplicationName: str = ...,
         TemplateName: str = ...,
         EnvironmentName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
-        Options: Sequence[OptionSpecificationTypeDef] = ...
+        Options: Sequence[OptionSpecificationTypeDef] = ...,
     ) -> ConfigurationOptionsDescriptionTypeDef:
         """
         Describes the configuration options that are used in a particular configuration
         template or environment, or that a specified solution stack
         defines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_configuration_options)
@@ -439,44 +439,44 @@
         """
 
     async def describe_environment_health(
         self,
         *,
         EnvironmentName: str = ...,
         EnvironmentId: str = ...,
-        AttributeNames: Sequence[EnvironmentHealthAttributeType] = ...
+        AttributeNames: Sequence[EnvironmentHealthAttributeType] = ...,
     ) -> DescribeEnvironmentHealthResultTypeDef:
         """
         Returns information about the overall health of the specified environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environment_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_environment_health)
         """
 
     async def describe_environment_managed_action_history(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         NextToken: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> DescribeEnvironmentManagedActionHistoryResultTypeDef:
         """
         Lists an environment's completed and failed managed actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environment_managed_action_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_environment_managed_action_history)
         """
 
     async def describe_environment_managed_actions(
         self,
         *,
         EnvironmentName: str = ...,
         EnvironmentId: str = ...,
-        Status: ActionStatusType = ...
+        Status: ActionStatusType = ...,
     ) -> DescribeEnvironmentManagedActionsResultTypeDef:
         """
         Lists an environment's upcoming and in-progress managed actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environment_managed_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_environment_managed_actions)
         """
@@ -497,15 +497,15 @@
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> EnvironmentDescriptionsMessageTypeDef:
         """
         Returns descriptions for existing environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_environments)
         """
@@ -520,30 +520,30 @@
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> EventDescriptionsMessageTypeDef:
         """
         Returns list of event descriptions matching criteria up to the last 6 weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#describe_events)
         """
 
     async def describe_instances_health(
         self,
         *,
         EnvironmentName: str = ...,
         EnvironmentId: str = ...,
         AttributeNames: Sequence[InstancesHealthAttributeType] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeInstancesHealthResultTypeDef:
         """
         Retrieves detailed information about the health of instances in your AWS
         Elastic
         Beanstalk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_instances_health)
@@ -597,29 +597,29 @@
         """
 
     async def list_platform_branches(
         self,
         *,
         Filters: Sequence[SearchFilterTypeDef] = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPlatformBranchesResultTypeDef:
         """
         Lists the platform branches available for your account in an AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.list_platform_branches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#list_platform_branches)
         """
 
     async def list_platform_versions(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPlatformVersionsResultTypeDef:
         """
         Lists the platform versions available for your account in an AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.list_platform_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#list_platform_versions)
         """
@@ -647,15 +647,15 @@
         """
 
     async def request_environment_info(
         self,
         *,
         InfoType: EnvironmentInfoTypeType,
         EnvironmentId: str = ...,
-        EnvironmentName: str = ...
+        EnvironmentName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Initiates a request to compile the specified type of information of the
         deployed
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.request_environment_info)
@@ -675,45 +675,45 @@
         """
 
     async def retrieve_environment_info(
         self,
         *,
         InfoType: EnvironmentInfoTypeType,
         EnvironmentId: str = ...,
-        EnvironmentName: str = ...
+        EnvironmentName: str = ...,
     ) -> RetrieveEnvironmentInfoResultMessageTypeDef:
         """
         Retrieves the compiled information from a  RequestEnvironmentInfo request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.retrieve_environment_info)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#retrieve_environment_info)
         """
 
     async def swap_environment_cnames(
         self,
         *,
         SourceEnvironmentId: str = ...,
         SourceEnvironmentName: str = ...,
         DestinationEnvironmentId: str = ...,
-        DestinationEnvironmentName: str = ...
+        DestinationEnvironmentName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Swaps the CNAMEs of two environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.swap_environment_cnames)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#swap_environment_cnames)
         """
 
     async def terminate_environment(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         TerminateResources: bool = ...,
-        ForceTerminate: bool = ...
+        ForceTerminate: bool = ...,
     ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Terminates the specified environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.terminate_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#terminate_environment)
         """
@@ -728,15 +728,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_application)
         """
 
     async def update_application_resource_lifecycle(
         self,
         *,
         ApplicationName: str,
-        ResourceLifecycleConfig: ApplicationResourceLifecycleConfigTypeDef
+        ResourceLifecycleConfig: ApplicationResourceLifecycleConfigTypeDef,
     ) -> ApplicationResourceLifecycleDescriptionMessageTypeDef:
         """
         Modifies lifecycle settings for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_application_resource_lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_application_resource_lifecycle)
         """
@@ -754,15 +754,15 @@
     async def update_configuration_template(
         self,
         *,
         ApplicationName: str,
         TemplateName: str,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
-        OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
+        OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
     ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Updates the specified configuration template to have the specified properties
         or configuration option
         values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_configuration_template)
@@ -779,15 +779,15 @@
         Description: str = ...,
         Tier: EnvironmentTierTypeDef = ...,
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
-        OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
+        OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
     ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Updates the environment description, deploys a new application version, updates
         the configuration settings to an entirely new configuration template, or
         updates select configuration option values in the running
         environment.
 
@@ -796,30 +796,30 @@
         """
 
     async def update_tags_for_resource(
         self,
         *,
         ResourceArn: str,
         TagsToAdd: Sequence[TagTypeDef] = ...,
-        TagsToRemove: Sequence[str] = ...
+        TagsToRemove: Sequence[str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update the list of tags applied to an AWS Elastic Beanstalk resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_tags_for_resource)
         """
 
     async def validate_configuration_settings(
         self,
         *,
         ApplicationName: str,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef],
         TemplateName: str = ...,
-        EnvironmentName: str = ...
+        EnvironmentName: str = ...,
     ) -> ConfigurationSettingsValidationMessagesTypeDef:
         """
         Takes a set of configuration settings and either a configuration template or
         environment, and determines whether those values are
         valid.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.validate_configuration_settings)
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/literals.py` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/literals.py`

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
     "ActionHistoryStatusType",
     "ActionStatusType",
     "ActionTypeType",
     "ApplicationVersionStatusType",
     "ComputeTypeType",
     "ConfigurationDeploymentStatusType",
@@ -52,15 +51,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionHistoryStatusType = Literal["Completed", "Failed", "Unknown"]
 ActionStatusType = Literal["Pending", "Running", "Scheduled", "Unknown"]
 ActionTypeType = Literal["InstanceRefresh", "PlatformUpdate", "Unknown"]
 ApplicationVersionStatusType = Literal[
     "Building", "Failed", "Processed", "Processing", "Unprocessed"
 ]
 ComputeTypeType = Literal["BUILD_GENERAL1_LARGE", "BUILD_GENERAL1_MEDIUM", "BUILD_GENERAL1_SMALL"]
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/literals.pyi` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/paginator.py` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     "DescribeApplicationVersionsPaginator",
     "DescribeEnvironmentManagedActionHistoryPaginator",
     "DescribeEnvironmentsPaginator",
     "DescribeEventsPaginator",
     "ListPlatformVersionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -72,15 +71,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ApplicationVersionDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
         """
 
 
@@ -91,15 +90,15 @@
     """
 
     def paginate(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
         """
 
 
@@ -114,15 +113,15 @@
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
 
@@ -141,15 +140,15 @@
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeeventspaginator)
         """
 
 
@@ -159,13 +158,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#listplatformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPlatformVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#listplatformversionspaginator)
         """
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/paginator.pyi` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ApplicationVersionDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
         """
 
 class DescribeEnvironmentManagedActionHistoryPaginator(AioPaginator):
@@ -87,15 +87,15 @@
     """
 
     def paginate(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
         """
 
 class DescribeEnvironmentsPaginator(AioPaginator):
@@ -109,15 +109,15 @@
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -135,15 +135,15 @@
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeeventspaginator)
         """
 
 class ListPlatformVersionsPaginator(AioPaginator):
@@ -152,13 +152,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#listplatformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPlatformVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#listplatformversionspaginator)
         """
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/type_defs.py` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
     "ResponseMetadataTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
     "S3LocationTypeDef",
     "SourceBuildInformationTypeDef",
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/type_defs.pyi` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/waiter.py` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/waiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentexistswaiter)
         """
 
 
@@ -72,15 +72,15 @@
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentterminatedwaiter)
         """
 
 
@@ -97,13 +97,13 @@
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentupdatedwaiter)
         """
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk/waiter.pyi` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentexistswaiter)
         """
 
 class EnvironmentTerminatedWaiter(AIOWaiter):
@@ -70,15 +70,15 @@
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentterminatedwaiter)
         """
 
 class EnvironmentUpdatedWaiter(AIOWaiter):
@@ -94,13 +94,13 @@
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentupdatedwaiter)
         """
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticbeanstalk
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/
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
 
 <a id="types-aiobotocore-elasticbeanstalk"></a>
 
 # types-aiobotocore-elasticbeanstalk
 
 [![PyPI - types-aiobotocore-elasticbeanstalk](https://img.shields.io/pypi/v/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticBeanstalk 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[aiobotocore.ElasticBeanstalk 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [types-aiobotocore-elasticbeanstalk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.9.0/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt` & `types-aiobotocore-elasticbeanstalk-2.9.1/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

