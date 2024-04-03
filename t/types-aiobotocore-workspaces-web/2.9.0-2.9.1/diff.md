# Comparing `tmp/types-aiobotocore-workspaces-web-2.9.0.tar.gz` & `tmp/types-aiobotocore-workspaces-web-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workspaces-web-2.9.0.tar", last modified: Wed Dec 13 20:00:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-workspaces-web-2.9.1.tar", last modified: Thu Jan 18 01:22:05 2024, max compression
```

## Comparing `types-aiobotocore-workspaces-web-2.9.0.tar` & `types-aiobotocore-workspaces-web-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:48.624982 types-aiobotocore-workspaces-web-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-12-13 20:00:48.624982 types-aiobotocore-workspaces-web-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11057 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:48.624982 types-aiobotocore-workspaces-web-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:48.624982 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40682 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    40679 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8910 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    36130 2023-12-13 19:58:10.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    36129 2023-12-13 19:58:10.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:48.624982 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.348959 types-aiobotocore-workspaces-web-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-01-18 01:22:05.348959 types-aiobotocore-workspaces-web-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:05.348959 types-aiobotocore-workspaces-web-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.348959 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40696 2024-01-18 01:19:35.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40693 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-01-18 01:19:35.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-01-18 01:19:35.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    36129 2024-01-18 01:19:35.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36129 2024-01-18 01:19:35.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.348959 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-01-18 01:22:05.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-18 01:22:05.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:05.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:05.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:05.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:22:05.000000 types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/LICENSE` & `types-aiobotocore-workspaces-web-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-workspaces-web-2.9.0/PKG-INFO` & `types-aiobotocore-workspaces-web-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces-web
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkSpacesWeb 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkSpacesWeb 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/
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
 
 <a id="types-aiobotocore-workspaces-web"></a>
 
 # types-aiobotocore-workspaces-web
 
 [![PyPI - types-aiobotocore-workspaces-web](https://img.shields.io/pypi/v/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-web)](https://pepy.tech/project/types-aiobotocore-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpacesWeb 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[aiobotocore.WorkSpacesWeb 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [types-aiobotocore-workspaces-web docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/README.md` & `types-aiobotocore-workspaces-web-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-web)](https://pepy.tech/project/types-aiobotocore-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpacesWeb 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[aiobotocore.WorkSpacesWeb 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [types-aiobotocore-workspaces-web docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/setup.py` & `types-aiobotocore-workspaces-web-2.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workspaces-web",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_workspaces_web"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkSpacesWeb 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.WorkSpacesWeb 2.9.1 service generated with"
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
     keywords="aiobotocore workspaces-web type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_workspaces_web": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/__main__.py` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkSpacesWeb 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WorkSpacesWeb 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb\nOther"
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

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/client.py` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     async def create_browser_settings(
         self,
         *,
         browserPolicy: str,
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBrowserSettingsResponseTypeDef:
         """
         Creates a browser settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_browser_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_browser_settings)
         """
@@ -205,15 +205,15 @@
     async def create_identity_provider(
         self,
         *,
         identityProviderDetails: Mapping[str, str],
         identityProviderName: str,
         identityProviderType: IdentityProviderTypeType,
         portalArn: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an identity provider resource that is then associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_identity_provider)
         """
@@ -223,15 +223,15 @@
         *,
         ipRules: Sequence[IpRuleTypeDef],
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
         description: str = ...,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIpAccessSettingsResponseTypeDef:
         """
         Creates an IP access settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_ip_access_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_ip_access_settings)
         """
@@ -239,15 +239,15 @@
     async def create_network_settings(
         self,
         *,
         securityGroupIds: Sequence[str],
         subnetIds: Sequence[str],
         vpcId: str,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNetworkSettingsResponseTypeDef:
         """
         Creates a network settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_network_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_network_settings)
         """
@@ -256,29 +256,29 @@
         self,
         *,
         additionalEncryptionContext: Mapping[str, str] = ...,
         authenticationType: AuthenticationTypeType = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePortalResponseTypeDef:
         """
         Creates a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_portal)
         """
 
     async def create_trust_store(
         self,
         *,
         certificateList: Sequence[BlobTypeDef],
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrustStoreResponseTypeDef:
         """
         Creates a trust store that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_trust_store)
         """
@@ -305,15 +305,15 @@
         uploadAllowed: EnabledTypeType,
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         cookieSynchronizationConfiguration: CookieSynchronizationConfigurationTypeDef = ...,
         customerManagedKey: str = ...,
         disconnectTimeoutInMinutes: int = ...,
         idleDisconnectTimeoutInMinutes: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserSettingsResponseTypeDef:
         """
         Creates a user settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_user_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_user_settings)
         """
@@ -671,15 +671,15 @@
     async def update_identity_provider(
         self,
         *,
         identityProviderArn: str,
         clientToken: str = ...,
         identityProviderDetails: Mapping[str, str] = ...,
         identityProviderName: str = ...,
-        identityProviderType: IdentityProviderTypeType = ...
+        identityProviderType: IdentityProviderTypeType = ...,
     ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_identity_provider)
         """
