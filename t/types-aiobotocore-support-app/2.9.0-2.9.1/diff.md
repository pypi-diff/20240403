# Comparing `tmp/types-aiobotocore-support-app-2.9.0.tar.gz` & `tmp/types-aiobotocore-support-app-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-support-app-2.9.0.tar", last modified: Wed Dec 13 20:00:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-support-app-2.9.1.tar", last modified: Thu Jan 18 01:21:56 2024, max compression
```

## Comparing `types-aiobotocore-support-app-2.9.0.tar` & `types-aiobotocore-support-app-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.913066 types-aiobotocore-support-app-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2023-12-13 20:00:38.913066 types-aiobotocore-support-app-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10919 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:38.913066 types-aiobotocore-support-app-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.913066 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:12.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.913066 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2023-12-13 20:00:38.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 20:00:38.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:38.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:38.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:38.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 20:00:38.000000 types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.497000 types-aiobotocore-support-app-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-01-18 01:21:56.497000 types-aiobotocore-support-app-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:56.497000 types-aiobotocore-support-app-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-01-18 01:18:39.000000 types-aiobotocore-support-app-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.497000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:40.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.497000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-01-18 01:21:56.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:21:56.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:56.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:56.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:56.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:21:56.000000 types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-support-app-2.9.0/LICENSE` & `types-aiobotocore-support-app-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-support-app-2.9.0/PKG-INFO` & `types-aiobotocore-support-app-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support-app
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SupportApp 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SupportApp 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
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
 
 <a id="types-aiobotocore-support-app"></a>
 
 # types-aiobotocore-support-app
 
 [![PyPI - types-aiobotocore-support-app](https://img.shields.io/pypi/v/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupportApp 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
+[aiobotocore.SupportApp 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-support-app-2.9.0/README.md` & `types-aiobotocore-support-app-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupportApp 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
+[aiobotocore.SupportApp 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-support-app-2.9.0/setup.py` & `types-aiobotocore-support-app-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-support-app",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_support_app"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SupportApp 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SupportApp 2.9.1 service generated with"
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
     keywords="aiobotocore support-app type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_support_app": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/__main__.py` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SupportApp 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SupportApp 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp\nOther"
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

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/client.py` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         channelId: str,
         channelRoleArn: str,
         notifyOnCaseSeverity: NotificationSeverityLevelType,
         teamId: str,
         channelName: str = ...,
         notifyOnAddCorrespondenceToCase: bool = ...,
         notifyOnCreateOrReopenCase: bool = ...,
-        notifyOnResolveCase: bool = ...
+        notifyOnResolveCase: bool = ...,
     ) -> Dict[str, Any]:
         """
         Creates a Slack channel configuration for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client.create_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/client/#create_slack_channel_configuration)
         """
@@ -194,15 +194,15 @@
         channelId: str,
         teamId: str,
         channelName: str = ...,
         channelRoleArn: str = ...,
         notifyOnAddCorrespondenceToCase: bool = ...,
         notifyOnCaseSeverity: NotificationSeverityLevelType = ...,
         notifyOnCreateOrReopenCase: bool = ...,
-        notifyOnResolveCase: bool = ...
+        notifyOnResolveCase: bool = ...,
     ) -> UpdateSlackChannelConfigurationResultTypeDef:
         """
         Updates the configuration for a Slack channel, such as case update
         notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client.update_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/client/#update_slack_channel_configuration)
```

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/client.pyi` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         channelId: str,
         channelRoleArn: str,
         notifyOnCaseSeverity: NotificationSeverityLevelType,
         teamId: str,
         channelName: str = ...,
         notifyOnAddCorrespondenceToCase: bool = ...,
         notifyOnCreateOrReopenCase: bool = ...,
-        notifyOnResolveCase: bool = ...
+        notifyOnResolveCase: bool = ...,
     ) -> Dict[str, Any]:
         """
         Creates a Slack channel configuration for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client.create_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/client/#create_slack_channel_configuration)
         """
@@ -191,15 +191,15 @@
         channelId: str,
         teamId: str,
         channelName: str = ...,
         channelRoleArn: str = ...,
         notifyOnAddCorrespondenceToCase: bool = ...,
         notifyOnCaseSeverity: NotificationSeverityLevelType = ...,
         notifyOnCreateOrReopenCase: bool = ...,
-        notifyOnResolveCase: bool = ...
+        notifyOnResolveCase: bool = ...,
     ) -> UpdateSlackChannelConfigurationResultTypeDef:
         """
         Updates the configuration for a Slack channel, such as case update
         notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client.update_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/client/#update_slack_channel_configuration)
```

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/literals.py` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountTypeType",
     "NotificationSeverityLevelType",
     "SupportAppServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AccountTypeType = Literal["management", "member"]
 NotificationSeverityLevelType = Literal["all", "high", "none"]
 SupportAppServiceName = Literal["support-app"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/literals.pyi` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/type_defs.py` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateSlackChannelConfigurationRequestRequestTypeDef",
     "DeleteSlackChannelConfigurationRequestRequestTypeDef",
     "DeleteSlackWorkspaceConfigurationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ListSlackChannelConfigurationsRequestRequestTypeDef",
     "SlackChannelConfigurationTypeDef",
```

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app/type_defs.pyi` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/PKG-INFO` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support-app
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SupportApp 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SupportApp 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
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
 
 <a id="types-aiobotocore-support-app"></a>
 
 # types-aiobotocore-support-app
 
 [![PyPI - types-aiobotocore-support-app](https://img.shields.io/pypi/v/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupportApp 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
+[aiobotocore.SupportApp 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-support-app-2.9.0/types_aiobotocore_support_app.egg-info/SOURCES.txt` & `types-aiobotocore-support-app-2.9.1/types_aiobotocore_support_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

