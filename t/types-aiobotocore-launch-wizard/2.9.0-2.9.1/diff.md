# Comparing `tmp/types-aiobotocore-launch-wizard-2.9.0.tar.gz` & `tmp/types-aiobotocore-launch-wizard-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-launch-wizard-2.9.0.tar", last modified: Wed Dec 13 19:59:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-launch-wizard-2.9.1.tar", last modified: Thu Jan 18 01:21:05 2024, max compression
```

## Comparing `types-aiobotocore-launch-wizard-2.9.0.tar` & `types-aiobotocore-launch-wizard-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:43.337545 types-aiobotocore-launch-wizard-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13832 2023-12-13 19:59:43.337545 types-aiobotocore-launch-wizard-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12246 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:43.337545 types-aiobotocore-launch-wizard-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:43.337545 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11070 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:50.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:43.337545 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13832 2023-12-13 19:59:43.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 19:59:43.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:43.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:43.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:43.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:59:43.000000 types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.989228 types-aiobotocore-launch-wizard-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-01-18 01:21:05.989228 types-aiobotocore-launch-wizard-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:05.989228 types-aiobotocore-launch-wizard-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.985228 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:37.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.989228 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-01-18 01:21:05.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:21:05.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:05.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:05.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:05.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:05.000000 types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/LICENSE` & `types-aiobotocore-launch-wizard-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-launch-wizard-2.9.0/PKG-INFO` & `types-aiobotocore-launch-wizard-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-launch-wizard
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LaunchWizard 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LaunchWizard 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/
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
 
 <a id="types-aiobotocore-launch-wizard"></a>
 
 # types-aiobotocore-launch-wizard
 
 [![PyPI - types-aiobotocore-launch-wizard](https://img.shields.io/pypi/v/types-aiobotocore-launch-wizard.svg?color=blue)](https://pypi.org/project/types-aiobotocore-launch-wizard)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-launch-wizard.svg?color=blue)](https://pypi.org/project/types-aiobotocore-launch-wizard)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-launch-wizard)](https://pepy.tech/project/types-aiobotocore-launch-wizard)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LaunchWizard 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
+[aiobotocore.LaunchWizard 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
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
 [types-aiobotocore-launch-wizard docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/README.md` & `types-aiobotocore-launch-wizard-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-launch-wizard.svg?color=blue)](https://pypi.org/project/types-aiobotocore-launch-wizard)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-launch-wizard)](https://pepy.tech/project/types-aiobotocore-launch-wizard)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LaunchWizard 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
+[aiobotocore.LaunchWizard 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
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
 [types-aiobotocore-launch-wizard docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/setup.py` & `types-aiobotocore-launch-wizard-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-launch-wizard",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_launch_wizard"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LaunchWizard 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LaunchWizard 2.9.1 service generated with"
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
     keywords="aiobotocore launch-wizard type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_launch_wizard": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/__init__.py` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListDeploymentsPaginator,
     ListWorkloadDeploymentPatternsPaginator,
     ListWorkloadsPaginator,
 )
 
 Client = LaunchWizardClient
 
-
 __all__ = (
     "Client",
     "LaunchWizardClient",
     "ListDeploymentEventsPaginator",
     "ListDeploymentsPaginator",
     "ListWorkloadDeploymentPatternsPaginator",
     "ListWorkloadsPaginator",
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/__init__.pyi` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/__main__.py` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LaunchWizard 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LaunchWizard 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard\nOther"
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

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/client.py` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LaunchWizardClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -100,15 +99,15 @@
     async def create_deployment(
         self,
         *,
         deploymentPatternName: str,
         name: str,
         specifications: Mapping[str, str],
         workloadName: str,
-        dryRun: bool = ...
+        dryRun: bool = ...,
     ) -> CreateDeploymentOutputTypeDef:
         """
         Creates a deployment for the given workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/client/#create_deployment)
         """
@@ -162,15 +161,15 @@
         """
 
     async def list_deployments(
         self,
         *,
         filters: Sequence[DeploymentFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsOutputTypeDef:
         """
         Lists the deployments that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/client/#list_deployments)
         """
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/client.pyi` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     async def create_deployment(
         self,
         *,
         deploymentPatternName: str,
         name: str,
         specifications: Mapping[str, str],
         workloadName: str,
-        dryRun: bool = ...
+        dryRun: bool = ...,
     ) -> CreateDeploymentOutputTypeDef:
         """
         Creates a deployment for the given workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/client/#create_deployment)
         """
@@ -158,15 +158,15 @@
         """
 
     async def list_deployments(
         self,
         *,
         filters: Sequence[DeploymentFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsOutputTypeDef:
         """
         Lists the deployments that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/client/#list_deployments)
         """
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/literals.py` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/literals.py`

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
     "DeploymentFilterKeyType",
     "DeploymentStatusType",
     "EventStatusType",
     "ListDeploymentEventsPaginatorName",
     "ListDeploymentsPaginatorName",
     "ListWorkloadDeploymentPatternsPaginatorName",
@@ -32,15 +31,14 @@
     "WorkloadStatusType",
     "LaunchWizardServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 DeploymentFilterKeyType = Literal["DEPLOYMENT_STATUS", "WORKLOAD_NAME"]
 DeploymentStatusType = Literal[
     "COMPLETED",
     "CREATING",
     "DELETED",
     "DELETE_FAILED",
     "DELETE_INITIATING",
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/literals.pyi` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/paginator.py` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "ListDeploymentEventsPaginator",
     "ListDeploymentsPaginator",
     "ListWorkloadDeploymentPatternsPaginator",
     "ListWorkloadsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -80,15 +79,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[DeploymentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/paginators/#listdeploymentspaginator)
         """
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/paginator.pyi` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[DeploymentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/paginators/#listdeploymentspaginator)
         """
 
 class ListWorkloadDeploymentPatternsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/type_defs.py` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateDeploymentInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteDeploymentInputRequestTypeDef",
     "DeploymentDataSummaryTypeDef",
     "DeploymentDataTypeDef",
     "DeploymentEventDataSummaryTypeDef",
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard/type_defs.pyi` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/PKG-INFO` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-launch-wizard
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LaunchWizard 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LaunchWizard 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/
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
 
 <a id="types-aiobotocore-launch-wizard"></a>
 
 # types-aiobotocore-launch-wizard
 
 [![PyPI - types-aiobotocore-launch-wizard](https://img.shields.io/pypi/v/types-aiobotocore-launch-wizard.svg?color=blue)](https://pypi.org/project/types-aiobotocore-launch-wizard)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-launch-wizard.svg?color=blue)](https://pypi.org/project/types-aiobotocore-launch-wizard)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-launch-wizard)](https://pepy.tech/project/types-aiobotocore-launch-wizard)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LaunchWizard 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
+[aiobotocore.LaunchWizard 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
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
 [types-aiobotocore-launch-wizard docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_launch_wizard/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-launch-wizard-2.9.0/types_aiobotocore_launch_wizard.egg-info/SOURCES.txt` & `types-aiobotocore-launch-wizard-2.9.1/types_aiobotocore_launch_wizard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

