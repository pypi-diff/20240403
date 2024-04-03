# Comparing `tmp/types-aiobotocore-sso-admin-2.9.0.tar.gz` & `tmp/types-aiobotocore-sso-admin-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sso-admin-2.9.0.tar", last modified: Wed Dec 13 20:00:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-sso-admin-2.9.1.tar", last modified: Thu Jan 18 01:21:54 2024, max compression
```

## Comparing `types-aiobotocore-sso-admin-2.9.0.tar` & `types-aiobotocore-sso-admin-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:36.677085 types-aiobotocore-sso-admin-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-13 20:00:36.677085 types-aiobotocore-sso-admin-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:36.677085 types-aiobotocore-sso-admin-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:36.677085 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66298 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    66294 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2023-12-13 19:57:02.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13863 2023-12-13 19:57:02.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27671 2023-12-13 19:57:02.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27649 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    57791 2023-12-13 19:57:03.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    57790 2023-12-13 19:57:02.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:01.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:36.677085 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-13 20:00:36.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 20:00:36.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:36.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:36.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:36.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 20:00:36.000000 types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:54.457009 types-aiobotocore-sso-admin-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-01-18 01:21:54.453009 types-aiobotocore-sso-admin-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:54.457009 types-aiobotocore-sso-admin-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:54.453009 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66323 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66320 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13863 2024-01-18 01:18:29.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13863 2024-01-18 01:18:29.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27682 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27661 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57790 2024-01-18 01:18:34.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57790 2024-01-18 01:18:33.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:28.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:54.453009 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-01-18 01:21:54.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:21:54.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:54.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:54.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:54.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:54.000000 types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/LICENSE` & `types-aiobotocore-sso-admin-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sso-admin-2.9.0/PKG-INFO` & `types-aiobotocore-sso-admin-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso-admin
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSOAdmin 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSOAdmin 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/
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
 
 <a id="types-aiobotocore-sso-admin"></a>
 
 # types-aiobotocore-sso-admin
 
 [![PyPI - types-aiobotocore-sso-admin](https://img.shields.io/pypi/v/types-aiobotocore-sso-admin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-admin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso-admin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso-admin)](https://pepy.tech/project/types-aiobotocore-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSOAdmin 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[aiobotocore.SSOAdmin 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [types-aiobotocore-sso-admin docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/README.md` & `types-aiobotocore-sso-admin-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso-admin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso-admin)](https://pepy.tech/project/types-aiobotocore-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSOAdmin 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[aiobotocore.SSOAdmin 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [types-aiobotocore-sso-admin docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/setup.py` & `types-aiobotocore-sso-admin-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sso-admin",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sso_admin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSOAdmin 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SSOAdmin 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore sso-admin type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sso_admin": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/__init__.py` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     ListPermissionSetsProvisionedToAccountPaginator,
     ListTagsForResourcePaginator,
     ListTrustedTokenIssuersPaginator,
 )
 
 Client = SSOAdminClient
 
-
 __all__ = (
     "Client",
     "ListAccountAssignmentCreationStatusPaginator",
     "ListAccountAssignmentDeletionStatusPaginator",
     "ListAccountAssignmentsForPrincipalPaginator",
     "ListAccountAssignmentsPaginator",
     "ListAccountsForProvisionedPermissionSetPaginator",
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/__init__.pyi` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/__main__.py` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSOAdmin 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SSOAdmin 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin\nOther"
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

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/client.py` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSOAdminClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -157,15 +156,15 @@
         """
 
     async def attach_customer_managed_policy_reference_to_permission_set(
         self,
         *,
         CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,
         InstanceArn: str,
-        PermissionSetArn: str
+        PermissionSetArn: str,
     ) -> Dict[str, Any]:
         """
         Attaches the specified customer managed policy to the specified  PermissionSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.attach_customer_managed_policy_reference_to_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#attach_customer_managed_policy_reference_to_permission_set)
         """
@@ -200,15 +199,15 @@
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         TargetId: str,
-        TargetType: Literal["AWS_ACCOUNT"]
+        TargetType: Literal["AWS_ACCOUNT"],
     ) -> CreateAccountAssignmentResponseTypeDef:
         """
         Assigns access to a principal for a specified Amazon Web Services account using
         a specified permission
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_account_assignment)
@@ -221,15 +220,15 @@
         ApplicationProviderArn: str,
         InstanceArn: str,
         Name: str,
         ClientToken: str = ...,
         Description: str = ...,
         PortalOptions: PortalOptionsTypeDef = ...,
         Status: ApplicationStatusType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application in IAM Identity Center for the given application
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_application)
@@ -258,15 +257,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_instance)
         """
 
     async def create_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,
-        InstanceArn: str
+        InstanceArn: str,
     ) -> Dict[str, Any]:
         """
         Enables the attributes-based access control (ABAC) feature for the specified
         IAM Identity Center
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_instance_access_control_attribute_configuration)
@@ -277,15 +276,15 @@
         self,
         *,
         InstanceArn: str,
         Name: str,
         Description: str = ...,
         RelayState: str = ...,
         SessionDuration: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePermissionSetResponseTypeDef:
         """
         Creates a permission set within a specified IAM Identity Center instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_permission_set)
         """
@@ -294,15 +293,15 @@
         self,
         *,
         InstanceArn: str,
         Name: str,
         TrustedTokenIssuerConfiguration: TrustedTokenIssuerConfigurationTypeDef,
         TrustedTokenIssuerType: Literal["OIDC_JWT"],
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrustedTokenIssuerResponseTypeDef:
         """
         Creates a connection to a trusted token issuer in an instance of IAM Identity
         Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_trusted_token_issuer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_trusted_token_issuer)
@@ -312,15 +311,15 @@
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         TargetId: str,
-        TargetType: Literal["AWS_ACCOUNT"]
+        TargetType: Literal["AWS_ACCOUNT"],
     ) -> DeleteAccountAssignmentResponseTypeDef:
         """
         Deletes a principal's access from a specified Amazon Web Services account using
         a specified permission
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.delete_account_assignment)
@@ -545,15 +544,15 @@
         """
 
     async def detach_customer_managed_policy_reference_from_permission_set(
         self,
         *,
         CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,
         InstanceArn: str,
-        PermissionSetArn: str
+        PermissionSetArn: str,
     ) -> Dict[str, Any]:
         """
         Detaches the specified customer managed policy from the specified
         PermissionSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.detach_customer_managed_policy_reference_from_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#detach_customer_managed_policy_reference_from_permission_set)
@@ -648,15 +647,15 @@
 
     async def list_account_assignment_creation_status(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssignmentCreationStatusResponseTypeDef:
         """
         Lists the status of the Amazon Web Services account assignment creation
         requests for a specified IAM Identity Center
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_account_assignment_creation_status)
@@ -665,15 +664,15 @@
 
     async def list_account_assignment_deletion_status(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssignmentDeletionStatusResponseTypeDef:
         """
         Lists the status of the Amazon Web Services account assignment deletion
         requests for a specified IAM Identity Center
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_account_assignment_deletion_status)
@@ -683,15 +682,15 @@
     async def list_account_assignments(
         self,
         *,
         AccountId: str,
         InstanceArn: str,
         PermissionSetArn: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssignmentsResponseTypeDef:
         """
         Lists the assignee of the specified Amazon Web Services account with the
         specified permission
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_account_assignments)
@@ -702,15 +701,15 @@
         self,
         *,
         InstanceArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         Filter: ListAccountAssignmentsFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssignmentsForPrincipalResponseTypeDef:
         """
         Retrieves a list of the IAM Identity Center associated Amazon Web Services
         accounts that the principal has access
         to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_account_assignments_for_principal)
@@ -720,15 +719,15 @@
     async def list_accounts_for_provisioned_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ProvisioningStatus: ProvisioningStatusType = ...
+        ProvisioningStatus: ProvisioningStatusType = ...,
     ) -> ListAccountsForProvisionedPermissionSetResponseTypeDef:
         """
         Lists all the Amazon Web Services accounts where the specified permission set
         is
         provisioned.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_accounts_for_provisioned_permission_set)
@@ -759,15 +758,15 @@
         self,
         *,
         InstanceArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         Filter: ListApplicationAssignmentsFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListApplicationAssignmentsForPrincipalResponseTypeDef:
         """
         Lists the applications to which a specified principal is assigned.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_application_assignments_for_principal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#list_application_assignments_for_principal)
         """
@@ -805,30 +804,30 @@
 
     async def list_applications(
         self,
         *,
         InstanceArn: str,
         Filter: ListApplicationsFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists all applications associated with the instance of IAM Identity Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#list_applications)
         """
 
     async def list_customer_managed_policy_references_in_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef:
         """
         Lists all customer managed policies attached to a specified  PermissionSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_customer_managed_policy_references_in_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#list_customer_managed_policy_references_in_permission_set)
         """
@@ -847,15 +846,15 @@
 
     async def list_managed_policies_in_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListManagedPoliciesInPermissionSetResponseTypeDef:
         """
         Lists the Amazon Web Services managed policy that is attached to a specified
         permission
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_managed_policies_in_permission_set)
@@ -864,15 +863,15 @@
 
     async def list_permission_set_provisioning_status(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPermissionSetProvisioningStatusResponseTypeDef:
         """
         Lists the status of the permission set provisioning requests for a specified
         IAM Identity Center
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_permission_set_provisioning_status)
@@ -892,15 +891,15 @@
     async def list_permission_sets_provisioned_to_account(
         self,
         *,
         AccountId: str,
         InstanceArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ProvisioningStatus: ProvisioningStatusType = ...
+        ProvisioningStatus: ProvisioningStatusType = ...,
     ) -> ListPermissionSetsProvisionedToAccountResponseTypeDef:
         """
         Lists all the permission sets that are provisioned to a specified Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_permission_sets_provisioned_to_account)
@@ -930,15 +929,15 @@
 
     async def provision_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         TargetType: ProvisionTargetTypeType,
-        TargetId: str = ...
+        TargetId: str = ...,
     ) -> ProvisionPermissionSetResponseTypeDef:
         """
         The process by which a specified permission set is provisioned to the specified
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.provision_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#provision_permission_set)
@@ -967,15 +966,15 @@
         """
 
     async def put_application_authentication_method(
         self,
         *,
         ApplicationArn: str,
         AuthenticationMethod: AuthenticationMethodTypeDef,
-        AuthenticationMethodType: Literal["IAM"]
+        AuthenticationMethodType: Literal["IAM"],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an authentication method for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.put_application_authentication_method)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#put_application_authentication_method)
         """
@@ -1001,15 +1000,15 @@
         """
 
     async def put_permissions_boundary_to_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PermissionsBoundary: PermissionsBoundaryTypeDef
+        PermissionsBoundary: PermissionsBoundaryTypeDef,
     ) -> Dict[str, Any]:
         """
         Attaches an Amazon Web Services managed or customer managed policy to the
         specified  PermissionSet as a permissions
         boundary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.put_permissions_boundary_to_permission_set)
@@ -1039,15 +1038,15 @@
     async def update_application(
         self,
         *,
         ApplicationArn: str,
         Description: str = ...,
         Name: str = ...,
         PortalOptions: UpdateApplicationPortalOptionsTypeDef = ...,
-        Status: ApplicationStatusType = ...
+        Status: ApplicationStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Updates application properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#update_application)
         """
@@ -1062,15 +1061,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#update_instance)
         """
 
     async def update_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,
-        InstanceArn: str
+        InstanceArn: str,
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center identity store attributes that you can use with
         the IAM Identity Center instance for attributes-based access control
         (ABAC).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_instance_access_control_attribute_configuration)
@@ -1080,29 +1079,29 @@
     async def update_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         Description: str = ...,
         RelayState: str = ...,
-        SessionDuration: str = ...
+        SessionDuration: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing permission set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#update_permission_set)
         """
 
     async def update_trusted_token_issuer(
         self,
         *,
         TrustedTokenIssuerArn: str,
         Name: str = ...,
-        TrustedTokenIssuerConfiguration: TrustedTokenIssuerUpdateConfigurationTypeDef = ...
+        TrustedTokenIssuerConfiguration: TrustedTokenIssuerUpdateConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the name of the trusted token issuer, or the path of a source attribute
         or destination attribute for a trusted token issuer
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_trusted_token_issuer)
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/client.pyi` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         """
 
     async def attach_customer_managed_policy_reference_to_permission_set(
         self,
         *,
         CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,
         InstanceArn: str,
-        PermissionSetArn: str
+        PermissionSetArn: str,
     ) -> Dict[str, Any]:
         """
         Attaches the specified customer managed policy to the specified  PermissionSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.attach_customer_managed_policy_reference_to_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#attach_customer_managed_policy_reference_to_permission_set)
         """
@@ -196,15 +196,15 @@
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         TargetId: str,
-        TargetType: Literal["AWS_ACCOUNT"]
+        TargetType: Literal["AWS_ACCOUNT"],
     ) -> CreateAccountAssignmentResponseTypeDef:
         """
         Assigns access to a principal for a specified Amazon Web Services account using
         a specified permission
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_account_assignment)
@@ -217,15 +217,15 @@
         ApplicationProviderArn: str,
         InstanceArn: str,
         Name: str,
         ClientToken: str = ...,
         Description: str = ...,
         PortalOptions: PortalOptionsTypeDef = ...,
         Status: ApplicationStatusType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application in IAM Identity Center for the given application
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_application)
@@ -254,15 +254,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_instance)
         """
 
     async def create_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,
-        InstanceArn: str
+        InstanceArn: str,
     ) -> Dict[str, Any]:
         """
         Enables the attributes-based access control (ABAC) feature for the specified
         IAM Identity Center
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_instance_access_control_attribute_configuration)
@@ -273,15 +273,15 @@
         self,
         *,
         InstanceArn: str,
         Name: str,
         Description: str = ...,
         RelayState: str = ...,
         SessionDuration: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePermissionSetResponseTypeDef:
         """
         Creates a permission set within a specified IAM Identity Center instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_permission_set)
         """
