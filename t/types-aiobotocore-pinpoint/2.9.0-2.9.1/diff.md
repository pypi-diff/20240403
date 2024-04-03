# Comparing `tmp/types-aiobotocore-pinpoint-2.9.0.tar.gz` & `tmp/types-aiobotocore-pinpoint-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pinpoint-2.9.0.tar", last modified: Wed Dec 13 20:00:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-pinpoint-2.9.1.tar", last modified: Thu Jan 18 01:21:29 2024, max compression
```

## Comparing `types-aiobotocore-pinpoint-2.9.0.tar` & `types-aiobotocore-pinpoint-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:09.345321 types-aiobotocore-pinpoint-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:39.000000 types-aiobotocore-pinpoint-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2023-12-13 20:00:09.345321 types-aiobotocore-pinpoint-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2023-12-13 19:51:39.000000 types-aiobotocore-pinpoint-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:09.345321 types-aiobotocore-pinpoint-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:51:39.000000 types-aiobotocore-pinpoint-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:09.341321 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-13 19:51:39.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-13 19:51:39.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:51:39.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84339 2023-12-13 19:51:42.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    84336 2023-12-13 19:51:40.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11391 2023-12-13 19:51:42.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2023-12-13 19:51:42.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:39.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   139183 2023-12-13 19:51:45.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   139182 2023-12-13 19:51:43.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:39.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:09.345321 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:09.000000 types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.689119 types-aiobotocore-pinpoint-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:17.000000 types-aiobotocore-pinpoint-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-01-18 01:21:29.689119 types-aiobotocore-pinpoint-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-01-18 01:13:17.000000 types-aiobotocore-pinpoint-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:29.689119 types-aiobotocore-pinpoint-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:13:17.000000 types-aiobotocore-pinpoint-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.689119 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 01:13:17.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 01:13:17.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:13:17.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84360 2024-01-18 01:13:18.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84357 2024-01-18 01:13:18.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-01-18 01:13:18.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-01-18 01:13:18.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:17.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   139182 2024-01-18 01:13:23.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139182 2024-01-18 01:13:22.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:17.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.689119 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:29.000000 types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/LICENSE` & `types-aiobotocore-pinpoint-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-pinpoint-2.9.0/PKG-INFO` & `types-aiobotocore-pinpoint-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Pinpoint 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Pinpoint 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/
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
 
 <a id="types-aiobotocore-pinpoint"></a>
 
 # types-aiobotocore-pinpoint
 
 [![PyPI - types-aiobotocore-pinpoint](https://img.shields.io/pypi/v/types-aiobotocore-pinpoint.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint)](https://pepy.tech/project/types-aiobotocore-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Pinpoint 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[aiobotocore.Pinpoint 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [types-aiobotocore-pinpoint docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/README.md` & `types-aiobotocore-pinpoint-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint)](https://pepy.tech/project/types-aiobotocore-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Pinpoint 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[aiobotocore.Pinpoint 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [types-aiobotocore-pinpoint docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/setup.py` & `types-aiobotocore-pinpoint-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pinpoint",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Pinpoint 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Pinpoint 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore pinpoint type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_pinpoint": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/__main__.py` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Pinpoint 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Pinpoint 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
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

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/client.py` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#create_journey)
         """
 
     async def create_push_template(
         self,
         *,
         PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,
-        TemplateName: str
+        TemplateName: str,
     ) -> CreatePushTemplateResponseTypeDef:
         """
         Creates a message template for messages that are sent through a push
         notification
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_push_template)
@@ -689,15 +689,15 @@
         self,
         *,
         ApplicationId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetApplicationDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to
         an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_application_date_range_kpi)
@@ -759,15 +759,15 @@
         *,
         ApplicationId: str,
         CampaignId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetCampaignDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to a
         campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_date_range_kpi)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#get_campaign_date_range_kpi)
@@ -952,15 +952,15 @@
         *,
         ApplicationId: str,
         JourneyId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetJourneyDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard engagement metric that
         applies to a
         journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_date_range_kpi)
@@ -970,15 +970,15 @@
     async def get_journey_execution_activity_metrics(
         self,
         *,
         ApplicationId: str,
         JourneyActivityId: str,
         JourneyId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyExecutionActivityMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard execution metric that
         applies to a journey
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_execution_activity_metrics)
@@ -1001,15 +1001,15 @@
         self,
         *,
         ApplicationId: str,
         JourneyActivityId: str,
         JourneyId: str,
         RunId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyRunExecutionActivityMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard run execution metric
         that applies to a journey
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_activity_metrics)
@@ -1019,15 +1019,15 @@
     async def get_journey_run_execution_metrics(
         self,
         *,
         ApplicationId: str,
         JourneyId: str,
         RunId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyRunExecutionMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard run execution metric
         that applies to a
         journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_metrics)
@@ -1237,15 +1237,15 @@
 
     async def list_templates(
         self,
         *,
         NextToken: str = ...,
         PageSize: str = ...,
         Prefix: str = ...,
-        TemplateType: str = ...
+        TemplateType: str = ...,
     ) -> ListTemplatesResponseTypeDef:
         """
         Retrieves information about all the message templates that are associated with
         your Amazon Pinpoint
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.list_templates)
@@ -1287,15 +1287,15 @@
         """
 
     async def remove_attributes(
         self,
         *,
         ApplicationId: str,
         AttributeType: str,
-        UpdateAttributesRequest: UpdateAttributesRequestTypeDef
+        UpdateAttributesRequest: UpdateAttributesRequestTypeDef,
     ) -> RemoveAttributesResponseTypeDef:
         """
         Removes one or more custom attributes, of the same attribute type, from the
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.remove_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#remove_attributes)
@@ -1311,15 +1311,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#send_messages)
         """
 
     async def send_otp_message(
         self,
         *,
         ApplicationId: str,
-        SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef
+        SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef,
     ) -> SendOTPMessageResponseTypeDef:
         """
         Send an OTP message See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/SendOTPMessage).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_otp_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#send_otp_message)
@@ -1407,30 +1407,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_apns_voip_channel)
         """
 
     async def update_apns_voip_sandbox_channel(
         self,
         *,
         APNSVoipSandboxChannelRequest: APNSVoipSandboxChannelRequestTypeDef,
-        ApplicationId: str
+        ApplicationId: str,
     ) -> UpdateApnsVoipSandboxChannelResponseTypeDef:
         """
         Enables the APNs VoIP sandbox channel for an application or updates the status
         and settings of the APNs VoIP sandbox channel for an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_apns_voip_sandbox_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_apns_voip_sandbox_channel)
         """
 
     async def update_application_settings(
         self,
         *,
         ApplicationId: str,
-        WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef
+        WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef,
     ) -> UpdateApplicationSettingsResponseTypeDef:
         """
         Updates the settings for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_application_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_application_settings)
         """
@@ -1448,15 +1448,15 @@
         """
 
     async def update_campaign(
         self,
         *,
         ApplicationId: str,
         CampaignId: str,
-        WriteCampaignRequest: WriteCampaignRequestTypeDef
+        WriteCampaignRequest: WriteCampaignRequestTypeDef,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates the configuration and other settings for a campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_campaign)
         """
@@ -1475,15 +1475,15 @@
 
     async def update_email_template(
         self,
         *,
         EmailTemplateRequest: EmailTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateEmailTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the
         email
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_email_template)
@@ -1528,15 +1528,15 @@
 
     async def update_in_app_template(
         self,
         *,
         InAppTemplateRequest: InAppTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateInAppTemplateResponseTypeDef:
         """
         Updates an existing message template for messages sent through the in-app
         message
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_in_app_template)
@@ -1565,30 +1565,30 @@
 
     async def update_push_template(
         self,
         *,
         PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdatePushTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through a push
         notification
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_push_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_push_template)
         """
 
     async def update_recommender_configuration(
         self,
         *,
         RecommenderId: str,
-        UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef
+        UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef,
     ) -> UpdateRecommenderConfigurationResponseTypeDef:
         """
         Updates an Amazon Pinpoint configuration for a recommender model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_recommender_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_recommender_configuration)
         """
@@ -1619,30 +1619,30 @@
 
     async def update_sms_template(
         self,
         *,
         SMSTemplateRequest: SMSTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateSmsTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the SMS
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_sms_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_sms_template)
         """
 
     async def update_template_active_version(
         self,
         *,
         TemplateActiveVersionRequest: TemplateActiveVersionRequestTypeDef,
         TemplateName: str,
-        TemplateType: str
+        TemplateType: str,
     ) -> UpdateTemplateActiveVersionResponseTypeDef:
         """
         Changes the status of a specific version of a message template to *active*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_template_active_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_template_active_version)
         """
@@ -1661,30 +1661,30 @@
 
     async def update_voice_template(
         self,
         *,
         TemplateName: str,
         VoiceTemplateRequest: VoiceTemplateRequestTypeDef,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateVoiceTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the
         voice
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_voice_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_voice_template)
         """
 
     async def verify_otp_message(
         self,
         *,
         ApplicationId: str,
-        VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef
+        VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef,
     ) -> VerifyOTPMessageResponseTypeDef:
         """
         Verify an OTP See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/VerifyOTPMessage).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.verify_otp_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#verify_otp_message)
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/client.pyi` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#create_journey)
         """
 
     async def create_push_template(
         self,
         *,
         PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,
-        TemplateName: str
+        TemplateName: str,
     ) -> CreatePushTemplateResponseTypeDef:
         """
         Creates a message template for messages that are sent through a push
         notification
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_push_template)
@@ -686,15 +686,15 @@
         self,
         *,
         ApplicationId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetApplicationDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to
         an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_application_date_range_kpi)
