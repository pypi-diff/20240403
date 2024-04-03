# Comparing `tmp/types-aiobotocore-opsworks-2.9.0.tar.gz` & `tmp/types-aiobotocore-opsworks-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opsworks-2.9.0.tar", last modified: Wed Dec 13 20:00:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-opsworks-2.9.1.tar", last modified: Thu Jan 18 01:21:24 2024, max compression
```

## Comparing `types-aiobotocore-opsworks-2.9.0.tar` & `types-aiobotocore-opsworks-2.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.041366 types-aiobotocore-opsworks-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:13.000000 types-aiobotocore-opsworks-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16532 2023-12-13 20:00:04.041366 types-aiobotocore-opsworks-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14965 2023-12-13 19:51:13.000000 types-aiobotocore-opsworks-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:04.041366 types-aiobotocore-opsworks-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:51:13.000000 types-aiobotocore-opsworks-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.041366 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2023-12-13 19:51:13.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-13 19:51:13.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:51:13.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54766 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54762 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:13.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21714 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    21703 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    60139 2023-12-13 19:51:15.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60138 2023-12-13 19:51:15.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:13.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2023-12-13 19:51:14.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.041366 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16532 2023-12-13 20:00:04.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-12-13 20:00:04.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:04.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:04.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:04.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:04.000000 types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.969141 types-aiobotocore-opsworks-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16552 2024-01-18 01:21:24.969141 types-aiobotocore-opsworks-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:24.969141 types-aiobotocore-opsworks-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.965141 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54782 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54779 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21859 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21849 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    60138 2024-01-18 01:12:55.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60138 2024-01-18 01:12:55.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:53.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-01-18 01:12:54.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.969141 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16552 2024-01-18 01:21:24.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-01-18 01:21:24.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:24.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:24.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:24.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:24.000000 types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opsworks-2.9.0/LICENSE` & `types-aiobotocore-opsworks-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-opsworks-2.9.0/PKG-INFO` & `types-aiobotocore-opsworks-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworks
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpsWorks 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpsWorks 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/
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
 
 <a id="types-aiobotocore-opsworks"></a>
 
 # types-aiobotocore-opsworks
 
 [![PyPI - types-aiobotocore-opsworks](https://img.shields.io/pypi/v/types-aiobotocore-opsworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworks)](https://pepy.tech/project/types-aiobotocore-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorks 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[aiobotocore.OpsWorks 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [types-aiobotocore-opsworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opsworks-2.9.0/README.md` & `types-aiobotocore-opsworks-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworks)](https://pepy.tech/project/types-aiobotocore-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorks 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[aiobotocore.OpsWorks 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [types-aiobotocore-opsworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opsworks-2.9.0/setup.py` & `types-aiobotocore-opsworks-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opsworks",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.OpsWorks 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.OpsWorks 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore opsworks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_opsworks": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/__init__.py` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,16 @@
     InstanceRegisteredWaiter,
     InstanceStoppedWaiter,
     InstanceTerminatedWaiter,
 )
 
 Client = OpsWorksClient
 
-
 ServiceResource = OpsWorksServiceResource
 
-
 __all__ = (
     "AppExistsWaiter",
     "Client",
     "DeploymentSuccessfulWaiter",
     "DescribeEcsClustersPaginator",
     "InstanceOnlineWaiter",
     "InstanceRegisteredWaiter",
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/__init__.pyi` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/__main__.py` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpsWorks 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.OpsWorks 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
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

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/client.py` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("OpsWorksClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -204,15 +203,15 @@
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         ClonePermissions: bool = ...,
         CloneAppIds: Sequence[str] = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> CloneStackResultTypeDef:
         """
         Creates a clone of a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.clone_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#clone_stack)
         """
@@ -235,15 +234,15 @@
         Description: str = ...,
         DataSources: Sequence[DataSourceTypeDef] = ...,
         AppSource: SourceTypeDef = ...,
         Domains: Sequence[str] = ...,
         EnableSsl: bool = ...,
         SslConfiguration: SslConfigurationTypeDef = ...,
         Attributes: Mapping[AppAttributesKeysType, str] = ...,
-        Environment: Sequence[EnvironmentVariableTypeDef] = ...
+        Environment: Sequence[EnvironmentVariableTypeDef] = ...,
     ) -> CreateAppResultTypeDef:
         """
         Creates an app for a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_app)
         """
@@ -253,15 +252,15 @@
         *,
         StackId: str,
         Command: DeploymentCommandTypeDef,
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
-        CustomJson: str = ...
+        CustomJson: str = ...,
     ) -> CreateDeploymentResultTypeDef:
         """
         Runs deployment or stack commands.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_deployment)
         """
@@ -282,15 +281,15 @@
         SubnetId: str = ...,
         Architecture: ArchitectureType = ...,
         RootDeviceType: RootDeviceTypeType = ...,
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         InstallUpdatesOnBoot: bool = ...,
         EbsOptimized: bool = ...,
         AgentVersion: str = ...,
-        Tenancy: str = ...
+        Tenancy: str = ...,
     ) -> CreateInstanceResultTypeDef:
         """
         Creates an instance in a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_instance)
         """
@@ -311,15 +310,15 @@
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
         CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_layer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_layer)
         """
@@ -341,30 +340,30 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> CreateStackResultTypeDef:
         """
         Creates a new stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_stack)
         """
 
     async def create_user_profile(
         self,
         *,
         IamUserArn: str,
         SshUsername: str = ...,
         SshPublicKey: str = ...,
-        AllowSelfManagement: bool = ...
+        AllowSelfManagement: bool = ...,
     ) -> CreateUserProfileResultTypeDef:
         """
         Creates a new user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_user_profile)
         """
@@ -496,15 +495,15 @@
 
     async def describe_ecs_clusters(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeEcsClustersResultTypeDef:
         """
         Describes Amazon ECS clusters that are registered with a stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_ecs_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#describe_ecs_clusters)
         """
@@ -668,15 +667,15 @@
 
     async def describe_volumes(
         self,
         *,
         InstanceId: str = ...,
         StackId: str = ...,
         RaidArrayId: str = ...,
-        VolumeIds: Sequence[str] = ...
+        VolumeIds: Sequence[str] = ...,
     ) -> DescribeVolumesResultTypeDef:
         """
         Describes an instance's Amazon EBS volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_volumes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#describe_volumes)
         """
@@ -776,15 +775,15 @@
         *,
         StackId: str,
         Hostname: str = ...,
         PublicIp: str = ...,
         PrivateIp: str = ...,
         RsaPublicKey: str = ...,
         RsaPublicKeyFingerprint: str = ...,
-        InstanceIdentity: InstanceIdentityTypeDef = ...
+        InstanceIdentity: InstanceIdentityTypeDef = ...,
     ) -> RegisterInstanceResultTypeDef:
         """
         Registers instances that were created outside of AWS OpsWorks Stacks with a
         specified
         stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.register_instance)
@@ -813,15 +812,15 @@
 
     async def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
         UpScaling: AutoScalingThresholdsTypeDef = ...,
-        DownScaling: AutoScalingThresholdsTypeDef = ...
+        DownScaling: AutoScalingThresholdsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -829,15 +828,15 @@
     async def set_permission(
         self,
         *,
         StackId: str,
         IamUserArn: str,
         AllowSsh: bool = ...,
         AllowSudo: bool = ...,
-        Level: str = ...
+        Level: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_permission)
         """
@@ -931,15 +930,15 @@
         DataSources: Sequence[DataSourceTypeDef] = ...,
         Type: AppTypeType = ...,
         AppSource: SourceTypeDef = ...,
         Domains: Sequence[str] = ...,
         EnableSsl: bool = ...,
         SslConfiguration: SslConfigurationTypeDef = ...,
         Attributes: Mapping[AppAttributesKeysType, str] = ...,
-        Environment: Sequence[EnvironmentVariableTypeDef] = ...
+        Environment: Sequence[EnvironmentVariableTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_app)
         """
@@ -964,15 +963,15 @@
         Hostname: str = ...,
         Os: str = ...,
         AmiId: str = ...,
         SshKeyName: str = ...,
         Architecture: ArchitectureType = ...,
         InstallUpdatesOnBoot: bool = ...,
         EbsOptimized: bool = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_instance)
         """
@@ -992,15 +991,15 @@
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
         CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_layer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_layer)
         """
@@ -1041,30 +1040,30 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
         UseOpsworksSecurityGroups: bool = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_stack)
         """
 
     async def update_user_profile(
         self,
         *,
         IamUserArn: str,
         SshUsername: str = ...,
         SshPublicKey: str = ...,
-        AllowSelfManagement: bool = ...
+        AllowSelfManagement: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_user_profile)
         """
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/client.pyi` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         ClonePermissions: bool = ...,
         CloneAppIds: Sequence[str] = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> CloneStackResultTypeDef:
         """
         Creates a clone of a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.clone_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#clone_stack)
         """
@@ -231,15 +231,15 @@
         Description: str = ...,
         DataSources: Sequence[DataSourceTypeDef] = ...,
         AppSource: SourceTypeDef = ...,
         Domains: Sequence[str] = ...,
         EnableSsl: bool = ...,
         SslConfiguration: SslConfigurationTypeDef = ...,
         Attributes: Mapping[AppAttributesKeysType, str] = ...,
-        Environment: Sequence[EnvironmentVariableTypeDef] = ...
+        Environment: Sequence[EnvironmentVariableTypeDef] = ...,
     ) -> CreateAppResultTypeDef:
         """
         Creates an app for a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_app)
         """
@@ -249,15 +249,15 @@
         *,
         StackId: str,
         Command: DeploymentCommandTypeDef,
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
-        CustomJson: str = ...
+        CustomJson: str = ...,
     ) -> CreateDeploymentResultTypeDef:
         """
         Runs deployment or stack commands.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_deployment)
         """