@@ -290,15 +290,15 @@
         self,
         *,
         InstanceArn: str,
         Name: str,
         TrustedTokenIssuerConfiguration: TrustedTokenIssuerConfigurationTypeDef,
         TrustedTokenIssuerType: Literal["OIDC_JWT"],
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrustedTokenIssuerResponseTypeDef:
         """
         Creates a connection to a trusted token issuer in an instance of IAM Identity
         Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_trusted_token_issuer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_trusted_token_issuer)
@@ -308,15 +308,15 @@
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         TargetId: str,
-        TargetType: Literal["AWS_ACCOUNT"]
+        TargetType: Literal["AWS_ACCOUNT"],
     ) -> DeleteAccountAssignmentResponseTypeDef:
         """
         Deletes a principal's access from a specified Amazon Web Services account using
         a specified permission
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.delete_account_assignment)
@@ -541,15 +541,15 @@
         """
 
     async def detach_customer_managed_policy_reference_from_permission_set(
         self,
         *,
         CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,
         InstanceArn: str,
-        PermissionSetArn: str
+        PermissionSetArn: str,
     ) -> Dict[str, Any]:
         """
         Detaches the specified customer managed policy from the specified
         PermissionSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.detach_customer_managed_policy_reference_from_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#detach_customer_managed_policy_reference_from_permission_set)