@@ -687,15 +687,15 @@
     async def update_ip_access_settings(
         self,
         *,
         ipAccessSettingsArn: str,
         clientToken: str = ...,
         description: str = ...,
         displayName: str = ...,
-        ipRules: Sequence[IpRuleTypeDef] = ...
+        ipRules: Sequence[IpRuleTypeDef] = ...,
     ) -> UpdateIpAccessSettingsResponseTypeDef:
         """
         Updates IP access settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_ip_access_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_ip_access_settings)
         """
@@ -703,58 +703,58 @@
     async def update_network_settings(
         self,
         *,
         networkSettingsArn: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
         subnetIds: Sequence[str] = ...,
-        vpcId: str = ...
+        vpcId: str = ...,
     ) -> UpdateNetworkSettingsResponseTypeDef:
         """
         Updates network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_network_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_network_settings)
         """
 
     async def update_portal(
         self,
         *,
         portalArn: str,
         authenticationType: AuthenticationTypeType = ...,
-        displayName: str = ...
+        displayName: str = ...,
     ) -> UpdatePortalResponseTypeDef:
         """
         Updates a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_portal)
         """
 
     async def update_trust_store(
         self,
         *,
         trustStoreArn: str,
         certificatesToAdd: Sequence[BlobTypeDef] = ...,
         certificatesToDelete: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateTrustStoreResponseTypeDef:
         """
         Updates the trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_trust_store)
         """
 
     async def update_user_access_logging_settings(
         self,
         *,
         userAccessLoggingSettingsArn: str,
         clientToken: str = ...,
-        kinesisStreamArn: str = ...
+        kinesisStreamArn: str = ...,
     ) -> UpdateUserAccessLoggingSettingsResponseTypeDef:
         """
         Updates the user access logging settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_access_logging_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_user_access_logging_settings)
         """
@@ -767,15 +767,15 @@
         cookieSynchronizationConfiguration: CookieSynchronizationConfigurationTypeDef = ...,
         copyAllowed: EnabledTypeType = ...,
         disconnectTimeoutInMinutes: int = ...,
         downloadAllowed: EnabledTypeType = ...,
         idleDisconnectTimeoutInMinutes: int = ...,
         pasteAllowed: EnabledTypeType = ...,
         printAllowed: EnabledTypeType = ...,
-        uploadAllowed: EnabledTypeType = ...
+        uploadAllowed: EnabledTypeType = ...,
     ) -> UpdateUserSettingsResponseTypeDef:
         """
         Updates the user settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_user_settings)
         """
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/client.pyi` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     async def create_browser_settings(
         self,
         *,
         browserPolicy: str,
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBrowserSettingsResponseTypeDef:
         """
         Creates a browser settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_browser_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_browser_settings)
         """
@@ -202,15 +202,15 @@
     async def create_identity_provider(
         self,
         *,
         identityProviderDetails: Mapping[str, str],
         identityProviderName: str,
         identityProviderType: IdentityProviderTypeType,
         portalArn: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an identity provider resource that is then associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_identity_provider)
         """
@@ -220,15 +220,15 @@
         *,
         ipRules: Sequence[IpRuleTypeDef],
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
         description: str = ...,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIpAccessSettingsResponseTypeDef:
         """
         Creates an IP access settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_ip_access_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_ip_access_settings)
         """
@@ -236,15 +236,15 @@
     async def create_network_settings(
         self,
         *,
         securityGroupIds: Sequence[str],
         subnetIds: Sequence[str],
         vpcId: str,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNetworkSettingsResponseTypeDef:
         """
         Creates a network settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_network_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_network_settings)
         """
@@ -253,29 +253,29 @@
         self,
         *,
         additionalEncryptionContext: Mapping[str, str] = ...,
         authenticationType: AuthenticationTypeType = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePortalResponseTypeDef:
         """
         Creates a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_portal)
         """
 
     async def create_trust_store(
         self,
         *,
         certificateList: Sequence[BlobTypeDef],
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrustStoreResponseTypeDef:
         """
         Creates a trust store that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_trust_store)
         """
@@ -302,15 +302,15 @@
         uploadAllowed: EnabledTypeType,
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         cookieSynchronizationConfiguration: CookieSynchronizationConfigurationTypeDef = ...,
         customerManagedKey: str = ...,
         disconnectTimeoutInMinutes: int = ...,
         idleDisconnectTimeoutInMinutes: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserSettingsResponseTypeDef:
         """
         Creates a user settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_user_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#create_user_settings)
         """
@@ -668,15 +668,15 @@
     async def update_identity_provider(
         self,
         *,
         identityProviderArn: str,
         clientToken: str = ...,
         identityProviderDetails: Mapping[str, str] = ...,
         identityProviderName: str = ...,
-        identityProviderType: IdentityProviderTypeType = ...
+        identityProviderType: IdentityProviderTypeType = ...,
     ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_identity_provider)
         """
@@ -684,15 +684,15 @@
     async def update_ip_access_settings(
         self,
         *,
         ipAccessSettingsArn: str,
         clientToken: str = ...,
         description: str = ...,
         displayName: str = ...,
-        ipRules: Sequence[IpRuleTypeDef] = ...
+        ipRules: Sequence[IpRuleTypeDef] = ...,
     ) -> UpdateIpAccessSettingsResponseTypeDef:
         """
         Updates IP access settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_ip_access_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_ip_access_settings)
         """
@@ -700,58 +700,58 @@
     async def update_network_settings(
         self,
         *,
         networkSettingsArn: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
         subnetIds: Sequence[str] = ...,
-        vpcId: str = ...
+        vpcId: str = ...,
     ) -> UpdateNetworkSettingsResponseTypeDef:
         """
         Updates network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_network_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_network_settings)
         """
 
     async def update_portal(
         self,
         *,
         portalArn: str,
         authenticationType: AuthenticationTypeType = ...,
-        displayName: str = ...
+        displayName: str = ...,
     ) -> UpdatePortalResponseTypeDef:
         """
         Updates a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_portal)
         """
 
     async def update_trust_store(
         self,
         *,
         trustStoreArn: str,
         certificatesToAdd: Sequence[BlobTypeDef] = ...,
         certificatesToDelete: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateTrustStoreResponseTypeDef:
         """
         Updates the trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_trust_store)
         """
 
     async def update_user_access_logging_settings(
         self,
         *,
         userAccessLoggingSettingsArn: str,
         clientToken: str = ...,
-        kinesisStreamArn: str = ...
+        kinesisStreamArn: str = ...,
     ) -> UpdateUserAccessLoggingSettingsResponseTypeDef:
         """
         Updates the user access logging settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_access_logging_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_user_access_logging_settings)
         """
@@ -764,15 +764,15 @@
         cookieSynchronizationConfiguration: CookieSynchronizationConfigurationTypeDef = ...,
         copyAllowed: EnabledTypeType = ...,
         disconnectTimeoutInMinutes: int = ...,
         downloadAllowed: EnabledTypeType = ...,
         idleDisconnectTimeoutInMinutes: int = ...,
         pasteAllowed: EnabledTypeType = ...,
         printAllowed: EnabledTypeType = ...,
-        uploadAllowed: EnabledTypeType = ...
+        uploadAllowed: EnabledTypeType = ...,
     ) -> UpdateUserSettingsResponseTypeDef:
         """
         Updates the user settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/client/#update_user_settings)
         """
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/literals.py` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthenticationTypeType",
     "BrowserTypeType",
     "EnabledTypeType",
     "IdentityProviderTypeType",
     "PortalStatusType",
     "RendererTypeType",
     "WorkSpacesWebServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AuthenticationTypeType = Literal["IAM_Identity_Center", "Standard"]
 BrowserTypeType = Literal["Chrome"]
 EnabledTypeType = Literal["Disabled", "Enabled"]
 IdentityProviderTypeType = Literal[
     "Facebook", "Google", "LoginWithAmazon", "OIDC", "SAML", "SignInWithApple"
 ]
 PortalStatusType = Literal["Active", "Incomplete", "Pending"]
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/literals.pyi` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/type_defs.py` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web/type_defs.pyi` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/PKG-INFO` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces-web
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkSpacesWeb 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkSpacesWeb 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/
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
 
 <a id="types-aiobotocore-workspaces-web"></a>
 
 # types-aiobotocore-workspaces-web
 
 [![PyPI - types-aiobotocore-workspaces-web](https://img.shields.io/pypi/v/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-web.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-web)](https://pepy.tech/project/types-aiobotocore-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpacesWeb 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[aiobotocore.WorkSpacesWeb 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [types-aiobotocore-workspaces-web docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-web-2.9.0/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt` & `types-aiobotocore-workspaces-web-2.9.1/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

