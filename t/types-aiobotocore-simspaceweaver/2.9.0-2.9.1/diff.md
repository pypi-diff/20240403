# Comparing `tmp/types-aiobotocore-simspaceweaver-2.9.0.tar.gz` & `tmp/types-aiobotocore-simspaceweaver-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-simspaceweaver-2.9.0.tar", last modified: Wed Dec 13 20:00:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-simspaceweaver-2.9.1.tar", last modified: Thu Jan 18 01:21:50 2024, max compression
```

## Comparing `types-aiobotocore-simspaceweaver-2.9.0.tar` & `types-aiobotocore-simspaceweaver-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.497120 types-aiobotocore-simspaceweaver-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2023-12-13 20:00:32.497120 types-aiobotocore-simspaceweaver-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:32.497120 types-aiobotocore-simspaceweaver-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.497120 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13284 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:34.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.497120 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2023-12-13 20:00:32.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-13 20:00:32.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:32.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:32.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:32.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:32.000000 types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.717026 types-aiobotocore-simspaceweaver-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-01-18 01:21:50.717026 types-aiobotocore-simspaceweaver-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:50.717026 types-aiobotocore-simspaceweaver-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.717026 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-01-18 01:18:06.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-01-18 01:18:06.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:02.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.717026 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-01-18 01:21:50.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-18 01:21:50.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:50.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:50.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:50.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:50.000000 types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/LICENSE` & `types-aiobotocore-simspaceweaver-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/PKG-INFO` & `types-aiobotocore-simspaceweaver-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-simspaceweaver
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
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
 
 <a id="types-aiobotocore-simspaceweaver"></a>
 
 # types-aiobotocore-simspaceweaver
 
 [![PyPI - types-aiobotocore-simspaceweaver](https://img.shields.io/pypi/v/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimSpaceWeaver 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[aiobotocore.SimSpaceWeaver 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/README.md` & `types-aiobotocore-simspaceweaver-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimSpaceWeaver 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[aiobotocore.SimSpaceWeaver 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/setup.py` & `types-aiobotocore-simspaceweaver-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-simspaceweaver",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_simspaceweaver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SimSpaceWeaver 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SimSpaceWeaver 2.9.1 service generated with"
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
     keywords="aiobotocore simspaceweaver type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_simspaceweaver": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/__main__.py` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SimSpaceWeaver 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SimSpaceWeaver 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver\nOther"
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

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/client.py` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         self,
         *,
         Domain: str,
         Name: str,
         Simulation: str,
         ClientToken: str = ...,
         Description: str = ...,
-        LaunchOverrides: LaunchOverridesTypeDef = ...
+        LaunchOverrides: LaunchOverridesTypeDef = ...,
     ) -> StartAppOutputTypeDef:
         """
         Starts a custom app with the configuration specified in the simulation schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/client/#start_app)
         """
@@ -207,15 +207,15 @@
         Name: str,
         RoleArn: str,
         ClientToken: str = ...,
         Description: str = ...,
         MaximumDuration: str = ...,
         SchemaS3Location: S3LocationTypeDef = ...,
         SnapshotS3Location: S3LocationTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> StartSimulationOutputTypeDef:
         """
         Starts a simulation with the given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_simulation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/client/#start_simulation)
         """
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/client.pyi` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         self,
         *,
         Domain: str,
         Name: str,
         Simulation: str,
         ClientToken: str = ...,
         Description: str = ...,
-        LaunchOverrides: LaunchOverridesTypeDef = ...
+        LaunchOverrides: LaunchOverridesTypeDef = ...,
     ) -> StartAppOutputTypeDef:
         """
         Starts a custom app with the configuration specified in the simulation schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/client/#start_app)
         """
@@ -204,15 +204,15 @@
         Name: str,
         RoleArn: str,
         ClientToken: str = ...,
         Description: str = ...,
         MaximumDuration: str = ...,
         SchemaS3Location: S3LocationTypeDef = ...,
         SnapshotS3Location: S3LocationTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> StartSimulationOutputTypeDef:
         """
         Starts a simulation with the given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_simulation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/client/#start_simulation)
         """
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/literals.py` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ClockStatusType",
     "ClockTargetStatusType",
     "LifecycleManagementStrategyType",
     "SimulationAppStatusType",
     "SimulationAppTargetStatusType",
     "SimulationStatusType",
     "SimulationTargetStatusType",
     "SimSpaceWeaverServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ClockStatusType = Literal["STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"]
 ClockTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 LifecycleManagementStrategyType = Literal[
     "ByRequest", "BySpatialSubdivision", "PerWorker", "Unknown"
 ]
 SimulationAppStatusType = Literal["ERROR", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"]
 SimulationAppTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/literals.pyi` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/type_defs.py` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
     "LaunchOverridesTypeDef",
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver/type_defs.pyi` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-simspaceweaver
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
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
 
 <a id="types-aiobotocore-simspaceweaver"></a>
 
 # types-aiobotocore-simspaceweaver
 
 [![PyPI - types-aiobotocore-simspaceweaver](https://img.shields.io/pypi/v/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimSpaceWeaver 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[aiobotocore.SimSpaceWeaver 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-simspaceweaver-2.9.0/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt` & `types-aiobotocore-simspaceweaver-2.9.1/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

