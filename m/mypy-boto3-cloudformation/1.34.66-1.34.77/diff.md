# Comparing `tmp/mypy-boto3-cloudformation-1.34.66.tar.gz` & `tmp/mypy-boto3-cloudformation-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudformation-1.34.66.tar", last modified: Tue Mar 19 19:18:50 2024, max compression
+gzip compressed data, was "mypy-boto3-cloudformation-1.34.77.tar", last modified: Wed Apr  3 19:32:38 2024, max compression
```

## Comparing `mypy-boto3-cloudformation-1.34.66.tar` & `mypy-boto3-cloudformation-1.34.77.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:18:50.457375 mypy-boto3-cloudformation-1.34.66/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-03-19 19:18:50.457375 mypy-boto3-cloudformation-1.34.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:18:50.453375 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77001 2024-03-19 19:17:52.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    76998 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20978 2024-03-19 19:17:53.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    20978 2024-03-19 19:17:53.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22366 2024-03-19 19:17:52.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22347 2024-03-19 19:17:52.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-03-19 19:17:52.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    23302 2024-03-19 19:17:52.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    97790 2024-03-19 19:17:55.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    97790 2024-03-19 19:17:54.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-03-19 19:17:53.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-03-19 19:17:52.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:18:50.457375 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-03-19 19:18:50.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-19 19:18:50.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:18:50.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:18:50.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-19 19:18:50.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-19 19:18:50.000000 mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 19:18:50.457375 mypy-boto3-cloudformation-1.34.66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-19 19:17:51.000000 mypy-boto3-cloudformation-1.34.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77001 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76998 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21168 2024-04-03 19:32:01.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21168 2024-04-03 19:32:01.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22366 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22347 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23302 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    97867 2024-04-03 19:32:03.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97867 2024-04-03 19:32:02.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/setup.py
```

### Comparing `mypy-boto3-cloudformation-1.34.66/LICENSE` & `mypy-boto3-cloudformation-1.34.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/PKG-INFO` & `mypy-boto3-cloudformation-1.34.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.34.66
-Summary: Type annotations for boto3.CloudFormation 1.34.66 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.CloudFormation 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.34.66](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudformation-1.34.66/README.md` & `mypy-boto3-cloudformation-1.34.77/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.34.66](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/__init__.py` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/__init__.pyi` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/__main__.py` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFormation 1.34.66\n"
-        "Version:         1.34.66\n"
+        "Type annotations for boto3.CloudFormation 1.34.77\n"
+        "Version:         1.34.77\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.66")
+    print("1.34.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/client.py` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/client.pyi` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/literals.py` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "ListTypesPaginatorName",
     "OnFailureType",
     "OnStackFailureType",
     "OperationResultFilterNameType",
     "OperationStatusType",
     "OrganizationStatusType",
     "PermissionModelsType",
+    "PolicyActionType",
     "ProvisioningTypeType",
     "PublisherStatusType",
     "RegionConcurrencyTypeType",
     "RegistrationStatusType",
     "RegistryTypeType",
     "ReplacementType",
     "RequiresRecreationType",
@@ -219,14 +220,17 @@
 ListTypesPaginatorName = Literal["list_types"]
 OnFailureType = Literal["DELETE", "DO_NOTHING", "ROLLBACK"]
 OnStackFailureType = Literal["DELETE", "DO_NOTHING", "ROLLBACK"]
 OperationResultFilterNameType = Literal["OPERATION_RESULT_STATUS"]
 OperationStatusType = Literal["FAILED", "IN_PROGRESS", "PENDING", "SUCCESS"]
 OrganizationStatusType = Literal["DISABLED", "DISABLED_PERMANENTLY", "ENABLED"]
 PermissionModelsType = Literal["SELF_MANAGED", "SERVICE_MANAGED"]
+PolicyActionType = Literal[
+    "Delete", "ReplaceAndDelete", "ReplaceAndRetain", "ReplaceAndSnapshot", "Retain", "Snapshot"
+]
 ProvisioningTypeType = Literal["FULLY_MUTABLE", "IMMUTABLE", "NON_PROVISIONABLE"]
 PublisherStatusType = Literal["UNVERIFIED", "VERIFIED"]
 RegionConcurrencyTypeType = Literal["PARALLEL", "SEQUENTIAL"]
 RegistrationStatusType = Literal["COMPLETE", "FAILED", "IN_PROGRESS"]
 RegistryTypeType = Literal["HOOK", "MODULE", "RESOURCE"]
 ReplacementType = Literal["Conditional", "False", "True"]
 RequiresRecreationType = Literal["Always", "Conditionally", "Never"]
@@ -403,14 +407,15 @@
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
@@ -433,14 +438,15 @@
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
```

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/literals.pyi` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "ListTypesPaginatorName",
     "OnFailureType",
     "OnStackFailureType",
     "OperationResultFilterNameType",
     "OperationStatusType",
     "OrganizationStatusType",
     "PermissionModelsType",
+    "PolicyActionType",
     "ProvisioningTypeType",
     "PublisherStatusType",
     "RegionConcurrencyTypeType",
     "RegistrationStatusType",
     "RegistryTypeType",
     "ReplacementType",
     "RequiresRecreationType",
@@ -219,14 +220,17 @@
 ListTypesPaginatorName = Literal["list_types"]
 OnFailureType = Literal["DELETE", "DO_NOTHING", "ROLLBACK"]
 OnStackFailureType = Literal["DELETE", "DO_NOTHING", "ROLLBACK"]
 OperationResultFilterNameType = Literal["OPERATION_RESULT_STATUS"]
 OperationStatusType = Literal["FAILED", "IN_PROGRESS", "PENDING", "SUCCESS"]
 OrganizationStatusType = Literal["DISABLED", "DISABLED_PERMANENTLY", "ENABLED"]
 PermissionModelsType = Literal["SELF_MANAGED", "SERVICE_MANAGED"]
+PolicyActionType = Literal[
+    "Delete", "ReplaceAndDelete", "ReplaceAndRetain", "ReplaceAndSnapshot", "Retain", "Snapshot"
+]
 ProvisioningTypeType = Literal["FULLY_MUTABLE", "IMMUTABLE", "NON_PROVISIONABLE"]
 PublisherStatusType = Literal["UNVERIFIED", "VERIFIED"]
 RegionConcurrencyTypeType = Literal["PARALLEL", "SEQUENTIAL"]
 RegistrationStatusType = Literal["COMPLETE", "FAILED", "IN_PROGRESS"]
 RegistryTypeType = Literal["HOOK", "MODULE", "RESOURCE"]
 ReplacementType = Literal["Conditional", "False", "True"]
 RequiresRecreationType = Literal["Always", "Conditionally", "Never"]
@@ -403,14 +407,15 @@
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
@@ -433,14 +438,15 @@
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
```

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/paginator.py` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/paginator.pyi` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/service_resource.py` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/service_resource.pyi` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/type_defs.py` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     HookStatusType,
     IdentityProviderType,
     OnFailureType,
     OnStackFailureType,
     OperationStatusType,
     OrganizationStatusType,
     PermissionModelsType,
+    PolicyActionType,
     ProvisioningTypeType,
     PublisherStatusType,
     RegionConcurrencyTypeType,
     RegistrationStatusType,
     RegistryTypeType,
     ReplacementType,
     RequiresRecreationType,
@@ -2523,14 +2524,15 @@
         "StackResourceDrift": StackResourceDriftTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
+        "PolicyAction": NotRequired[PolicyActionType],
         "Action": NotRequired[ChangeActionType],
         "LogicalResourceId": NotRequired[str],
         "PhysicalResourceId": NotRequired[str],
         "ResourceType": NotRequired[str],
         "Replacement": NotRequired[ReplacementType],
         "Scope": NotRequired[List[ResourceAttributeType]],
         "Details": NotRequired[List[ResourceChangeDetailTypeDef]],
```

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/type_defs.pyi` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     HookStatusType,
     IdentityProviderType,
     OnFailureType,
     OnStackFailureType,
     OperationStatusType,
     OrganizationStatusType,
     PermissionModelsType,
+    PolicyActionType,
     ProvisioningTypeType,
     PublisherStatusType,
     RegionConcurrencyTypeType,
     RegistrationStatusType,
     RegistryTypeType,
     ReplacementType,
     RequiresRecreationType,
@@ -2523,14 +2524,15 @@
         "StackResourceDrift": StackResourceDriftTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
+        "PolicyAction": NotRequired[PolicyActionType],
         "Action": NotRequired[ChangeActionType],
         "LogicalResourceId": NotRequired[str],
         "PhysicalResourceId": NotRequired[str],
         "ResourceType": NotRequired[str],
         "Replacement": NotRequired[ReplacementType],
         "Scope": NotRequired[List[ResourceAttributeType]],
         "Details": NotRequired[List[ResourceChangeDetailTypeDef]],
```

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/waiter.py` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation/waiter.pyi` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/PKG-INFO` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.34.66
-Summary: Type annotations for boto3.CloudFormation 1.34.66 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.CloudFormation 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.34.66](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudformation-1.34.66/mypy_boto3_cloudformation.egg-info/SOURCES.txt` & `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.66/setup.py` & `mypy-boto3-cloudformation-1.34.77/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudformation",
-    version="1.34.66",
+    version="1.34.77",
     packages=["mypy_boto3_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CloudFormation 1.34.66 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CloudFormation 1.34.77 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

