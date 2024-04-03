# Comparing `tmp/types-aiobotocore-ssm-incidents-2.9.0.tar.gz` & `tmp/types-aiobotocore-ssm-incidents-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-incidents-2.9.0.tar", last modified: Wed Dec 13 20:00:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-incidents-2.9.1.tar", last modified: Thu Jan 18 01:21:53 2024, max compression
```

## Comparing `types-aiobotocore-ssm-incidents-2.9.0.tar` & `types-aiobotocore-ssm-incidents-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.509095 types-aiobotocore-ssm-incidents-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15300 2023-12-13 20:00:35.509095 types-aiobotocore-ssm-incidents-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:35.509095 types-aiobotocore-ssm-incidents-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.509095 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29513 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    29509 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10710 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28268 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28267 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.509095 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15300 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.401013 types-aiobotocore-ssm-incidents-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-01-18 01:21:53.401013 types-aiobotocore-ssm-incidents-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:53.401013 types-aiobotocore-ssm-incidents-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.401013 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29522 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29519 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28267 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28267 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.401013 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/LICENSE` & `types-aiobotocore-ssm-incidents-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/PKG-INFO` & `types-aiobotocore-ssm-incidents-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-incidents
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSMIncidents 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSMIncidents 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/
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
 
 <a id="types-aiobotocore-ssm-incidents"></a>
 
 # types-aiobotocore-ssm-incidents
 
 [![PyPI - types-aiobotocore-ssm-incidents](https://img.shields.io/pypi/v/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-incidents)](https://pepy.tech/project/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [types-aiobotocore-ssm-incidents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/README.md` & `types-aiobotocore-ssm-incidents-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-incidents)](https://pepy.tech/project/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [types-aiobotocore-ssm-incidents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/setup.py` & `types-aiobotocore-ssm-incidents-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-incidents",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSMIncidents 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SSMIncidents 2.9.1 service generated with"
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
     keywords="aiobotocore ssm-incidents type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ssm_incidents": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/__init__.py` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     ListResponsePlansPaginator,
     ListTimelineEventsPaginator,
 )
 from .waiter import WaitForReplicationSetActiveWaiter, WaitForReplicationSetDeletedWaiter
 
 Client = SSMIncidentsClient
 
-
 __all__ = (
     "Client",
     "GetResourcePoliciesPaginator",
     "ListIncidentFindingsPaginator",
     "ListIncidentRecordsPaginator",
     "ListRelatedItemsPaginator",
     "ListReplicationSetsPaginator",
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/__init__.pyi` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/__main__.py` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSMIncidents 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SSMIncidents 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
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

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/client.py` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 from .waiter import WaitForReplicationSetActiveWaiter, WaitForReplicationSetDeletedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSMIncidentsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -140,15 +139,15 @@
         """
 
     async def create_replication_set(
         self,
         *,
         regions: Mapping[str, RegionMapInputValueTypeDef],
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateReplicationSetOutputTypeDef:
         """
         A replication set replicates and encrypts your data to the provided Regions
         with the provided KMS
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_replication_set)
@@ -162,15 +161,15 @@
         name: str,
         actions: Sequence[ActionTypeDef] = ...,
         chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         integrations: Sequence[IntegrationTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateResponsePlanOutputTypeDef:
         """
         Creates a response plan that automates the initial response to incidents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_response_plan)
         """
@@ -179,15 +178,15 @@
         self,
         *,
         eventData: str,
         eventTime: TimestampTypeDef,
         eventType: str,
         incidentRecordArn: str,
         clientToken: str = ...,
-        eventReferences: Sequence[EventReferenceTypeDef] = ...
+        eventReferences: Sequence[EventReferenceTypeDef] = ...,
     ) -> CreateTimelineEventOutputTypeDef:
         """
         Creates a custom timeline event on the incident details page of an incident
         record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_timeline_event)
@@ -361,15 +360,15 @@
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["EVENT_TIME"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListTimelineEventsOutputTypeDef:
         """
         Lists timeline events for the specified incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_timeline_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_timeline_events)
         """
@@ -388,15 +387,15 @@
         self,
         *,
         responsePlanArn: str,
         clientToken: str = ...,
         impact: int = ...,
         relatedItems: Sequence[RelatedItemTypeDef] = ...,
         title: str = ...,
-        triggerDetails: TriggerDetailsTypeDef = ...
+        triggerDetails: TriggerDetailsTypeDef = ...,
     ) -> StartIncidentOutputTypeDef:
         """
         Used to start an incident from CloudWatch alarms, EventBridge events, or
         manually.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.start_incident)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#start_incident)