@@ -644,15 +644,15 @@
 
     async def list_account_assignment_creation_status(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssignmentCreationStatusResponseTypeDef:
         """
         Lists the status of the Amazon Web Services account assignment creation
         requests for a specified IAM Identity Center
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_account_assignment_creation_status)
@@ -661,15 +661,15 @@
 
     async def list_account_assignment_deletion_status(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssignmentDeletionStatusResponseTypeDef:
         """
         Lists the status of the Amazon Web Services account assignment deletion
         requests for a specified IAM Identity Center
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_account_assignment_deletion_status)
@@ -679,15 +679,15 @@
     async def list_account_assignments(
         self,
         *,
         AccountId: str,
         InstanceArn: str,
         PermissionSetArn: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssignmentsResponseTypeDef:
         """
         Lists the assignee of the specified Amazon Web Services account with the
         specified permission
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_account_assignments)
@@ -698,15 +698,15 @@
         self,
         *,
         InstanceArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         Filter: ListAccountAssignmentsFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssignmentsForPrincipalResponseTypeDef:
         """
         Retrieves a list of the IAM Identity Center associated Amazon Web Services
         accounts that the principal has access
         to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_account_assignments_for_principal)
@@ -716,15 +716,15 @@
     async def list_accounts_for_provisioned_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ProvisioningStatus: ProvisioningStatusType = ...