@@ -278,15 +278,15 @@
         SubnetId: str = ...,
         Architecture: ArchitectureType = ...,
         RootDeviceType: RootDeviceTypeType = ...,
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         InstallUpdatesOnBoot: bool = ...,
         EbsOptimized: bool = ...,
         AgentVersion: str = ...,
-        Tenancy: str = ...
+        Tenancy: str = ...,
     ) -> CreateInstanceResultTypeDef:
         """
         Creates an instance in a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_instance)
         """
@@ -307,15 +307,15 @@
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
         CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_layer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_layer)
         """
@@ -337,30 +337,30 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> CreateStackResultTypeDef:
         """
         Creates a new stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_stack)
         """
 
     async def create_user_profile(
         self,
         *,
         IamUserArn: str,
         SshUsername: str = ...,
         SshPublicKey: str = ...,
-        AllowSelfManagement: bool = ...
+        AllowSelfManagement: bool = ...,
     ) -> CreateUserProfileResultTypeDef:
         """
         Creates a new user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_user_profile)
         """
@@ -492,15 +492,15 @@
 
     async def describe_ecs_clusters(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeEcsClustersResultTypeDef:
         """
         Describes Amazon ECS clusters that are registered with a stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_ecs_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#describe_ecs_clusters)
         """
@@ -664,15 +664,15 @@
 
     async def describe_volumes(
         self,
         *,
         InstanceId: str = ...,
         StackId: str = ...,
         RaidArrayId: str = ...,
-        VolumeIds: Sequence[str] = ...
+        VolumeIds: Sequence[str] = ...,
     ) -> DescribeVolumesResultTypeDef:
         """
         Describes an instance's Amazon EBS volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_volumes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#describe_volumes)
         """
@@ -772,15 +772,15 @@
         *,
         StackId: str,
         Hostname: str = ...,
         PublicIp: str = ...,
         PrivateIp: str = ...,
         RsaPublicKey: str = ...,
         RsaPublicKeyFingerprint: str = ...,
-        InstanceIdentity: InstanceIdentityTypeDef = ...
+        InstanceIdentity: InstanceIdentityTypeDef = ...,
     ) -> RegisterInstanceResultTypeDef:
         """
         Registers instances that were created outside of AWS OpsWorks Stacks with a
         specified
         stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.register_instance)
