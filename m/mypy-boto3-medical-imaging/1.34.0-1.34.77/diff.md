# Comparing `tmp/mypy-boto3-medical-imaging-1.34.0.tar.gz` & `tmp/mypy-boto3-medical-imaging-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medical-imaging-1.34.0.tar", last modified: Wed Dec 13 21:23:16 2023, max compression
+gzip compressed data, was "mypy-boto3-medical-imaging-1.34.77.tar", last modified: Wed Apr  3 19:32:40 2024, max compression
```

## Comparing `mypy-boto3-medical-imaging-1.34.0.tar` & `mypy-boto3-medical-imaging-1.34.77.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:16.959291 mypy-boto3-medical-imaging-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2023-12-13 21:23:16.959291 mypy-boto3-medical-imaging-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11967 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:16.959291 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16173 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18755 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:16.959291 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2023-12-13 21:23:16.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 21:23:16.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:16.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:16.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:16.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 21:23:16.000000 mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:16.959291 mypy-boto3-medical-imaging-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-12-13 21:14:13.000000 mypy-boto3-medical-imaging-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.560159 mypy-boto3-medical-imaging-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-04-03 19:32:40.556159 mypy-boto3-medical-imaging-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.556159 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19327 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19327 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.556159 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:40.560159 mypy-boto3-medical-imaging-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/setup.py
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/LICENSE` & `mypy-boto3-medical-imaging-1.34.77/LICENSE`

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

### Comparing `mypy-boto3-medical-imaging-1.34.0/PKG-INFO` & `mypy-boto3-medical-imaging-1.34.77/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medical-imaging
-Version: 1.34.0
-Summary: Type annotations for boto3.HealthImaging 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.77
+Summary: Type annotations for boto3.HealthImaging 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/
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
 
 <a id="mypy-boto3-medical-imaging"></a>
 
 # mypy-boto3-medical-imaging
 
 [![PyPI - mypy-boto3-medical-imaging](https://img.shields.io/pypi/v/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/README.md` & `mypy-boto3-medical-imaging-1.34.77/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/__init__.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListDICOMImportJobsPaginator,
     ListImageSetVersionsPaginator,
     SearchImageSetsPaginator,
 )
 
 Client = HealthImagingClient
 
-
 __all__ = (
     "Client",
     "HealthImagingClient",
     "ListDICOMImportJobsPaginator",
     "ListDatastoresPaginator",
     "ListImageSetVersionsPaginator",
     "SearchImageSetsPaginator",
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/__init__.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/client.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,37 +50,33 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("HealthImagingClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class HealthImagingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/)
     """
 
     meta: ClientMeta
@@ -111,30 +107,30 @@
         """
 
     def copy_image_set(
         self,
         *,
         datastoreId: str,
         sourceImageSetId: str,
-        copyImageSetInformation: CopyImageSetInformationTypeDef
+        copyImageSetInformation: CopyImageSetInformationTypeDef,
     ) -> CopyImageSetResponseTypeDef:
         """
         Copy an image set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.copy_image_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#copy_image_set)
         """
 
     def create_datastore(
         self,
         *,
         clientToken: str,
         datastoreName: str = ...,
         tags: Mapping[str, str] = ...,
-        kmsKeyArn: str = ...
+        kmsKeyArn: str = ...,
     ) -> CreateDatastoreResponseTypeDef:
         """
         Create a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.create_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#create_datastore)
         """
@@ -190,15 +186,15 @@
         """
 
     def get_image_frame(
         self,
         *,
         datastoreId: str,
         imageSetId: str,
-        imageFrameInformation: ImageFrameInformationTypeDef
+        imageFrameInformation: ImageFrameInformationTypeDef,
     ) -> GetImageFrameResponseTypeDef:
         """
         Get an image frame (pixel data) for an image set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.get_image_frame)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#get_image_frame)
         """
@@ -224,30 +220,30 @@
         """
 
     def list_datastores(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDatastoresResponseTypeDef:
         """
         List data stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.list_datastores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#list_datastores)
         """
 
     def list_dicom_import_jobs(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDICOMImportJobsResponseTypeDef:
         """
         List import jobs created for a specific data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.list_dicom_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#list_dicom_import_jobs)
         """
@@ -272,15 +268,15 @@
 
     def search_image_sets(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchImageSetsResponseTypeDef:
         """
         Search image sets based on defined input attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.search_image_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#search_image_sets)
         """
@@ -289,15 +285,15 @@
         self,
         *,
         dataAccessRoleArn: str,
         clientToken: str,
         datastoreId: str,
         inputS3Uri: str,
         outputS3Uri: str,
-        jobName: str = ...
+        jobName: str = ...,
     ) -> StartDICOMImportJobResponseTypeDef:
         """
         Start importing bulk data into an `ACTIVE` data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.start_dicom_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#start_dicom_import_job)
         """
@@ -320,15 +316,15 @@
 
     def update_image_set_metadata(
         self,
         *,
         datastoreId: str,
         imageSetId: str,
         latestVersionId: str,
-        updateImageSetMetadataUpdates: MetadataUpdatesTypeDef
+        updateImageSetMetadataUpdates: MetadataUpdatesTypeDef,
     ) -> UpdateImageSetMetadataResponseTypeDef:
         """
         Update image set metadata attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.update_image_set_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#update_image_set_metadata)
         """
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/client.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,31 +52,34 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("HealthImagingClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class HealthImagingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/)
     """
 
     meta: ClientMeta
@@ -107,30 +110,30 @@
         """
 
     def copy_image_set(
         self,
         *,
         datastoreId: str,
         sourceImageSetId: str,
-        copyImageSetInformation: CopyImageSetInformationTypeDef
+        copyImageSetInformation: CopyImageSetInformationTypeDef,
     ) -> CopyImageSetResponseTypeDef:
         """
         Copy an image set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.copy_image_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#copy_image_set)
         """
 
     def create_datastore(
         self,
         *,
         clientToken: str,
         datastoreName: str = ...,
         tags: Mapping[str, str] = ...,
-        kmsKeyArn: str = ...
+        kmsKeyArn: str = ...,
     ) -> CreateDatastoreResponseTypeDef:
         """
         Create a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.create_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#create_datastore)
         """
@@ -186,15 +189,15 @@
         """
 
     def get_image_frame(
         self,
         *,
         datastoreId: str,
         imageSetId: str,
-        imageFrameInformation: ImageFrameInformationTypeDef
+        imageFrameInformation: ImageFrameInformationTypeDef,
     ) -> GetImageFrameResponseTypeDef:
         """
         Get an image frame (pixel data) for an image set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.get_image_frame)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#get_image_frame)
         """
@@ -220,30 +223,30 @@
         """
 
     def list_datastores(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDatastoresResponseTypeDef:
         """
         List data stores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.list_datastores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#list_datastores)
         """
 
     def list_dicom_import_jobs(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDICOMImportJobsResponseTypeDef:
         """
         List import jobs created for a specific data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.list_dicom_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#list_dicom_import_jobs)
         """
@@ -268,15 +271,15 @@
 
     def search_image_sets(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchImageSetsResponseTypeDef:
         """
         Search image sets based on defined input attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.search_image_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#search_image_sets)
         """
@@ -285,15 +288,15 @@
         self,
         *,
         dataAccessRoleArn: str,
         clientToken: str,
         datastoreId: str,
         inputS3Uri: str,
         outputS3Uri: str,
-        jobName: str = ...
+        jobName: str = ...,
     ) -> StartDICOMImportJobResponseTypeDef:
         """
         Start importing bulk data into an `ACTIVE` data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.start_dicom_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#start_dicom_import_job)
         """
@@ -316,15 +319,15 @@
 
     def update_image_set_metadata(
         self,
         *,
         datastoreId: str,
         imageSetId: str,
         latestVersionId: str,
-        updateImageSetMetadataUpdates: MetadataUpdatesTypeDef
+        updateImageSetMetadataUpdates: MetadataUpdatesTypeDef,
     ) -> UpdateImageSetMetadataResponseTypeDef:
         """
         Update image set metadata attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.update_image_set_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#update_image_set_metadata)
         """
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/literals.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DatastoreStatusType",
     "ImageSetStateType",
     "ImageSetWorkflowStatusType",
     "JobStatusType",
     "ListDICOMImportJobsPaginatorName",
     "ListDatastoresPaginatorName",
     "ListImageSetVersionsPaginatorName",
     "OperatorType",
     "SearchImageSetsPaginatorName",
+    "SortFieldType",
+    "SortOrderType",
     "HealthImagingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 DatastoreStatusType = Literal["ACTIVE", "CREATE_FAILED", "CREATING", "DELETED", "DELETING"]
 ImageSetStateType = Literal["ACTIVE", "DELETED", "LOCKED"]
 ImageSetWorkflowStatusType = Literal[
     "COPIED",
     "COPYING",
     "COPYING_WITH_READ_ONLY_ACCESS",
     "COPY_FAILED",
@@ -53,14 +53,16 @@
 ]
 JobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "SUBMITTED"]
 ListDICOMImportJobsPaginatorName = Literal["list_dicom_import_jobs"]
 ListDatastoresPaginatorName = Literal["list_datastores"]
 ListImageSetVersionsPaginatorName = Literal["list_image_set_versions"]
 OperatorType = Literal["BETWEEN", "EQUAL"]
 SearchImageSetsPaginatorName = Literal["search_image_sets"]
+SortFieldType = Literal["DICOMStudyDateAndTime", "createdAt", "updatedAt"]
+SortOrderType = Literal["ASC", "DESC"]
 HealthImagingServiceName = Literal["medical-imaging"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -80,14 +82,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -98,14 +101,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -123,14 +127,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -153,14 +158,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -221,15 +227,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -301,17 +306,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -401,19 +408,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/literals.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     "ImageSetWorkflowStatusType",
     "JobStatusType",
     "ListDICOMImportJobsPaginatorName",
     "ListDatastoresPaginatorName",
     "ListImageSetVersionsPaginatorName",
     "OperatorType",
     "SearchImageSetsPaginatorName",
+    "SortFieldType",
+    "SortOrderType",
     "HealthImagingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 DatastoreStatusType = Literal["ACTIVE", "CREATE_FAILED", "CREATING", "DELETED", "DELETING"]
@@ -51,14 +53,16 @@
 ]
 JobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "SUBMITTED"]
 ListDICOMImportJobsPaginatorName = Literal["list_dicom_import_jobs"]
 ListDatastoresPaginatorName = Literal["list_datastores"]
 ListImageSetVersionsPaginatorName = Literal["list_image_set_versions"]
 OperatorType = Literal["BETWEEN", "EQUAL"]
 SearchImageSetsPaginatorName = Literal["search_image_sets"]
+SortFieldType = Literal["DICOMStudyDateAndTime", "createdAt", "updatedAt"]
+SortOrderType = Literal["ASC", "DESC"]
 HealthImagingServiceName = Literal["medical-imaging"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -78,14 +82,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -96,14 +101,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -121,14 +127,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -151,14 +158,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -219,15 +227,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -299,17 +306,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -399,19 +408,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/paginator.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,87 +43,81 @@
 __all__ = (
     "ListDICOMImportJobsPaginator",
     "ListDatastoresPaginator",
     "ListImageSetVersionsPaginator",
     "SearchImageSetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListDICOMImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdicomimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDICOMImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdicomimportjobspaginator)
         """
 
-
 class ListDatastoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdatastorespaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdatastorespaginator)
         """
 
-
 class ListImageSetVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListImageSetVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listimagesetversionspaginator)
     """
 
     def paginate(
         self, *, datastoreId: str, imageSetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImageSetVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListImageSetVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listimagesetversionspaginator)
         """
 
-
 class SearchImageSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#searchimagesetspaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[SearchImageSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#searchimagesetspaginator)
         """
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/paginator.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,79 +45,84 @@
     "ListDatastoresPaginator",
     "ListImageSetVersionsPaginator",
     "SearchImageSetsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListDICOMImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdicomimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDICOMImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdicomimportjobspaginator)
         """
 
+
 class ListDatastoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdatastorespaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdatastorespaginator)
         """
 
+
 class ListImageSetVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListImageSetVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listimagesetversionspaginator)
     """
 
     def paginate(
         self, *, datastoreId: str, imageSetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImageSetVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListImageSetVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listimagesetversionspaginator)
         """
 
+
 class SearchImageSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#searchimagesetspaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[SearchImageSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#searchimagesetspaginator)
         """
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/type_defs.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 
 from .literals import (
     DatastoreStatusType,
     ImageSetStateType,
     ImageSetWorkflowStatusType,
     JobStatusType,
     OperatorType,
+    SortFieldType,
+    SortOrderType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "CopyDestinationImageSetPropertiesTypeDef",
     "CopyDestinationImageSetTypeDef",
     "CopySourceImageSetInformationTypeDef",
     "CopySourceImageSetPropertiesTypeDef",
     "ResponseMetadataTypeDef",
@@ -60,14 +61,15 @@
     "ImageSetPropertiesTypeDef",
     "PaginatorConfigTypeDef",
     "ListDICOMImportJobsRequestRequestTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListImageSetVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TimestampTypeDef",
+    "SortTypeDef",
     "StartDICOMImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DICOMUpdatesTypeDef",
     "CopyImageSetInformationTypeDef",
     "CopyImageSetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
@@ -138,18 +140,18 @@
         "imageSetArn": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 CreateDatastoreRequestRequestTypeDef = TypedDict(
     "CreateDatastoreRequestRequestTypeDef",
     {
         "clientToken": str,
         "datastoreName": NotRequired[str],
@@ -201,14 +203,18 @@
         "DICOMPatientSex": NotRequired[str],
         "DICOMStudyInstanceUID": NotRequired[str],
         "DICOMStudyId": NotRequired[str],
         "DICOMStudyDescription": NotRequired[str],
         "DICOMNumberOfStudyRelatedSeries": NotRequired[int],
         "DICOMNumberOfStudyRelatedInstances": NotRequired[int],
         "DICOMAccessionNumber": NotRequired[str],
+        "DICOMSeriesInstanceUID": NotRequired[str],
+        "DICOMSeriesModality": NotRequired[str],
+        "DICOMSeriesBodyPart": NotRequired[str],
+        "DICOMSeriesNumber": NotRequired[int],
         "DICOMStudyDate": NotRequired[str],
         "DICOMStudyTime": NotRequired[str],
     },
 )
 DatastorePropertiesTypeDef = TypedDict(
     "DatastorePropertiesTypeDef",
     {
@@ -330,14 +336,21 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 TimestampTypeDef = Union[datetime, str]
+SortTypeDef = TypedDict(
+    "SortTypeDef",
+    {
+        "sortOrder": SortOrderType,
+        "sortField": SortFieldType,
+    },
+)
 StartDICOMImportJobRequestRequestTypeDef = TypedDict(
     "StartDICOMImportJobRequestRequestTypeDef",
     {
         "dataAccessRoleArn": str,
         "clientToken": str,
         "datastoreId": str,
         "inputS3Uri": str,
@@ -554,15 +567,17 @@
 SearchByAttributeValueTypeDef = TypedDict(
     "SearchByAttributeValueTypeDef",
     {
         "DICOMPatientId": NotRequired[str],
         "DICOMAccessionNumber": NotRequired[str],
         "DICOMStudyId": NotRequired[str],
         "DICOMStudyInstanceUID": NotRequired[str],
+        "DICOMSeriesInstanceUID": NotRequired[str],
         "createdAt": NotRequired[TimestampTypeDef],
+        "updatedAt": NotRequired[TimestampTypeDef],
         "DICOMStudyDateAndTime": NotRequired[DICOMStudyDateAndTimeTypeDef],
     },
 )
 MetadataUpdatesTypeDef = TypedDict(
     "MetadataUpdatesTypeDef",
     {
         "DICOMUpdates": NotRequired[DICOMUpdatesTypeDef],
@@ -576,14 +591,15 @@
         "copyImageSetInformation": CopyImageSetInformationTypeDef,
     },
 )
 SearchImageSetsResponseTypeDef = TypedDict(
     "SearchImageSetsResponseTypeDef",
     {
         "imageSetsMetadataSummaries": List[ImageSetsMetadataSummaryTypeDef],
+        "sort": SortTypeDef,
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchFilterTypeDef = TypedDict(
     "SearchFilterTypeDef",
     {
@@ -600,14 +616,15 @@
         "updateImageSetMetadataUpdates": MetadataUpdatesTypeDef,
     },
 )
 SearchCriteriaTypeDef = TypedDict(
     "SearchCriteriaTypeDef",
     {
         "filters": NotRequired[Sequence[SearchFilterTypeDef]],
+        "sort": NotRequired[SortTypeDef],
     },
 )
 SearchImageSetsRequestRequestTypeDef = TypedDict(
     "SearchImageSetsRequestRequestTypeDef",
     {
         "datastoreId": str,
         "searchCriteria": NotRequired[SearchCriteriaTypeDef],
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging/type_defs.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 from .literals import (
     DatastoreStatusType,
     ImageSetStateType,
     ImageSetWorkflowStatusType,
     JobStatusType,
     OperatorType,
+    SortFieldType,
+    SortOrderType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
@@ -59,14 +61,15 @@
     "ImageSetPropertiesTypeDef",
     "PaginatorConfigTypeDef",
     "ListDICOMImportJobsRequestRequestTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListImageSetVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TimestampTypeDef",
+    "SortTypeDef",
     "StartDICOMImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DICOMUpdatesTypeDef",
     "CopyImageSetInformationTypeDef",
     "CopyImageSetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
@@ -137,18 +140,18 @@
         "imageSetArn": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 CreateDatastoreRequestRequestTypeDef = TypedDict(
     "CreateDatastoreRequestRequestTypeDef",
     {
         "clientToken": str,
         "datastoreName": NotRequired[str],
@@ -200,14 +203,18 @@
         "DICOMPatientSex": NotRequired[str],
         "DICOMStudyInstanceUID": NotRequired[str],
         "DICOMStudyId": NotRequired[str],
         "DICOMStudyDescription": NotRequired[str],
         "DICOMNumberOfStudyRelatedSeries": NotRequired[int],
         "DICOMNumberOfStudyRelatedInstances": NotRequired[int],
         "DICOMAccessionNumber": NotRequired[str],
+        "DICOMSeriesInstanceUID": NotRequired[str],
+        "DICOMSeriesModality": NotRequired[str],
+        "DICOMSeriesBodyPart": NotRequired[str],
+        "DICOMSeriesNumber": NotRequired[int],
         "DICOMStudyDate": NotRequired[str],
         "DICOMStudyTime": NotRequired[str],
     },
 )
 DatastorePropertiesTypeDef = TypedDict(
     "DatastorePropertiesTypeDef",
     {
@@ -329,14 +336,21 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 TimestampTypeDef = Union[datetime, str]
+SortTypeDef = TypedDict(
+    "SortTypeDef",
+    {
+        "sortOrder": SortOrderType,
+        "sortField": SortFieldType,
+    },
+)
 StartDICOMImportJobRequestRequestTypeDef = TypedDict(
     "StartDICOMImportJobRequestRequestTypeDef",
     {
         "dataAccessRoleArn": str,
         "clientToken": str,
         "datastoreId": str,
         "inputS3Uri": str,
@@ -553,15 +567,17 @@
 SearchByAttributeValueTypeDef = TypedDict(
     "SearchByAttributeValueTypeDef",
     {
         "DICOMPatientId": NotRequired[str],
         "DICOMAccessionNumber": NotRequired[str],
         "DICOMStudyId": NotRequired[str],
         "DICOMStudyInstanceUID": NotRequired[str],
+        "DICOMSeriesInstanceUID": NotRequired[str],
         "createdAt": NotRequired[TimestampTypeDef],
+        "updatedAt": NotRequired[TimestampTypeDef],
         "DICOMStudyDateAndTime": NotRequired[DICOMStudyDateAndTimeTypeDef],
     },
 )
 MetadataUpdatesTypeDef = TypedDict(
     "MetadataUpdatesTypeDef",
     {
         "DICOMUpdates": NotRequired[DICOMUpdatesTypeDef],
@@ -575,14 +591,15 @@
         "copyImageSetInformation": CopyImageSetInformationTypeDef,
     },
 )
 SearchImageSetsResponseTypeDef = TypedDict(
     "SearchImageSetsResponseTypeDef",
     {
         "imageSetsMetadataSummaries": List[ImageSetsMetadataSummaryTypeDef],
+        "sort": SortTypeDef,
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchFilterTypeDef = TypedDict(
     "SearchFilterTypeDef",
     {
@@ -599,14 +616,15 @@
         "updateImageSetMetadataUpdates": MetadataUpdatesTypeDef,
     },
 )
 SearchCriteriaTypeDef = TypedDict(
     "SearchCriteriaTypeDef",
     {
         "filters": NotRequired[Sequence[SearchFilterTypeDef]],
+        "sort": NotRequired[SortTypeDef],
     },
 )
 SearchImageSetsRequestRequestTypeDef = TypedDict(
     "SearchImageSetsRequestRequestTypeDef",
     {
         "datastoreId": str,
         "searchCriteria": NotRequired[SearchCriteriaTypeDef],
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/PKG-INFO` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medical-imaging
-Version: 1.34.0
-Summary: Type annotations for boto3.HealthImaging 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.77
+Summary: Type annotations for boto3.HealthImaging 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/
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
 
 <a id="mypy-boto3-medical-imaging"></a>
 
 # mypy-boto3-medical-imaging
 
 [![PyPI - mypy-boto3-medical-imaging](https://img.shields.io/pypi/v/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medical-imaging-1.34.0/mypy_boto3_medical_imaging.egg-info/SOURCES.txt` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.34.0/setup.py` & `mypy-boto3-medical-imaging-1.34.77/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medical-imaging",
-    version="1.34.0",
+    version="1.34.77",
     packages=["mypy_boto3_medical_imaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.HealthImaging 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.HealthImaging 1.34.77 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 medical-imaging type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_medical_imaging": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