@@ -756,15 +756,15 @@
         *,
         ApplicationId: str,
         CampaignId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetCampaignDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to a
         campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_date_range_kpi)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#get_campaign_date_range_kpi)
@@ -949,15 +949,15 @@
         *,
         ApplicationId: str,
         JourneyId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetJourneyDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard engagement metric that
         applies to a
         journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_date_range_kpi)
@@ -967,15 +967,15 @@
     async def get_journey_execution_activity_metrics(
         self,
         *,
         ApplicationId: str,
         JourneyActivityId: str,
         JourneyId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyExecutionActivityMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard execution metric that
         applies to a journey
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_execution_activity_metrics)
@@ -998,15 +998,15 @@
         self,
         *,
         ApplicationId: str,
         JourneyActivityId: str,
         JourneyId: str,
         RunId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyRunExecutionActivityMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard run execution metric
         that applies to a journey
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_activity_metrics)
@@ -1016,15 +1016,15 @@
     async def get_journey_run_execution_metrics(
         self,
         *,
         ApplicationId: str,
         JourneyId: str,
         RunId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyRunExecutionMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard run execution metric
         that applies to a
         journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_metrics)
@@ -1234,15 +1234,15 @@
 
     async def list_templates(
         self,
         *,
         NextToken: str = ...,
         PageSize: str = ...,
         Prefix: str = ...,
-        TemplateType: str = ...
+        TemplateType: str = ...,
     ) -> ListTemplatesResponseTypeDef:
         """
         Retrieves information about all the message templates that are associated with
         your Amazon Pinpoint
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.list_templates)
@@ -1284,15 +1284,15 @@
         """
 
     async def remove_attributes(
         self,
         *,
         ApplicationId: str,
         AttributeType: str,
-        UpdateAttributesRequest: UpdateAttributesRequestTypeDef
+        UpdateAttributesRequest: UpdateAttributesRequestTypeDef,
     ) -> RemoveAttributesResponseTypeDef:
         """
         Removes one or more custom attributes, of the same attribute type, from the
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.remove_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#remove_attributes)
@@ -1308,15 +1308,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#send_messages)
         """
 
     async def send_otp_message(
         self,
         *,
         ApplicationId: str,
-        SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef
+        SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef,
     ) -> SendOTPMessageResponseTypeDef:
         """
         Send an OTP message See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/SendOTPMessage).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_otp_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#send_otp_message)
@@ -1404,30 +1404,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_apns_voip_channel)
         """
 
     async def update_apns_voip_sandbox_channel(
         self,
         *,
         APNSVoipSandboxChannelRequest: APNSVoipSandboxChannelRequestTypeDef,
-        ApplicationId: str
+        ApplicationId: str,
     ) -> UpdateApnsVoipSandboxChannelResponseTypeDef:
         """
         Enables the APNs VoIP sandbox channel for an application or updates the status
         and settings of the APNs VoIP sandbox channel for an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_apns_voip_sandbox_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_apns_voip_sandbox_channel)
         """
 
     async def update_application_settings(
         self,
         *,
         ApplicationId: str,
-        WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef
+        WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef,
     ) -> UpdateApplicationSettingsResponseTypeDef:
         """
         Updates the settings for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_application_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_application_settings)
         """