@@ -809,15 +809,15 @@
 
     async def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
         UpScaling: AutoScalingThresholdsTypeDef = ...,
-        DownScaling: AutoScalingThresholdsTypeDef = ...
+        DownScaling: AutoScalingThresholdsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -825,15 +825,15 @@
     async def set_permission(
         self,
         *,
         StackId: str,
         IamUserArn: str,
         AllowSsh: bool = ...,
         AllowSudo: bool = ...,
-        Level: str = ...
+        Level: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_permission)
         """
@@ -927,15 +927,15 @@
         DataSources: Sequence[DataSourceTypeDef] = ...,
         Type: AppTypeType = ...,
         AppSource: SourceTypeDef = ...,
         Domains: Sequence[str] = ...,
         EnableSsl: bool = ...,
         SslConfiguration: SslConfigurationTypeDef = ...,
         Attributes: Mapping[AppAttributesKeysType, str] = ...,
-        Environment: Sequence[EnvironmentVariableTypeDef] = ...
+        Environment: Sequence[EnvironmentVariableTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_app)
         """
@@ -960,15 +960,15 @@
         Hostname: str = ...,
         Os: str = ...,
         AmiId: str = ...,
         SshKeyName: str = ...,
         Architecture: ArchitectureType = ...,
         InstallUpdatesOnBoot: bool = ...,
         EbsOptimized: bool = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_instance)
         """
@@ -988,15 +988,15 @@
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
         CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_layer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_layer)
         """