+        ProvisioningStatus: ProvisioningStatusType = ...,
     ) -> ListAccountsForProvisionedPermissionSetResponseTypeDef:
         """
         Lists all the Amazon Web Services accounts where the specified permission set
         is
         provisioned.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_accounts_for_provisioned_permission_set)
@@ -755,15 +755,15 @@
         self,
         *,
         InstanceArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         Filter: ListApplicationAssignmentsFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListApplicationAssignmentsForPrincipalResponseTypeDef:
         """
         Lists the applications to which a specified principal is assigned.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_application_assignments_for_principal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#list_application_assignments_for_principal)
         """
@@ -801,30 +801,30 @@
 
     async def list_applications(
         self,
         *,
         InstanceArn: str,
         Filter: ListApplicationsFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists all applications associated with the instance of IAM Identity Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#list_applications)
         """
 
     async def list_customer_managed_policy_references_in_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef:
         """
         Lists all customer managed policies attached to a specified  PermissionSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_customer_managed_policy_references_in_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#list_customer_managed_policy_references_in_permission_set)
         """
@@ -843,15 +843,15 @@
 
     async def list_managed_policies_in_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListManagedPoliciesInPermissionSetResponseTypeDef:
         """
         Lists the Amazon Web Services managed policy that is attached to a specified
         permission
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_managed_policies_in_permission_set)
@@ -860,15 +860,15 @@
 
     async def list_permission_set_provisioning_status(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPermissionSetProvisioningStatusResponseTypeDef:
         """
         Lists the status of the permission set provisioning requests for a specified
         IAM Identity Center
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_permission_set_provisioning_status)
@@ -888,15 +888,15 @@
     async def list_permission_sets_provisioned_to_account(
         self,
         *,
         AccountId: str,
         InstanceArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ProvisioningStatus: ProvisioningStatusType = ...
+        ProvisioningStatus: ProvisioningStatusType = ...,
     ) -> ListPermissionSetsProvisionedToAccountResponseTypeDef:
         """
         Lists all the permission sets that are provisioned to a specified Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_permission_sets_provisioned_to_account)
@@ -926,15 +926,15 @@
 
     async def provision_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         TargetType: ProvisionTargetTypeType,
-        TargetId: str = ...
+        TargetId: str = ...,
     ) -> ProvisionPermissionSetResponseTypeDef:
         """
         The process by which a specified permission set is provisioned to the specified
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.provision_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#provision_permission_set)
@@ -963,15 +963,15 @@
         """
 
     async def put_application_authentication_method(
         self,
         *,
         ApplicationArn: str,
         AuthenticationMethod: AuthenticationMethodTypeDef,
-        AuthenticationMethodType: Literal["IAM"]
+        AuthenticationMethodType: Literal["IAM"],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an authentication method for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.put_application_authentication_method)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#put_application_authentication_method)
         """