@@ -1445,15 +1445,15 @@
         """
 
     async def update_campaign(
         self,
         *,
         ApplicationId: str,
         CampaignId: str,
-        WriteCampaignRequest: WriteCampaignRequestTypeDef
+        WriteCampaignRequest: WriteCampaignRequestTypeDef,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates the configuration and other settings for a campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_campaign)
         """
@@ -1472,15 +1472,15 @@
 
     async def update_email_template(
         self,
         *,
         EmailTemplateRequest: EmailTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateEmailTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the
         email
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_email_template)
@@ -1525,15 +1525,15 @@
 
     async def update_in_app_template(
         self,
         *,
         InAppTemplateRequest: InAppTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateInAppTemplateResponseTypeDef:
         """
         Updates an existing message template for messages sent through the in-app
         message
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_in_app_template)
@@ -1562,30 +1562,30 @@
 
     async def update_push_template(
         self,
         *,
         PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdatePushTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through a push
         notification
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_push_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_push_template)
         """
 
     async def update_recommender_configuration(
         self,
         *,
         RecommenderId: str,
-        UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef
+        UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef,
     ) -> UpdateRecommenderConfigurationResponseTypeDef:
         """
         Updates an Amazon Pinpoint configuration for a recommender model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_recommender_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_recommender_configuration)
         """
@@ -1616,30 +1616,30 @@
 
     async def update_sms_template(
         self,
         *,
         SMSTemplateRequest: SMSTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateSmsTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the SMS
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_sms_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_sms_template)
         """
 
     async def update_template_active_version(
         self,
         *,
         TemplateActiveVersionRequest: TemplateActiveVersionRequestTypeDef,
         TemplateName: str,
-        TemplateType: str
+        TemplateType: str,
     ) -> UpdateTemplateActiveVersionResponseTypeDef:
         """
         Changes the status of a specific version of a message template to *active*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_template_active_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_template_active_version)
         """
@@ -1658,30 +1658,30 @@
 
     async def update_voice_template(
         self,
         *,
         TemplateName: str,
         VoiceTemplateRequest: VoiceTemplateRequestTypeDef,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateVoiceTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the
         voice
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_voice_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#update_voice_template)
         """
 
     async def verify_otp_message(
         self,
         *,
         ApplicationId: str,
-        VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef
+        VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef,
     ) -> VerifyOTPMessageResponseTypeDef:
         """
         Verify an OTP See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/VerifyOTPMessage).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.verify_otp_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#verify_otp_message)
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/literals.py` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/literals.py`

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
     "ActionType",
     "AlignmentType",
     "AttributeTypeType",
     "ButtonActionType",
     "CampaignStatusType",
     "ChannelTypeType",
@@ -51,15 +50,14 @@
     "TypeType",
     "PinpointServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ActionType = Literal["DEEP_LINK", "OPEN_APP", "URL"]
 AlignmentType = Literal["CENTER", "LEFT", "RIGHT"]
 AttributeTypeType = Literal[
     "AFTER", "BEFORE", "BETWEEN", "CONTAINS", "EXCLUSIVE", "INCLUSIVE", "ON"
 ]
 ButtonActionType = Literal["CLOSE", "DEEP_LINK", "LINK"]
 CampaignStatusType = Literal[
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/literals.pyi` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/type_defs.py` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint/type_defs.pyi` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/PKG-INFO` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Pinpoint 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Pinpoint 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/
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
 
 <a id="types-aiobotocore-pinpoint"></a>
 
 # types-aiobotocore-pinpoint
 
 [![PyPI - types-aiobotocore-pinpoint](https://img.shields.io/pypi/v/types-aiobotocore-pinpoint.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint)](https://pepy.tech/project/types-aiobotocore-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Pinpoint 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[aiobotocore.Pinpoint 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [types-aiobotocore-pinpoint docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pinpoint-2.9.0/types_aiobotocore_pinpoint.egg-info/SOURCES.txt` & `types-aiobotocore-pinpoint-2.9.1/types_aiobotocore_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