@@ -1037,30 +1037,30 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
         UseOpsworksSecurityGroups: bool = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_stack)
         """
 
     async def update_user_profile(
         self,
         *,
         IamUserArn: str,
         SshUsername: str = ...,
         SshPublicKey: str = ...,
-        AllowSelfManagement: bool = ...
+        AllowSelfManagement: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#update_user_profile)
         """
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/literals.py` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/literals.py`

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
     "AppAttributesKeysType",
     "AppExistsWaiterName",
     "AppTypeType",
     "ArchitectureType",
     "AutoScalingTypeType",
     "CloudWatchLogsEncodingType",
@@ -47,15 +46,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AppAttributesKeysType = Literal[
     "AutoBundleOnDeploy", "AwsFlowRubySettings", "DocumentRoot", "RailsEnv"
 ]
 AppExistsWaiterName = Literal["app_exists"]
 AppTypeType = Literal["aws-flow-ruby", "java", "nodejs", "other", "php", "rails", "static"]
 ArchitectureType = Literal["i386", "x86_64"]
 AutoScalingTypeType = Literal["load", "timer"]
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/literals.pyi` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/paginator.py` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import DescribeEcsClustersResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("DescribeEcsClustersPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -48,13 +47,13 @@
     """
 
     def paginate(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEcsClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/paginators/#describeecsclusterspaginator)
         """
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/paginator.pyi` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     """
 
     def paginate(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEcsClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/paginators/#describeecsclusterspaginator)
         """
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/service_resource.py` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 else:
     from typing_extensions import Literal
 try:
     from boto3.resources.base import ResourceMeta
 except ImportError:
     from builtins import object as ResourceMeta
 
-
 __all__ = (
     "OpsWorksServiceResource",
     "Layer",
     "Stack",
     "StackSummary",
     "ServiceResourceStacksCollection",
     "StackLayersCollection",
@@ -202,14 +201,15 @@
     custom_recipes: Awaitable[RecipesResponseTypeDef]
     created_at: Awaitable[str]
     install_updates_on_boot: Awaitable[bool]
     use_ebs_optimized_instances: Awaitable[bool]
     lifecycle_event_configuration: Awaitable[LifecycleEventConfigurationResponseTypeDef]
     id: str
     stack: "Stack"
+    meta: Awaitable["OpsWorksResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Layer.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#layerdelete-method)
@@ -255,14 +255,15 @@
 
     name: Awaitable[str]
     arn: Awaitable[str]
     layers_count: Awaitable[int]
     apps_count: Awaitable[int]
     instances_count: Awaitable[InstancesCountResponseTypeDef]
     stack_id: str
+    meta: Awaitable["OpsWorksResourceMeta"]
 
     async def Stack(self) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.Stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#stacksummarystack-method)
@@ -326,16 +327,17 @@
     custom_cookbooks_source: Awaitable[SourceResponseTypeDef]
     default_ssh_key_name: Awaitable[str]
     created_at: Awaitable[str]
     default_root_device_type: Awaitable[RootDeviceTypeType]
     agent_version: Awaitable[str]
     id: str
     layers: StackLayersCollection
+    meta: Awaitable["OpsWorksResourceMeta"]
 
-    async def Summary(self) -> _StackSummary:
+    async def Summary(self) -> "_StackSummary":
         """
         Creates a StackSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.Summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#stacksummary-method)
         """
 
@@ -354,16 +356,16 @@
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
         CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
-    ) -> _Layer:
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
+    ) -> "_Layer":
         """
         Creates a layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.create_layer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#stackcreate_layer-method)
         """
 
@@ -416,31 +418,31 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/)
     """
 
     meta: "OpsWorksResourceMeta"
     stacks: ServiceResourceStacksCollection
 
-    async def Layer(self, id: str) -> _Layer:
+    async def Layer(self, id: str) -> "_Layer":
         """
         Creates a Layer resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Layer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#opsworksserviceresourcelayer-method)
         """
 
-    async def Stack(self, id: str) -> _Stack:
+    async def Stack(self, id: str) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#opsworksserviceresourcestack-method)
         """
 
