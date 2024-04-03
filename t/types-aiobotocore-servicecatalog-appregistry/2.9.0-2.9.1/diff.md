# Comparing `tmp/types-aiobotocore-servicecatalog-appregistry-2.9.0.tar.gz` & `tmp/types-aiobotocore-servicecatalog-appregistry-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicecatalog-appregistry-2.9.0.tar", last modified: Wed Dec 13 20:00:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicecatalog-appregistry-2.9.1.tar", last modified: Thu Jan 18 01:21:48 2024, max compression
```

## Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0.tar` & `types-aiobotocore-servicecatalog-appregistry-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.857143 types-aiobotocore-servicecatalog-appregistry-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2023-12-13 20:00:29.857143 types-aiobotocore-servicecatalog-appregistry-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:29.857143 types-aiobotocore-servicecatalog-appregistry-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.857143 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23176 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23172 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10245 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19574 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19573 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.857143 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2023-12-13 20:00:29.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-13 20:00:29.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:29.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:29.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:29.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-13 20:00:29.000000 types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.337037 types-aiobotocore-servicecatalog-appregistry-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-01-18 01:21:48.337037 types-aiobotocore-servicecatalog-appregistry-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:48.337037 types-aiobotocore-servicecatalog-appregistry-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.337037 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23178 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23175 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19573 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19573 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.337037 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/LICENSE` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/PKG-INFO` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog-appregistry
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppRegistry 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppRegistry 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/
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
 
 <a id="types-aiobotocore-servicecatalog-appregistry"></a>
 
 # types-aiobotocore-servicecatalog-appregistry
 
 [![PyPI - types-aiobotocore-servicecatalog-appregistry](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog-appregistry)](https://pepy.tech/project/types-aiobotocore-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRegistry 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[aiobotocore.AppRegistry 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/README.md` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog-appregistry)](https://pepy.tech/project/types-aiobotocore-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRegistry 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[aiobotocore.AppRegistry 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/setup.py` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,51 +7,50 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicecatalog-appregistry",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_servicecatalog_appregistry"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppRegistry 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AppRegistry 2.9.1 service generated with"
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
         "aiobotocore servicecatalog-appregistry type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_servicecatalog_appregistry": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/__init__.py` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListAssociatedResourcesPaginator,
     ListAttributeGroupsForApplicationPaginator,
     ListAttributeGroupsPaginator,
 )
 
 Client = AppRegistryClient
 
-
 __all__ = (
     "AppRegistryClient",
     "Client",
     "ListApplicationsPaginator",
     "ListAssociatedAttributeGroupsPaginator",
     "ListAssociatedResourcesPaginator",
     "ListAttributeGroupsForApplicationPaginator",
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/__init__.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/__main__.py` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppRegistry 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AppRegistry 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry\nOther"
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

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/client.py` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppRegistryClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -113,15 +112,15 @@
 
     async def associate_resource(
         self,
         *,
         application: str,
         resourceType: ResourceTypeType,
         resource: str,
-        options: Sequence[AssociationOptionType] = ...
+        options: Sequence[AssociationOptionType] = ...,
     ) -> AssociateResourceResponseTypeDef:
         """
         Associates a resource with an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.associate_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/client/#associate_resource)
         """
@@ -157,15 +156,15 @@
     async def create_attribute_group(
         self,
         *,
         name: str,
         attributes: str,
         clientToken: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAttributeGroupResponseTypeDef:
         """
         Creates a new attribute group as a container for user-defined attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.create_attribute_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/client/#create_attribute_group)
         """
@@ -239,15 +238,15 @@
         self,
         *,
         application: str,
         resourceType: ResourceTypeType,
         resource: str,
         nextToken: str = ...,
         resourceTagStatus: Sequence[ResourceItemStatusType] = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetAssociatedResourceResponseTypeDef:
         """
         Gets the resource associated with the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.get_associated_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/client/#get_associated_resource)
         """
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/client.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     async def associate_resource(
         self,
         *,
         application: str,
         resourceType: ResourceTypeType,
         resource: str,
-        options: Sequence[AssociationOptionType] = ...
+        options: Sequence[AssociationOptionType] = ...,
     ) -> AssociateResourceResponseTypeDef:
         """
         Associates a resource with an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.associate_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/client/#associate_resource)
         """
@@ -153,15 +153,15 @@
     async def create_attribute_group(
         self,
         *,
         name: str,
         attributes: str,
         clientToken: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAttributeGroupResponseTypeDef:
         """
         Creates a new attribute group as a container for user-defined attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.create_attribute_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/client/#create_attribute_group)
         """
@@ -235,15 +235,15 @@
         self,
         *,
         application: str,
         resourceType: ResourceTypeType,
         resource: str,
         nextToken: str = ...,
         resourceTagStatus: Sequence[ResourceItemStatusType] = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetAssociatedResourceResponseTypeDef:
         """
         Gets the resource associated with the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.get_associated_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/client/#get_associated_resource)
         """
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/literals.py` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/literals.py`

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
     "ApplicationTagStatusType",
     "AssociationOptionType",
     "ListApplicationsPaginatorName",
     "ListAssociatedAttributeGroupsPaginatorName",
     "ListAssociatedResourcesPaginatorName",
     "ListAttributeGroupsForApplicationPaginatorName",
@@ -35,15 +34,14 @@
     "AppRegistryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationTagStatusType = Literal["FAILURE", "IN_PROGRESS", "SUCCESS"]
 AssociationOptionType = Literal["APPLY_APPLICATION_TAG", "SKIP_APPLICATION_TAG"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListAssociatedAttributeGroupsPaginatorName = Literal["list_associated_attribute_groups"]
 ListAssociatedResourcesPaginatorName = Literal["list_associated_resources"]
 ListAttributeGroupsForApplicationPaginatorName = Literal["list_attribute_groups_for_application"]
 ListAttributeGroupsPaginatorName = Literal["list_attribute_groups"]
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/literals.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/paginator.py` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListApplicationsPaginator",
     "ListAssociatedAttributeGroupsPaginator",
     "ListAssociatedResourcesPaginator",
     "ListAttributeGroupsPaginator",
     "ListAttributeGroupsForApplicationPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/paginator.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/type_defs.py` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/type_defs.py`

 * *Files 1% similar despite different names*

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
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ResourcesListItemTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog-appregistry
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppRegistry 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppRegistry 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/
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
 
 <a id="types-aiobotocore-servicecatalog-appregistry"></a>
 
 # types-aiobotocore-servicecatalog-appregistry
 
 [![PyPI - types-aiobotocore-servicecatalog-appregistry](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog-appregistry)](https://pepy.tech/project/types-aiobotocore-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRegistry 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[aiobotocore.AppRegistry 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.9.0/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt` & `types-aiobotocore-servicecatalog-appregistry-2.9.1/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