@@ -436,43 +435,43 @@
         arn: str,
         chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         impact: int = ...,
         notificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         status: IncidentRecordStatusType = ...,
         summary: str = ...,
-        title: str = ...
+        title: str = ...,
     ) -> Dict[str, Any]:
         """
         Update the details of an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_incident_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_incident_record)
         """
 
     async def update_related_items(
         self,
         *,
         incidentRecordArn: str,
         relatedItemsUpdate: RelatedItemsUpdateTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Add or remove related items from the related items tab of an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_related_items)
         """
 
     async def update_replication_set(
         self,
         *,
         actions: Sequence[UpdateReplicationSetActionTypeDef],
         arn: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Add or delete Regions from your replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_replication_set)
         """
@@ -488,15 +487,15 @@
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
         incidentTemplateTags: Mapping[str, str] = ...,
         incidentTemplateTitle: str = ...,
-        integrations: Sequence[IntegrationTypeDef] = ...
+        integrations: Sequence[IntegrationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_response_plan)
         """
@@ -506,15 +505,15 @@
         *,
         eventId: str,
         incidentRecordArn: str,
         clientToken: str = ...,
         eventData: str = ...,
         eventReferences: Sequence[EventReferenceTypeDef] = ...,
         eventTime: TimestampTypeDef = ...,
-        eventType: str = ...
+        eventType: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a timeline event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_timeline_event)
         """
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/client.pyi` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         """
 
     async def create_replication_set(
         self,
         *,
         regions: Mapping[str, RegionMapInputValueTypeDef],
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateReplicationSetOutputTypeDef:
         """
         A replication set replicates and encrypts your data to the provided Regions
         with the provided KMS
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_replication_set)
@@ -158,15 +158,15 @@
         name: str,
         actions: Sequence[ActionTypeDef] = ...,
         chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         integrations: Sequence[IntegrationTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateResponsePlanOutputTypeDef:
         """
         Creates a response plan that automates the initial response to incidents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_response_plan)
         """
@@ -175,15 +175,15 @@
         self,
         *,
         eventData: str,
         eventTime: TimestampTypeDef,
         eventType: str,
         incidentRecordArn: str,
         clientToken: str = ...,
-        eventReferences: Sequence[EventReferenceTypeDef] = ...
+        eventReferences: Sequence[EventReferenceTypeDef] = ...,
     ) -> CreateTimelineEventOutputTypeDef:
         """
         Creates a custom timeline event on the incident details page of an incident
         record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_timeline_event)
@@ -357,15 +357,15 @@
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["EVENT_TIME"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListTimelineEventsOutputTypeDef:
         """
         Lists timeline events for the specified incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_timeline_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_timeline_events)
         """
@@ -384,15 +384,15 @@
         self,
         *,
         responsePlanArn: str,
         clientToken: str = ...,
         impact: int = ...,
         relatedItems: Sequence[RelatedItemTypeDef] = ...,
         title: str = ...,
-        triggerDetails: TriggerDetailsTypeDef = ...
+        triggerDetails: TriggerDetailsTypeDef = ...,
     ) -> StartIncidentOutputTypeDef:
         """
         Used to start an incident from CloudWatch alarms, EventBridge events, or
         manually.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.start_incident)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#start_incident)
@@ -432,43 +432,43 @@
         arn: str,
         chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         impact: int = ...,
         notificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         status: IncidentRecordStatusType = ...,
         summary: str = ...,
-        title: str = ...
+        title: str = ...,
     ) -> Dict[str, Any]:
         """
         Update the details of an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_incident_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_incident_record)
         """
 
     async def update_related_items(
         self,
         *,
         incidentRecordArn: str,
         relatedItemsUpdate: RelatedItemsUpdateTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Add or remove related items from the related items tab of an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_related_items)
         """
 
     async def update_replication_set(
         self,
         *,
         actions: Sequence[UpdateReplicationSetActionTypeDef],
         arn: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Add or delete Regions from your replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_replication_set)
         """
@@ -484,15 +484,15 @@
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
         incidentTemplateTags: Mapping[str, str] = ...,
         incidentTemplateTitle: str = ...,
-        integrations: Sequence[IntegrationTypeDef] = ...
+        integrations: Sequence[IntegrationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_response_plan)
         """
@@ -502,15 +502,15 @@
         *,
         eventId: str,
         incidentRecordArn: str,
         clientToken: str = ...,
         eventData: str = ...,
         eventReferences: Sequence[EventReferenceTypeDef] = ...,
         eventTime: TimestampTypeDef = ...,
-        eventType: str = ...
+        eventType: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a timeline event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_timeline_event)
         """
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/literals.py` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/literals.py`

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
     "GetResourcePoliciesPaginatorName",
     "IncidentRecordStatusType",
     "ItemTypeType",
     "ListIncidentFindingsPaginatorName",
     "ListIncidentRecordsPaginatorName",
     "ListRelatedItemsPaginatorName",
@@ -42,15 +41,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 GetResourcePoliciesPaginatorName = Literal["get_resource_policies"]
 IncidentRecordStatusType = Literal["OPEN", "RESOLVED"]
 ItemTypeType = Literal[
     "ANALYSIS",
     "ATTACHMENT",
     "AUTOMATION",
     "INCIDENT",
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/literals.pyi` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/paginator.py` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,26 +53,24 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GetResourcePoliciesPaginator",
     "ListIncidentFindingsPaginator",
     "ListIncidentRecordsPaginator",
     "ListRelatedItemsPaginator",
     "ListReplicationSetsPaginator",
     "ListResponsePlansPaginator",
     "ListTimelineEventsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -115,15 +113,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/paginators/#listincidentrecordspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIncidentRecordsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListIncidentRecords.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/paginators/#listincidentrecordspaginator)
         """
 
 
@@ -181,13 +179,13 @@
     def paginate(
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         sortBy: Literal["EVENT_TIME"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTimelineEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListTimelineEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/paginators/#listtimelineeventspaginator)
         """
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/paginator.pyi` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/paginators/#listincidentrecordspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIncidentRecordsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListIncidentRecords.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/paginators/#listincidentrecordspaginator)
         """
 
 class ListRelatedItemsPaginator(AioPaginator):
@@ -171,13 +171,13 @@
     def paginate(
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         sortBy: Literal["EVENT_TIME"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTimelineEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListTimelineEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/paginators/#listtimelineeventspaginator)
         """
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/type_defs.py` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/type_defs.py`

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
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
     "BatchGetIncidentFindingsErrorTypeDef",
     "BatchGetIncidentFindingsInputRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/type_defs.pyi` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/waiter.py` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents/waiter.pyi` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-incidents
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSMIncidents 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSMIncidents 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/
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
 
 <a id="types-aiobotocore-ssm-incidents"></a>
 
 # types-aiobotocore-ssm-incidents
 
 [![PyPI - types-aiobotocore-ssm-incidents](https://img.shields.io/pypi/v/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-incidents)](https://pepy.tech/project/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [types-aiobotocore-ssm-incidents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-incidents-2.9.0/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-incidents-2.9.1/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