@@ -997,15 +997,15 @@
         """
 
     async def put_permissions_boundary_to_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PermissionsBoundary: PermissionsBoundaryTypeDef
+        PermissionsBoundary: PermissionsBoundaryTypeDef,
     ) -> Dict[str, Any]:
         """
         Attaches an Amazon Web Services managed or customer managed policy to the
         specified  PermissionSet as a permissions
         boundary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.put_permissions_boundary_to_permission_set)
@@ -1035,15 +1035,15 @@
     async def update_application(
         self,
         *,
         ApplicationArn: str,
         Description: str = ...,
         Name: str = ...,
         PortalOptions: UpdateApplicationPortalOptionsTypeDef = ...,
-        Status: ApplicationStatusType = ...
+        Status: ApplicationStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Updates application properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#update_application)
         """
@@ -1058,15 +1058,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#update_instance)
         """
 
     async def update_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,
-        InstanceArn: str
+        InstanceArn: str,
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center identity store attributes that you can use with
         the IAM Identity Center instance for attributes-based access control
         (ABAC).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_instance_access_control_attribute_configuration)
@@ -1076,29 +1076,29 @@
     async def update_permission_set(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         Description: str = ...,
         RelayState: str = ...,
-        SessionDuration: str = ...
+        SessionDuration: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing permission set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_permission_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#update_permission_set)
         """
 
     async def update_trusted_token_issuer(
         self,
         *,
         TrustedTokenIssuerArn: str,
         Name: str = ...,
-        TrustedTokenIssuerConfiguration: TrustedTokenIssuerUpdateConfigurationTypeDef = ...
+        TrustedTokenIssuerConfiguration: TrustedTokenIssuerUpdateConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the name of the trusted token issuer, or the path of a source attribute
         or destination attribute for a trusted token issuer
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_trusted_token_issuer)
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/literals.py` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/literals.py`

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
     "ApplicationStatusType",
     "ApplicationVisibilityType",
     "AuthenticationMethodTypeType",
     "FederationProtocolType",
     "GrantTypeType",
     "InstanceAccessControlAttributeConfigurationStatusType",
@@ -59,15 +58,14 @@
     "SSOAdminServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStatusType = Literal["DISABLED", "ENABLED"]
 ApplicationVisibilityType = Literal["DISABLED", "ENABLED"]
 AuthenticationMethodTypeType = Literal["IAM"]
 FederationProtocolType = Literal["OAUTH", "SAML"]
 GrantTypeType = Literal[
     "authorization_code",
     "refresh_token",
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/literals.pyi` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/paginator.py` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     "ListPermissionSetProvisioningStatusPaginator",
     "ListPermissionSetsPaginator",
     "ListPermissionSetsProvisionedToAccountPaginator",
     "ListTagsForResourcePaginator",
     "ListTrustedTokenIssuersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -134,15 +133,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssignmentCreationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentCreationStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountassignmentcreationstatuspaginator)
         """
 
 
@@ -153,15 +152,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssignmentDeletionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentDeletionStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountassignmentdeletionstatuspaginator)
         """
 
 
@@ -173,15 +172,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssignmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountassignmentspaginator)
         """
 
 
