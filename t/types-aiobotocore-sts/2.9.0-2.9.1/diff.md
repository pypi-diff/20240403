# Comparing `tmp/types-aiobotocore-sts-2.9.0.tar.gz` & `tmp/types-aiobotocore-sts-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sts-2.9.0.tar", last modified: Wed Dec 13 20:00:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-sts-2.9.1.tar", last modified: Thu Jan 18 01:21:56 2024, max compression
```

## Comparing `types-aiobotocore-sts-2.9.0.tar` & `types-aiobotocore-sts-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.545069 types-aiobotocore-sts-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2023-12-13 20:00:38.545069 types-aiobotocore-sts-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:38.545069 types-aiobotocore-sts-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.545069 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10238 2023-12-13 19:57:11.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2023-12-13 19:57:11.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2023-12-13 19:57:11.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2023-12-13 19:57:11.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2023-12-13 19:57:11.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:10.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.545069 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2023-12-13 20:00:38.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-13 20:00:38.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:38.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:38.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:38.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:38.000000 types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.169001 types-aiobotocore-sts-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-01-18 01:21:56.169001 types-aiobotocore-sts-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:56.169001 types-aiobotocore-sts-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.169001 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-01-18 01:18:39.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-01-18 01:18:39.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:38.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.169001 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-01-18 01:21:56.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-18 01:21:56.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:56.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:56.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:56.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:56.000000 types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sts-2.9.0/LICENSE` & `types-aiobotocore-sts-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sts-2.9.0/PKG-INFO` & `types-aiobotocore-sts-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sts
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.STS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.STS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/
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
 
 <a id="types-aiobotocore-sts"></a>
 
 # types-aiobotocore-sts
 
 [![PyPI - types-aiobotocore-sts](https://img.shields.io/pypi/v/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sts)](https://pepy.tech/project/types-aiobotocore-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.STS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[aiobotocore.STS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sts-2.9.0/README.md` & `types-aiobotocore-sts-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sts)](https://pepy.tech/project/types-aiobotocore-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.STS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[aiobotocore.STS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sts-2.9.0/setup.py` & `types-aiobotocore-sts-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sts",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.STS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.STS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore sts type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sts": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/__main__.py` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.STS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.STS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS\nOther"
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

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/client.py` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         DurationSeconds: int = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TransitiveTagKeys: Sequence[str] = ...,
         ExternalId: str = ...,
         SerialNumber: str = ...,
         TokenCode: str = ...,
         SourceIdentity: str = ...,
-        ProvidedContexts: Sequence[ProvidedContextTypeDef] = ...
+        ProvidedContexts: Sequence[ProvidedContextTypeDef] = ...,
     ) -> AssumeRoleResponseTypeDef:
         """
         Returns a set of temporary security credentials that you can use to access
         Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role)
@@ -103,15 +103,15 @@
         self,
         *,
         RoleArn: str,
         PrincipalArn: str,
         SAMLAssertion: str,
         PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,
         Policy: str = ...,
-        DurationSeconds: int = ...
+        DurationSeconds: int = ...,
     ) -> AssumeRoleWithSAMLResponseTypeDef:
         """
         Returns a set of temporary security credentials for users who have been
         authenticated via a SAML authentication
         response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role_with_saml)
@@ -123,15 +123,15 @@
         *,
         RoleArn: str,
         RoleSessionName: str,
         WebIdentityToken: str,
         ProviderId: str = ...,
         PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,
         Policy: str = ...,
-        DurationSeconds: int = ...
+        DurationSeconds: int = ...,
     ) -> AssumeRoleWithWebIdentityResponseTypeDef:
         """
         Returns a set of temporary security credentials for users who have been
         authenticated in a mobile or web application with a web identity
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role_with_web_identity)
@@ -201,15 +201,15 @@
     async def get_federation_token(
         self,
         *,
         Name: str,
         Policy: str = ...,
         PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,
         DurationSeconds: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> GetFederationTokenResponseTypeDef:
         """
         Returns a set of temporary security credentials (consisting of an access key
         ID, a secret access key, and a security token) for a
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.get_federation_token)
```

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/client.pyi` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         DurationSeconds: int = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TransitiveTagKeys: Sequence[str] = ...,
         ExternalId: str = ...,
         SerialNumber: str = ...,
         TokenCode: str = ...,
         SourceIdentity: str = ...,
-        ProvidedContexts: Sequence[ProvidedContextTypeDef] = ...
+        ProvidedContexts: Sequence[ProvidedContextTypeDef] = ...,
     ) -> AssumeRoleResponseTypeDef:
         """
         Returns a set of temporary security credentials that you can use to access
         Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role)
@@ -100,15 +100,15 @@
         self,
         *,
         RoleArn: str,
         PrincipalArn: str,
         SAMLAssertion: str,
         PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,
         Policy: str = ...,
-        DurationSeconds: int = ...
+        DurationSeconds: int = ...,
     ) -> AssumeRoleWithSAMLResponseTypeDef:
         """
         Returns a set of temporary security credentials for users who have been
         authenticated via a SAML authentication
         response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role_with_saml)
@@ -120,15 +120,15 @@
         *,
         RoleArn: str,
         RoleSessionName: str,
         WebIdentityToken: str,
         ProviderId: str = ...,
         PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,
         Policy: str = ...,
-        DurationSeconds: int = ...
+        DurationSeconds: int = ...,
     ) -> AssumeRoleWithWebIdentityResponseTypeDef:
         """
         Returns a set of temporary security credentials for users who have been
         authenticated in a mobile or web application with a web identity
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role_with_web_identity)
@@ -198,15 +198,15 @@
     async def get_federation_token(
         self,
         *,
         Name: str,
         Policy: str = ...,
         PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,
         DurationSeconds: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> GetFederationTokenResponseTypeDef:
         """
         Returns a set of temporary security credentials (consisting of an access key
         ID, a secret access key, and a security token) for a
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.get_federation_token)
```

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/literals.py` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("STSServiceName", "ServiceName", "ResourceServiceName", "RegionName")
 
-
 STSServiceName = Literal["sts"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/literals.pyi` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/type_defs.py` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "PolicyDescriptorTypeTypeDef",
     "ProvidedContextTypeDef",
     "TagTypeDef",
     "AssumedRoleUserTypeDef",
     "CredentialsTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts/type_defs.pyi` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/PKG-INFO` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sts
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.STS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.STS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/
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
 
 <a id="types-aiobotocore-sts"></a>
 
 # types-aiobotocore-sts
 
 [![PyPI - types-aiobotocore-sts](https://img.shields.io/pypi/v/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sts)](https://pepy.tech/project/types-aiobotocore-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.STS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[aiobotocore.STS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sts-2.9.0/types_aiobotocore_sts.egg-info/SOURCES.txt` & `types-aiobotocore-sts-2.9.1/types_aiobotocore_sts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

