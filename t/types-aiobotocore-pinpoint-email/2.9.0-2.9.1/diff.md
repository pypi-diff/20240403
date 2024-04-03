# Comparing `tmp/types-aiobotocore-pinpoint-email-2.9.0.tar.gz` & `tmp/types-aiobotocore-pinpoint-email-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pinpoint-email-2.9.0.tar", last modified: Wed Dec 13 20:00:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-pinpoint-email-2.9.1.tar", last modified: Thu Jan 18 01:21:29 2024, max compression
```

## Comparing `types-aiobotocore-pinpoint-email-2.9.0.tar` & `types-aiobotocore-pinpoint-email-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:08.965324 types-aiobotocore-pinpoint-email-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14087 2023-12-13 20:00:08.965324 types-aiobotocore-pinpoint-email-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:08.965324 types-aiobotocore-pinpoint-email-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:08.965324 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35209 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35205 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30078 2023-12-13 19:51:48.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30077 2023-12-13 19:51:46.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:08.965324 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14087 2023-12-13 20:00:08.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:08.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:08.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:08.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:08.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:08.000000 types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.349121 types-aiobotocore-pinpoint-email-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14107 2024-01-18 01:21:29.349121 types-aiobotocore-pinpoint-email-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:29.349121 types-aiobotocore-pinpoint-email-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.349121 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35217 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35214 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30077 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30077 2024-01-18 01:13:24.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.349121 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14107 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/LICENSE` & `types-aiobotocore-pinpoint-email-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/PKG-INFO` & `types-aiobotocore-pinpoint-email-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-email
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PinpointEmail 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PinpointEmail 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/
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
 
 <a id="types-aiobotocore-pinpoint-email"></a>
 
 # types-aiobotocore-pinpoint-email
 
 [![PyPI - types-aiobotocore-pinpoint-email](https://img.shields.io/pypi/v/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-email)](https://pepy.tech/project/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [types-aiobotocore-pinpoint-email docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/README.md` & `types-aiobotocore-pinpoint-email-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-email)](https://pepy.tech/project/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [types-aiobotocore-pinpoint-email docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/setup.py` & `types-aiobotocore-pinpoint-email-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pinpoint-email",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PinpointEmail 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PinpointEmail 2.9.1 service generated with"
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
     keywords="aiobotocore pinpoint-email type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_pinpoint_email": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/__init__.py` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListDedicatedIpPoolsPaginator,
     ListDeliverabilityTestReportsPaginator,
     ListEmailIdentitiesPaginator,
 )
 
 Client = PinpointEmailClient
 
-
 __all__ = (
     "Client",
     "GetDedicatedIpsPaginator",
     "ListConfigurationSetsPaginator",
     "ListDedicatedIpPoolsPaginator",
     "ListDeliverabilityTestReportsPaginator",
     "ListEmailIdentitiesPaginator",
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/__init__.pyi` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/__main__.py` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PinpointEmail 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PinpointEmail 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail\nOther"
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

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/client.py` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PinpointEmailClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -131,29 +130,29 @@
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
         ReputationOptions: ReputationOptionsTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_configuration_set)
         """
 
     async def create_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef
+        EventDestination: EventDestinationDefinitionTypeDef,
     ) -> Dict[str, Any]:
         """
         Create an event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_configuration_set_event_destination)
         """
@@ -170,15 +169,15 @@
 
     async def create_deliverability_test_report(
         self,
         *,
         FromEmailAddress: str,
         Content: EmailContentTypeDef,
         ReportName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDeliverabilityTestReportResponseTypeDef:
         """
         Create a new predictive inbox placement test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_deliverability_test_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_deliverability_test_report)
         """
@@ -402,15 +401,15 @@
     async def list_domain_deliverability_campaigns(
         self,
         *,
         StartDate: TimestampTypeDef,
         EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListDomainDeliverabilityCampaignsResponseTypeDef:
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_domain_deliverability_campaigns)
@@ -460,15 +459,15 @@
         """
 
     async def put_configuration_set_delivery_options(
         self,
         *,
         ConfigurationSetName: str,
         TlsPolicy: TlsPolicyType = ...,
-        SendingPoolName: str = ...
+        SendingPoolName: str = ...,
     ) -> Dict[str, Any]:
         """
         Associate a configuration set with a dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_delivery_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_delivery_options)
         """
@@ -530,15 +529,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_dedicated_ip_warmup_attributes)
         """
 
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard for your Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_deliverability_dashboard_option)
         """
@@ -564,15 +563,15 @@
         """
 
     async def put_email_identity_mail_from_attributes(
         self,
         *,
         EmailIdentity: str,
         MailFromDomain: str = ...,
-        BehaviorOnMxFailure: BehaviorOnMxFailureType = ...
+        BehaviorOnMxFailure: BehaviorOnMxFailureType = ...,
     ) -> Dict[str, Any]:
         """
         Used to enable or disable the custom Mail-From domain configuration for an
         email
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_email_identity_mail_from_attributes)
@@ -584,15 +583,15 @@
         *,
         Destination: DestinationTypeDef,
         Content: EmailContentTypeDef,
         FromEmailAddress: str = ...,
         ReplyToAddresses: Sequence[str] = ...,
         FeedbackForwardingEmailAddress: str = ...,
         EmailTags: Sequence[MessageTagTypeDef] = ...,