@@ -194,15 +193,15 @@
     def paginate(
         self,
         *,
         InstanceArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         Filter: ListAccountAssignmentsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssignmentsForPrincipalResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentsForPrincipal.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountassignmentsforprincipalpaginator)
         """
 
 
@@ -214,15 +213,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountsForProvisionedPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountsForProvisionedPermissionSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountsforprovisionedpermissionsetpaginator)
         """
 
 
@@ -265,15 +264,15 @@
     def paginate(
         self,
         *,
         InstanceArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         Filter: ListApplicationAssignmentsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationAssignmentsForPrincipalResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListApplicationAssignmentsForPrincipal.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listapplicationassignmentsforprincipalpaginator)
         """
 
 
@@ -329,15 +328,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: ListApplicationsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listapplicationspaginator)
         """
 
 
@@ -348,15 +347,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListCustomerManagedPolicyReferencesInPermissionSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listcustomermanagedpolicyreferencesinpermissionsetpaginator)
         """
 
 
@@ -382,15 +381,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListManagedPoliciesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListManagedPoliciesInPermissionSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listmanagedpoliciesinpermissionsetpaginator)
         """
 
 
@@ -401,15 +400,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPermissionSetProvisioningStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetProvisioningStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listpermissionsetprovisioningstatuspaginator)
         """
 
 
@@ -436,15 +435,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         InstanceArn: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPermissionSetsProvisionedToAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetsProvisionedToAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listpermissionsetsprovisionedtoaccountpaginator)
         """
 
 