-    async def StackSummary(self, stack_id: str) -> _StackSummary:
+    async def StackSummary(self, stack_id: str) -> "_StackSummary":
         """
         Creates a StackSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.StackSummary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#opsworksserviceresourcestacksummary-method)
         """
 
@@ -461,16 +463,16 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
-    ) -> _Stack:
+        AgentVersion: str = ...,
+    ) -> "_Stack":
         """
         Creates a new stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#opsworksserviceresourcecreate_stack-method)
         """
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/service_resource.pyi` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
     custom_recipes: Awaitable[RecipesResponseTypeDef]
     created_at: Awaitable[str]
     install_updates_on_boot: Awaitable[bool]
     use_ebs_optimized_instances: Awaitable[bool]
     lifecycle_event_configuration: Awaitable[LifecycleEventConfigurationResponseTypeDef]
     id: str
     stack: "Stack"
+    meta: Awaitable["OpsWorksResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Layer.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#layerdelete-method)
@@ -249,14 +250,15 @@
 
     name: Awaitable[str]
     arn: Awaitable[str]
     layers_count: Awaitable[int]
     apps_count: Awaitable[int]
     instances_count: Awaitable[InstancesCountResponseTypeDef]
     stack_id: str
+    meta: Awaitable["OpsWorksResourceMeta"]
 
     async def Stack(self) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.Stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#stacksummarystack-method)
@@ -318,16 +320,17 @@
     custom_cookbooks_source: Awaitable[SourceResponseTypeDef]
     default_ssh_key_name: Awaitable[str]
     created_at: Awaitable[str]
     default_root_device_type: Awaitable[RootDeviceTypeType]
     agent_version: Awaitable[str]
     id: str
     layers: StackLayersCollection
+    meta: Awaitable["OpsWorksResourceMeta"]
 
-    async def Summary(self) -> _StackSummary:
+    async def Summary(self) -> "_StackSummary":
         """
         Creates a StackSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.Summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#stacksummary-method)
         """
 
@@ -346,16 +349,16 @@
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
         CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
-    ) -> _Layer:
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
+    ) -> "_Layer":
         """
         Creates a layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.create_layer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#stackcreate_layer-method)
         """
 
@@ -405,31 +408,31 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/)
     """
 
     meta: "OpsWorksResourceMeta"
     stacks: ServiceResourceStacksCollection
 
-    async def Layer(self, id: str) -> _Layer:
+    async def Layer(self, id: str) -> "_Layer":
         """
         Creates a Layer resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Layer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#opsworksserviceresourcelayer-method)
         """
 
-    async def Stack(self, id: str) -> _Stack:
+    async def Stack(self, id: str) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#opsworksserviceresourcestack-method)
         """
 
-    async def StackSummary(self, stack_id: str) -> _StackSummary:
+    async def StackSummary(self, stack_id: str) -> "_StackSummary":
         """
         Creates a StackSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.StackSummary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#opsworksserviceresourcestacksummary-method)
         """
 
@@ -450,16 +453,16 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
-    ) -> _Stack:
+        AgentVersion: str = ...,
+    ) -> "_Stack":
         """
         Creates a new stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/service_resource/#opsworksserviceresourcecreate_stack-method)
         """
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/type_defs.py` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "StackConfigurationManagerTypeDef",
     "DataSourceTypeDef",
     "EnvironmentVariableTypeDef",
     "SourceTypeDef",
     "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/type_defs.pyi` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/waiter.py` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         AppIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.AppExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#appexistswaiter)
         """
 
 
@@ -74,15 +74,15 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         AppId: str = ...,
         DeploymentIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.DeploymentSuccessful.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#deploymentsuccessfulwaiter)
         """
 
 