-        ConfigurationSetName: str = ...
+        ConfigurationSetName: str = ...,
     ) -> SendEmailResponseTypeDef:
         """
         Sends an email message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.send_email)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#send_email)
         """
@@ -614,15 +613,15 @@
         """
 
     async def update_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef
+        EventDestination: EventDestinationDefinitionTypeDef,
     ) -> Dict[str, Any]:
         """
         Update the configuration of an event destination for a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#update_configuration_set_event_destination)
         """
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/client.pyi` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -127,29 +127,29 @@
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
         ReputationOptions: ReputationOptionsTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_configuration_set)
         """
 
     async def create_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef
+        EventDestination: EventDestinationDefinitionTypeDef,
     ) -> Dict[str, Any]:
         """
         Create an event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_configuration_set_event_destination)
         """
@@ -166,15 +166,15 @@
 
     async def create_deliverability_test_report(
         self,
         *,
         FromEmailAddress: str,
         Content: EmailContentTypeDef,
         ReportName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDeliverabilityTestReportResponseTypeDef:
         """
         Create a new predictive inbox placement test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_deliverability_test_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_deliverability_test_report)
         """
@@ -398,15 +398,15 @@
     async def list_domain_deliverability_campaigns(
         self,
         *,
         StartDate: TimestampTypeDef,
         EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListDomainDeliverabilityCampaignsResponseTypeDef:
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_domain_deliverability_campaigns)
@@ -456,15 +456,15 @@
         """
 
     async def put_configuration_set_delivery_options(
         self,
         *,
         ConfigurationSetName: str,
         TlsPolicy: TlsPolicyType = ...,
-        SendingPoolName: str = ...
+        SendingPoolName: str = ...,
     ) -> Dict[str, Any]:
         """
         Associate a configuration set with a dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_delivery_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_delivery_options)
         """
@@ -526,15 +526,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_dedicated_ip_warmup_attributes)
         """
 
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard for your Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_deliverability_dashboard_option)
         """
@@ -560,15 +560,15 @@
         """
 
     async def put_email_identity_mail_from_attributes(
         self,
         *,
         EmailIdentity: str,
         MailFromDomain: str = ...,
-        BehaviorOnMxFailure: BehaviorOnMxFailureType = ...
+        BehaviorOnMxFailure: BehaviorOnMxFailureType = ...,
     ) -> Dict[str, Any]:
         """
         Used to enable or disable the custom Mail-From domain configuration for an
         email
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_email_identity_mail_from_attributes)
@@ -580,15 +580,15 @@
         *,
         Destination: DestinationTypeDef,
         Content: EmailContentTypeDef,
         FromEmailAddress: str = ...,
         ReplyToAddresses: Sequence[str] = ...,
         FeedbackForwardingEmailAddress: str = ...,
         EmailTags: Sequence[MessageTagTypeDef] = ...,
-        ConfigurationSetName: str = ...
+        ConfigurationSetName: str = ...,
     ) -> SendEmailResponseTypeDef:
         """
         Sends an email message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.send_email)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#send_email)
         """
@@ -610,15 +610,15 @@
         """
 
     async def update_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
-        EventDestination: EventDestinationDefinitionTypeDef
+        EventDestination: EventDestinationDefinitionTypeDef,
     ) -> Dict[str, Any]:
         """
         Update the configuration of an event destination for a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#update_configuration_set_event_destination)
         """
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/literals.py` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/literals.py`

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
     "BehaviorOnMxFailureType",
     "DeliverabilityDashboardAccountStatusType",
     "DeliverabilityTestStatusType",
     "DimensionValueSourceType",
     "DkimStatusType",
     "EventTypeType",
@@ -39,15 +38,14 @@
     "PinpointEmailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BehaviorOnMxFailureType = Literal["REJECT_MESSAGE", "USE_DEFAULT_VALUE"]
 DeliverabilityDashboardAccountStatusType = Literal["ACTIVE", "DISABLED", "PENDING_EXPIRATION"]
 DeliverabilityTestStatusType = Literal["COMPLETED", "IN_PROGRESS"]
 DimensionValueSourceType = Literal["EMAIL_HEADER", "LINK_TAG", "MESSAGE_TAG"]
 DkimStatusType = Literal["FAILED", "NOT_STARTED", "PENDING", "SUCCESS", "TEMPORARY_FAILURE"]
 EventTypeType = Literal[
     "BOUNCE", "CLICK", "COMPLAINT", "DELIVERY", "OPEN", "REJECT", "RENDERING_FAILURE", "SEND"
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/literals.pyi` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/paginator.py` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "GetDedicatedIpsPaginator",
     "ListConfigurationSetsPaginator",
     "ListDedicatedIpPoolsPaginator",
     "ListDeliverabilityTestReportsPaginator",
     "ListEmailIdentitiesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/paginator.pyi` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/type_defs.py` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlacklistEntryTypeDef",
     "BlobTypeDef",
     "ContentTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "SendingOptionsTypeDef",
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email/type_defs.pyi` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-email
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PinpointEmail 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PinpointEmail 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/
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
 
 <a id="types-aiobotocore-pinpoint-email"></a>
 
 # types-aiobotocore-pinpoint-email
 
 [![PyPI - types-aiobotocore-pinpoint-email](https://img.shields.io/pypi/v/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-email)](https://pepy.tech/project/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [types-aiobotocore-pinpoint-email docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-email-2.9.0/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt` & `types-aiobotocore-pinpoint-email-2.9.1/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

