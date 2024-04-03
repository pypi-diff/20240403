# Comparing `tmp/types-aiobotocore-panorama-2.9.0.tar.gz` & `tmp/types-aiobotocore-panorama-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-panorama-2.9.0.tar", last modified: Wed Dec 13 20:00:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-panorama-2.9.1.tar", last modified: Thu Jan 18 01:21:26 2024, max compression
```

## Comparing `types-aiobotocore-panorama-2.9.0.tar` & `types-aiobotocore-panorama-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.969350 types-aiobotocore-panorama-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12338 2023-12-13 20:00:05.969350 types-aiobotocore-panorama-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:05.969350 types-aiobotocore-panorama-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.969350 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25605 2023-12-13 19:51:23.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25601 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2023-12-13 19:51:23.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2023-12-13 19:51:23.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    32382 2023-12-13 19:51:25.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32381 2023-12-13 19:51:23.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:22.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.969350 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12338 2023-12-13 20:00:05.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 20:00:05.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:05.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:05.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:05.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:05.000000 types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.669133 types-aiobotocore-panorama-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:02.000000 types-aiobotocore-panorama-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-01-18 01:21:26.669133 types-aiobotocore-panorama-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-01-18 01:13:02.000000 types-aiobotocore-panorama-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:26.669133 types-aiobotocore-panorama-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:13:02.000000 types-aiobotocore-panorama-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.669133 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 01:13:02.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 01:13:02.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:13:02.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25615 2024-01-18 01:13:03.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25612 2024-01-18 01:13:03.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-01-18 01:13:03.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-01-18 01:13:03.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:02.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    32381 2024-01-18 01:13:03.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32381 2024-01-18 01:13:03.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:02.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.669133 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-01-18 01:21:26.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-18 01:21:26.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:26.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:26.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:26.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:26.000000 types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-panorama-2.9.0/LICENSE` & `types-aiobotocore-panorama-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-panorama-2.9.0/PKG-INFO` & `types-aiobotocore-panorama-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-panorama
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Panorama 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Panorama 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/
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
 
 <a id="types-aiobotocore-panorama"></a>
 
 # types-aiobotocore-panorama
 
 [![PyPI - types-aiobotocore-panorama](https://img.shields.io/pypi/v/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-panorama)](https://pepy.tech/project/types-aiobotocore-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Panorama 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[aiobotocore.Panorama 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [types-aiobotocore-panorama docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-panorama-2.9.0/README.md` & `types-aiobotocore-panorama-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-panorama)](https://pepy.tech/project/types-aiobotocore-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Panorama 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[aiobotocore.Panorama 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [types-aiobotocore-panorama docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-panorama-2.9.0/setup.py` & `types-aiobotocore-panorama-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-panorama",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_panorama"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Panorama 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Panorama 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore panorama type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_panorama": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/__main__.py` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Panorama 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Panorama 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama\nOther"
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

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/client.py` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PanoramaClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -135,29 +134,29 @@
         DefaultRuntimeContextDevice: str,
         ManifestPayload: ManifestPayloadTypeDef,
         ApplicationInstanceIdToReplace: str = ...,
         Description: str = ...,
         ManifestOverridesPayload: ManifestOverridesPayloadTypeDef = ...,
         Name: str = ...,
         RuntimeRoleArn: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateApplicationInstanceResponseTypeDef:
         """
         Creates an application instance and deploys it to a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_application_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_application_instance)
         """
 
     async def create_job_for_devices(
         self,
         *,
         DeviceIds: Sequence[str],
         JobType: JobTypeType,
-        DeviceJobConfig: DeviceJobConfigTypeDef = ...
+        DeviceJobConfig: DeviceJobConfigTypeDef = ...,
     ) -> CreateJobForDevicesResponseTypeDef:
         """
         Creates a job to run on a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_job_for_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_job_for_devices)
         """
@@ -167,15 +166,15 @@
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
         JobTags: Sequence[JobResourceTagsTypeDef] = ...,
-        NodeDescription: str = ...
+        NodeDescription: str = ...,
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_node_from_template_job)
         """
@@ -193,15 +192,15 @@
     async def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...
+        JobTags: Sequence[JobResourceTagsTypeDef] = ...,
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_package_import_job)
         """
@@ -225,15 +224,15 @@
     async def deregister_package_version(
         self,
         *,
         PackageId: str,
         PackageVersion: str,
         PatchVersion: str,
         OwnerAccount: str = ...,
-        UpdatedLatestPatchVersion: str = ...
+        UpdatedLatestPatchVersion: str = ...,
     ) -> Dict[str, Any]:
         """
         Deregisters a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.deregister_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#deregister_package_version)
         """
@@ -314,15 +313,15 @@
 
     async def describe_package_version(
         self,
         *,
         PackageId: str,
         PackageVersion: str,
         OwnerAccount: str = ...,
-        PatchVersion: str = ...
+        PatchVersion: str = ...,
     ) -> DescribePackageVersionResponseTypeDef:
         """
         Returns information about a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#describe_package_version)
         """
@@ -363,15 +362,15 @@
 
     async def list_application_instances(
         self,
         *,
         DeviceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StatusFilter: StatusFilterType = ...
+        StatusFilter: StatusFilterType = ...,
     ) -> ListApplicationInstancesResponseTypeDef:
         """
         Returns a list of application instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_application_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#list_application_instances)
         """
@@ -380,15 +379,15 @@
         self,
         *,
         DeviceAggregatedStatusFilter: DeviceAggregatedStatusType = ...,
         MaxResults: int = ...,
         NameFilter: str = ...,
         NextToken: str = ...,
         SortBy: ListDevicesSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListDevicesResponseTypeDef:
         """
         Returns a list of devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#list_devices)
         """
@@ -418,15 +417,15 @@
         *,
         Category: NodeCategoryType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         OwnerAccount: str = ...,
         PackageName: str = ...,
         PackageVersion: str = ...,
-        PatchVersion: str = ...
+        PatchVersion: str = ...,
     ) -> ListNodesResponseTypeDef:
         """
         Returns a list of nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_nodes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#list_nodes)
         """
@@ -463,15 +462,15 @@
 
     async def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
         NetworkingConfiguration: NetworkPayloadTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#provision_device)
         """
@@ -479,15 +478,15 @@
     async def register_package_version(
         self,
         *,
         PackageId: str,
         PackageVersion: str,
         PatchVersion: str,
         MarkLatest: bool = ...,
-        OwnerAccount: str = ...
+        OwnerAccount: str = ...,
     ) -> Dict[str, Any]:
         """
         Registers a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.register_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#register_package_version)
         """
```

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/client.pyi` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -131,29 +131,29 @@
         DefaultRuntimeContextDevice: str,
         ManifestPayload: ManifestPayloadTypeDef,
         ApplicationInstanceIdToReplace: str = ...,
         Description: str = ...,
         ManifestOverridesPayload: ManifestOverridesPayloadTypeDef = ...,
         Name: str = ...,
         RuntimeRoleArn: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateApplicationInstanceResponseTypeDef:
         """
         Creates an application instance and deploys it to a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_application_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_application_instance)
         """
 
     async def create_job_for_devices(
         self,
         *,
         DeviceIds: Sequence[str],
         JobType: JobTypeType,
-        DeviceJobConfig: DeviceJobConfigTypeDef = ...
+        DeviceJobConfig: DeviceJobConfigTypeDef = ...,
     ) -> CreateJobForDevicesResponseTypeDef:
         """
         Creates a job to run on a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_job_for_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_job_for_devices)
         """
@@ -163,15 +163,15 @@
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
         JobTags: Sequence[JobResourceTagsTypeDef] = ...,
-        NodeDescription: str = ...
+        NodeDescription: str = ...,
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_node_from_template_job)
         """
@@ -189,15 +189,15 @@
     async def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...
+        JobTags: Sequence[JobResourceTagsTypeDef] = ...,
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_package_import_job)
         """
@@ -221,15 +221,15 @@
     async def deregister_package_version(
         self,
         *,
         PackageId: str,
         PackageVersion: str,
         PatchVersion: str,
         OwnerAccount: str = ...,
-        UpdatedLatestPatchVersion: str = ...
+        UpdatedLatestPatchVersion: str = ...,
     ) -> Dict[str, Any]:
         """
         Deregisters a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.deregister_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#deregister_package_version)
         """
@@ -310,15 +310,15 @@
 
     async def describe_package_version(
         self,
         *,
         PackageId: str,
         PackageVersion: str,
         OwnerAccount: str = ...,
-        PatchVersion: str = ...
+        PatchVersion: str = ...,
     ) -> DescribePackageVersionResponseTypeDef:
         """
         Returns information about a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#describe_package_version)
         """
@@ -359,15 +359,15 @@
 
     async def list_application_instances(
         self,
         *,
         DeviceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StatusFilter: StatusFilterType = ...
+        StatusFilter: StatusFilterType = ...,
     ) -> ListApplicationInstancesResponseTypeDef:
         """
         Returns a list of application instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_application_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#list_application_instances)
         """
@@ -376,15 +376,15 @@
         self,
         *,
         DeviceAggregatedStatusFilter: DeviceAggregatedStatusType = ...,
         MaxResults: int = ...,
         NameFilter: str = ...,
         NextToken: str = ...,
         SortBy: ListDevicesSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListDevicesResponseTypeDef:
         """
         Returns a list of devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#list_devices)
         """
@@ -414,15 +414,15 @@
         *,
         Category: NodeCategoryType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         OwnerAccount: str = ...,
         PackageName: str = ...,
         PackageVersion: str = ...,
-        PatchVersion: str = ...
+        PatchVersion: str = ...,
     ) -> ListNodesResponseTypeDef:
         """
         Returns a list of nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_nodes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#list_nodes)
         """
@@ -459,15 +459,15 @@
 
     async def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
         NetworkingConfiguration: NetworkPayloadTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#provision_device)
         """
@@ -475,15 +475,15 @@
     async def register_package_version(
         self,
         *,
         PackageId: str,
         PackageVersion: str,
         PatchVersion: str,
         MarkLatest: bool = ...,
-        OwnerAccount: str = ...
+        OwnerAccount: str = ...,
     ) -> Dict[str, Any]:
         """
         Registers a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.register_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#register_package_version)
         """
```

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/literals.py` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/literals.py`

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
     "ApplicationInstanceHealthStatusType",
     "ApplicationInstanceStatusType",
     "ConnectionTypeType",
     "DesiredStateType",
     "DeviceAggregatedStatusType",
     "DeviceBrandType",
@@ -48,15 +47,14 @@
     "TemplateTypeType",
     "UpdateProgressType",
     "PanoramaServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 ApplicationInstanceHealthStatusType = Literal["ERROR", "NOT_AVAILABLE", "RUNNING"]
 ApplicationInstanceStatusType = Literal[
     "DEPLOYMENT_ERROR",
     "DEPLOYMENT_FAILED",
     "DEPLOYMENT_IN_PROGRESS",
     "DEPLOYMENT_PENDING",
     "DEPLOYMENT_REQUESTED",
```

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/literals.pyi` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/type_defs.py` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
```

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama/type_defs.pyi` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/PKG-INFO` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-panorama
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Panorama 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Panorama 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/
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
 
 <a id="types-aiobotocore-panorama"></a>
 
 # types-aiobotocore-panorama
 
 [![PyPI - types-aiobotocore-panorama](https://img.shields.io/pypi/v/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-panorama)](https://pepy.tech/project/types-aiobotocore-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Panorama 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[aiobotocore.Panorama 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [types-aiobotocore-panorama docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-panorama-2.9.0/types_aiobotocore_panorama.egg-info/SOURCES.txt` & `types-aiobotocore-panorama-2.9.1/types_aiobotocore_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

