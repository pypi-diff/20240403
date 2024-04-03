# Comparing `tmp/types-aiobotocore-codestar-notifications-2.9.0.tar.gz` & `tmp/types-aiobotocore-codestar-notifications-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-notifications-2.9.0.tar", last modified: Wed Dec 13 19:58:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-notifications-2.9.1.tar", last modified: Thu Jan 18 01:20:22 2024, max compression
```

## Comparing `types-aiobotocore-codestar-notifications-2.9.0.tar` & `types-aiobotocore-codestar-notifications-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:56.337918 types-aiobotocore-codestar-notifications-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2023-12-13 19:58:56.337918 types-aiobotocore-codestar-notifications-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:56.337918 types-aiobotocore-codestar-notifications-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:56.333918 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15326 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2023-12-13 19:43:02.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2023-12-13 19:43:02.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2023-12-13 19:43:02.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:56.333918 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.513433 types-aiobotocore-codestar-notifications-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-01-18 01:20:22.513433 types-aiobotocore-codestar-notifications-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:22.513433 types-aiobotocore-codestar-notifications-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.513433 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-01-18 01:04:58.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-01-18 01:04:59.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-01-18 01:04:58.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.513433 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/LICENSE` & `types-aiobotocore-codestar-notifications-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/PKG-INFO` & `types-aiobotocore-codestar-notifications-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-notifications
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeStarNotifications 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeStarNotifications 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/
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
 
 <a id="types-aiobotocore-codestar-notifications"></a>
 
 # types-aiobotocore-codestar-notifications
 
 [![PyPI - types-aiobotocore-codestar-notifications](https://img.shields.io/pypi/v/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarNotifications 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[aiobotocore.CodeStarNotifications 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/README.md` & `types-aiobotocore-codestar-notifications-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarNotifications 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[aiobotocore.CodeStarNotifications 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/setup.py` & `types-aiobotocore-codestar-notifications-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar-notifications",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codestar_notifications"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeStarNotifications 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeStarNotifications 2.9.1 service generated with"
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
         "aiobotocore codestar-notifications type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codestar_notifications": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/__init__.py` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import CodeStarNotificationsClient
 from .paginator import ListEventTypesPaginator, ListNotificationRulesPaginator, ListTargetsPaginator
 
 Client = CodeStarNotificationsClient
 
-
 __all__ = (
     "Client",
     "CodeStarNotificationsClient",
     "ListEventTypesPaginator",
     "ListNotificationRulesPaginator",
     "ListTargetsPaginator",
 )
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/__init__.pyi` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/__main__.py` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeStarNotifications 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeStarNotifications 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications\nOther"
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

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/client.py` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeStarNotificationsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -108,15 +107,15 @@
         Name: str,
         EventTypeIds: Sequence[str],
         Resource: str,
         Targets: Sequence[TargetTypeDef],
         DetailType: DetailTypeType,
         ClientRequestToken: str = ...,
         Tags: Mapping[str, str] = ...,
-        Status: NotificationRuleStatusType = ...
+        Status: NotificationRuleStatusType = ...,
     ) -> CreateNotificationRuleResultTypeDef:
         """
         Creates a notification rule for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.create_notification_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#create_notification_rule)
         """
@@ -164,30 +163,30 @@
         """
 
     async def list_event_types(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEventTypesResultTypeDef:
         """
         Returns information about the event types available for configuring
         notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.list_event_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#list_event_types)
         """
 
     async def list_notification_rules(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListNotificationRulesResultTypeDef:
         """
         Returns a list of the notification rules for an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.list_notification_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#list_notification_rules)
         """
@@ -201,15 +200,15 @@
         """
 
     async def list_targets(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTargetsResultTypeDef:
         """
         Returns a list of the notification rule targets for an Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.list_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#list_targets)
@@ -260,15 +259,15 @@
         self,
         *,
         Arn: str,
         Name: str = ...,
         Status: NotificationRuleStatusType = ...,
         EventTypeIds: Sequence[str] = ...,
         Targets: Sequence[TargetTypeDef] = ...,
-        DetailType: DetailTypeType = ...
+        DetailType: DetailTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates a notification rule for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.update_notification_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#update_notification_rule)
         """
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/client.pyi` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         Name: str,
         EventTypeIds: Sequence[str],
         Resource: str,
         Targets: Sequence[TargetTypeDef],
         DetailType: DetailTypeType,
         ClientRequestToken: str = ...,
         Tags: Mapping[str, str] = ...,
-        Status: NotificationRuleStatusType = ...
+        Status: NotificationRuleStatusType = ...,
     ) -> CreateNotificationRuleResultTypeDef:
         """
         Creates a notification rule for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.create_notification_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#create_notification_rule)
         """
@@ -160,30 +160,30 @@
         """
 
     async def list_event_types(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEventTypesResultTypeDef:
         """
         Returns information about the event types available for configuring
         notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.list_event_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#list_event_types)
         """
 
     async def list_notification_rules(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListNotificationRulesResultTypeDef:
         """
         Returns a list of the notification rules for an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.list_notification_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#list_notification_rules)
         """
@@ -197,15 +197,15 @@
         """
 
     async def list_targets(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTargetsResultTypeDef:
         """
         Returns a list of the notification rule targets for an Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.list_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#list_targets)
@@ -256,15 +256,15 @@
         self,
         *,
         Arn: str,
         Name: str = ...,
         Status: NotificationRuleStatusType = ...,
         EventTypeIds: Sequence[str] = ...,
         Targets: Sequence[TargetTypeDef] = ...,
-        DetailType: DetailTypeType = ...
+        DetailType: DetailTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates a notification rule for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client.update_notification_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/client/#update_notification_rule)
         """
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/literals.py` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/literals.py`

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
     "DetailTypeType",
     "ListEventTypesFilterNameType",
     "ListEventTypesPaginatorName",
     "ListNotificationRulesFilterNameType",
     "ListNotificationRulesPaginatorName",
     "ListTargetsFilterNameType",
@@ -33,15 +32,14 @@
     "CodeStarNotificationsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DetailTypeType = Literal["BASIC", "FULL"]
 ListEventTypesFilterNameType = Literal["RESOURCE_TYPE", "SERVICE_NAME"]
 ListEventTypesPaginatorName = Literal["list_event_types"]
 ListNotificationRulesFilterNameType = Literal[
     "CREATED_BY", "EVENT_TYPE_ID", "RESOURCE", "TARGET_ADDRESS"
 ]
 ListNotificationRulesPaginatorName = Literal["list_notification_rules"]
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/literals.pyi` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/paginator.py` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     ListTargetsFilterTypeDef,
     ListTargetsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListEventTypesPaginator", "ListNotificationRulesPaginator", "ListTargetsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -59,15 +58,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listeventtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEventTypesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listeventtypespaginator)
         """
 
 
@@ -77,15 +76,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listnotificationrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotificationRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listnotificationrulespaginator)
         """
 
 
@@ -95,13 +94,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listtargetspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listtargetspaginator)
         """
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/paginator.pyi` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listeventtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEventTypesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listeventtypespaginator)
         """
 
 class ListNotificationRulesPaginator(AioPaginator):
@@ -73,15 +73,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listnotificationrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotificationRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listnotificationrulespaginator)
         """
 
 class ListTargetsPaginator(AioPaginator):
@@ -90,13 +90,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listtargetspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/paginators/#listtargetspaginator)
         """
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/type_defs.py` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TargetTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteNotificationRuleRequestRequestTypeDef",
     "DeleteTargetRequestRequestTypeDef",
     "DescribeNotificationRuleRequestRequestTypeDef",
     "EventTypeSummaryTypeDef",
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications/type_defs.pyi` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-notifications
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeStarNotifications 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeStarNotifications 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/
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
 
 <a id="types-aiobotocore-codestar-notifications"></a>
 
 # types-aiobotocore-codestar-notifications
 
 [![PyPI - types-aiobotocore-codestar-notifications](https://img.shields.io/pypi/v/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarNotifications 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[aiobotocore.CodeStarNotifications 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-notifications-2.9.0/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-notifications-2.9.1/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