@@ -94,15 +94,15 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceOnline.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#instanceonlinewaiter)
         """
 
 
@@ -114,15 +114,15 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceRegistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#instanceregisteredwaiter)
         """
 
 
@@ -134,15 +134,15 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceStopped.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#instancestoppedwaiter)
         """
 
 
@@ -154,13 +154,13 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceTerminated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#instanceterminatedwaiter)
         """
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks/waiter.pyi` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         AppIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.AppExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#appexistswaiter)
         """
 
 class DeploymentSuccessfulWaiter(AIOWaiter):
@@ -72,15 +72,15 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         AppId: str = ...,
         DeploymentIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.DeploymentSuccessful.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#deploymentsuccessfulwaiter)
         """
 
 class InstanceOnlineWaiter(AIOWaiter):
@@ -91,15 +91,15 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceOnline.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#instanceonlinewaiter)
         """
 
 class InstanceRegisteredWaiter(AIOWaiter):
@@ -110,15 +110,15 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceRegistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#instanceregisteredwaiter)
         """
 
 class InstanceStoppedWaiter(AIOWaiter):
@@ -129,15 +129,15 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceStopped.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#instancestoppedwaiter)
         """
 
 class InstanceTerminatedWaiter(AIOWaiter):
@@ -148,13 +148,13 @@
 
     async def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceTerminated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/waiters/#instanceterminatedwaiter)
         """
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/PKG-INFO` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworks
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpsWorks 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpsWorks 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/
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
 
 <a id="types-aiobotocore-opsworks"></a>
 
 # types-aiobotocore-opsworks
 
 [![PyPI - types-aiobotocore-opsworks](https://img.shields.io/pypi/v/types-aiobotocore-opsworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworks)](https://pepy.tech/project/types-aiobotocore-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorks 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[aiobotocore.OpsWorks 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [types-aiobotocore-opsworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opsworks-2.9.0/types_aiobotocore_opsworks.egg-info/SOURCES.txt` & `types-aiobotocore-opsworks-2.9.1/types_aiobotocore_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

