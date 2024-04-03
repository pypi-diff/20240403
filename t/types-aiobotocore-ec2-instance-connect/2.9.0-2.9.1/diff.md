# Comparing `tmp/types-aiobotocore-ec2-instance-connect-2.9.0.tar.gz` & `tmp/types-aiobotocore-ec2-instance-connect-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.9.0.tar", last modified: Wed Dec 13 19:59:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.9.1.tar", last modified: Thu Jan 18 01:20:35 2024, max compression
```

## Comparing `types-aiobotocore-ec2-instance-connect-2.9.0.tar` & `types-aiobotocore-ec2-instance-connect-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:10.573801 types-aiobotocore-ec2-instance-connect-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12926 2023-12-13 19:59:10.573801 types-aiobotocore-ec2-instance-connect-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:10.573801 types-aiobotocore-ec2-instance-connect-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:10.573801 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2023-12-13 19:45:22.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2023-12-13 19:45:22.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2023-12-13 19:45:22.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-12-13 19:45:22.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:21.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:10.573801 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12926 2023-12-13 19:59:10.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-13 19:59:10.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:10.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:10.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:10.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-13 19:59:10.000000 types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.681366 types-aiobotocore-ec2-instance-connect-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-01-18 01:20:35.681366 types-aiobotocore-ec2-instance-connect-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:35.681366 types-aiobotocore-ec2-instance-connect-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.681366 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:18.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.681366 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-01-18 01:20:35.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-18 01:20:35.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:35.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:35.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:35.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-18 01:20:35.000000 types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/LICENSE` & `types-aiobotocore-ec2-instance-connect-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
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
 
 <a id="types-aiobotocore-ec2-instance-connect"></a>
 
 # types-aiobotocore-ec2-instance-connect
 
 [![PyPI - types-aiobotocore-ec2-instance-connect](https://img.shields.io/pypi/v/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/README.md` & `types-aiobotocore-ec2-instance-connect-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/setup.py` & `types-aiobotocore-ec2-instance-connect-2.9.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ec2-instance-connect",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ec2_instance_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EC2InstanceConnect 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.EC2InstanceConnect 2.9.1 service generated with"
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
         "aiobotocore ec2-instance-connect type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ec2_instance_connect": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/__init__.py` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import EC2InstanceConnectClient
 
 Client = EC2InstanceConnectClient
 
-
 __all__ = ("Client", "EC2InstanceConnectClient")
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/__init__.pyi` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/__main__.py` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EC2InstanceConnect 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EC2InstanceConnect 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect\nOther"
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

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/client.py` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     async def send_ssh_public_key(
         self,
         *,
         InstanceId: str,
         InstanceOSUser: str,
         SSHPublicKey: str,
-        AvailabilityZone: str = ...
+        AvailabilityZone: str = ...,
     ) -> SendSSHPublicKeyResponseTypeDef:
         """
         Pushes an SSH public key to the specified EC2 instance for use by the specified
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.send_ssh_public_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/client/#send_ssh_public_key)
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/client.pyi` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     async def send_ssh_public_key(
         self,
         *,
         InstanceId: str,
         InstanceOSUser: str,
         SSHPublicKey: str,
-        AvailabilityZone: str = ...
+        AvailabilityZone: str = ...,
     ) -> SendSSHPublicKeyResponseTypeDef:
         """
         Pushes an SSH public key to the specified EC2 instance for use by the specified
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.send_ssh_public_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/client/#send_ssh_public_key)
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/literals.py` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EC2InstanceConnectServiceName", "ServiceName", "ResourceServiceName")
 
-
 EC2InstanceConnectServiceName = Literal["ec2-instance-connect"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/literals.pyi` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/type_defs.py` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "SendSSHPublicKeyRequestRequestTypeDef",
     "SendSerialConsoleSSHPublicKeyRequestRequestTypeDef",
     "SendSSHPublicKeyResponseTypeDef",
     "SendSerialConsoleSSHPublicKeyResponseTypeDef",
 )
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect/type_defs.pyi` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
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
 
 <a id="types-aiobotocore-ec2-instance-connect"></a>
 
 # types-aiobotocore-ec2-instance-connect
 
 [![PyPI - types-aiobotocore-ec2-instance-connect](https://img.shields.io/pypi/v/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.9.0/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt` & `types-aiobotocore-ec2-instance-connect-2.9.1/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