@@ -455,15 +454,15 @@
     """
 
     def paginate(
         self,
         *,
         ResourceArn: str,
         InstanceArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/paginator.pyi` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssignmentCreationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentCreationStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountassignmentcreationstatuspaginator)
         """
 
 class ListAccountAssignmentDeletionStatusPaginator(AioPaginator):
@@ -149,15 +149,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssignmentDeletionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentDeletionStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountassignmentdeletionstatuspaginator)
         """
 
 class ListAccountAssignmentsPaginator(AioPaginator):
@@ -168,15 +168,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssignmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountassignmentspaginator)
         """
 
 class ListAccountAssignmentsForPrincipalPaginator(AioPaginator):
@@ -188,15 +188,15 @@
     def paginate(
         self,
         *,
         InstanceArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         Filter: ListAccountAssignmentsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssignmentsForPrincipalResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentsForPrincipal.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountassignmentsforprincipalpaginator)
         """
 
 class ListAccountsForProvisionedPermissionSetPaginator(AioPaginator):
@@ -207,15 +207,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountsForProvisionedPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountsForProvisionedPermissionSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listaccountsforprovisionedpermissionsetpaginator)
         """
 
 class ListApplicationAccessScopesPaginator(AioPaginator):
@@ -255,15 +255,15 @@
     def paginate(
         self,
         *,
         InstanceArn: str,
         PrincipalId: str,
         PrincipalType: PrincipalTypeType,
         Filter: ListApplicationAssignmentsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationAssignmentsForPrincipalResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListApplicationAssignmentsForPrincipal.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listapplicationassignmentsforprincipalpaginator)
         """
 
 class ListApplicationAuthenticationMethodsPaginator(AioPaginator):
@@ -315,15 +315,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: ListApplicationsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listapplicationspaginator)
         """
 
 class ListCustomerManagedPolicyReferencesInPermissionSetPaginator(AioPaginator):
@@ -333,15 +333,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListCustomerManagedPolicyReferencesInPermissionSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listcustomermanagedpolicyreferencesinpermissionsetpaginator)
         """
 
 class ListInstancesPaginator(AioPaginator):
@@ -365,15 +365,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListManagedPoliciesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListManagedPoliciesInPermissionSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listmanagedpoliciesinpermissionsetpaginator)
         """
 
 class ListPermissionSetProvisioningStatusPaginator(AioPaginator):
@@ -383,15 +383,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPermissionSetProvisioningStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetProvisioningStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listpermissionsetprovisioningstatuspaginator)
         """
 
 class ListPermissionSetsPaginator(AioPaginator):
@@ -416,15 +416,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         InstanceArn: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPermissionSetsProvisionedToAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetsProvisionedToAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listpermissionsetsprovisionedtoaccountpaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
@@ -434,15 +434,15 @@
     """
 
     def paginate(
         self,
         *,
         ResourceArn: str,
         InstanceArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTrustedTokenIssuersPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/type_defs.py` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessControlAttributeValueTypeDef",
     "AccountAssignmentForPrincipalTypeDef",
     "AccountAssignmentOperationStatusMetadataTypeDef",
     "AccountAssignmentOperationStatusTypeDef",
     "AccountAssignmentTypeDef",
     "ApplicationAssignmentForPrincipalTypeDef",
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin/type_defs.pyi` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/PKG-INFO` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso-admin
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSOAdmin 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSOAdmin 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/
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
 
 <a id="types-aiobotocore-sso-admin"></a>
 
 # types-aiobotocore-sso-admin
 
 [![PyPI - types-aiobotocore-sso-admin](https://img.shields.io/pypi/v/types-aiobotocore-sso-admin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-admin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso-admin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso-admin)](https://pepy.tech/project/types-aiobotocore-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSOAdmin 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[aiobotocore.SSOAdmin 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [types-aiobotocore-sso-admin docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sso-admin-2.9.0/types_aiobotocore_sso_admin.egg-info/SOURCES.txt` & `types-aiobotocore-sso-admin-2.9.1/types_aiobotocore_sso_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

