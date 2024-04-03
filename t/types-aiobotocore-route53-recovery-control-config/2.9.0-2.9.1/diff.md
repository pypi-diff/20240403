# Comparing `tmp/types-aiobotocore-route53-recovery-control-config-2.9.0.tar.gz` & `tmp/types-aiobotocore-route53-recovery-control-config-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-control-config-2.9.0.tar", last modified: Wed Dec 13 20:00:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-control-config-2.9.1.tar", last modified: Thu Jan 18 01:21:40 2024, max compression
```

## Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0.tar` & `types-aiobotocore-route53-recovery-control-config-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:20.745221 types-aiobotocore-route53-recovery-control-config-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16591 2023-12-13 20:00:20.745221 types-aiobotocore-route53-recovery-control-config-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14935 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:20.745221 types-aiobotocore-route53-recovery-control-config-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:20.741221 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26343 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    26339 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9934 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9932 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18429 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18428 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7507 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7501 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:20.745221 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16591 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.037074 types-aiobotocore-route53-recovery-control-config-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:27.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16611 2024-01-18 01:21:40.037074 types-aiobotocore-route53-recovery-control-config-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-01-18 01:16:27.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:40.037074 types-aiobotocore-route53-recovery-control-config-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-01-18 01:16:27.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.037074 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-01-18 01:16:27.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-01-18 01:16:27.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-18 01:16:27.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26346 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26343 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:27.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18428 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18428 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:27.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.037074 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16611 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/LICENSE` & `types-aiobotocore-route53-recovery-control-config-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/PKG-INFO` & `types-aiobotocore-route53-recovery-control-config-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-control-config
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/
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
 
 <a id="types-aiobotocore-route53-recovery-control-config"></a>
 
 # types-aiobotocore-route53-recovery-control-config
 
 [![PyPI - types-aiobotocore-route53-recovery-control-config](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-control-config)](https://pepy.tech/project/types-aiobotocore-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryControlConfig 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[aiobotocore.Route53RecoveryControlConfig 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/README.md` & `types-aiobotocore-route53-recovery-control-config-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-control-config)](https://pepy.tech/project/types-aiobotocore-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryControlConfig 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[aiobotocore.Route53RecoveryControlConfig 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/setup.py` & `types-aiobotocore-route53-recovery-control-config-2.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,51 +7,50 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-control-config",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_route53_recovery_control_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53RecoveryControlConfig 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Route53RecoveryControlConfig 2.9.1 service generated with"
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
         "aiobotocore route53-recovery-control-config type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53_recovery_control_config": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/__init__.py` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     ControlPanelDeletedWaiter,
     RoutingControlCreatedWaiter,
     RoutingControlDeletedWaiter,
 )
 
 Client = Route53RecoveryControlConfigClient
 
-
 __all__ = (
     "Client",
     "ClusterCreatedWaiter",
     "ClusterDeletedWaiter",
     "ControlPanelCreatedWaiter",
     "ControlPanelDeletedWaiter",
     "ListAssociatedRoute53HealthChecksPaginator",
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/__init__.pyi` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/__main__.py` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53RecoveryControlConfig 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Route53RecoveryControlConfig 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/client.py` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,37 +62,33 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Route53RecoveryControlConfigClient",)
 
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
 class Route53RecoveryControlConfigClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/)
     """
 
     meta: ClientMeta
@@ -134,45 +130,45 @@
 
     async def create_control_panel(
         self,
         *,
         ClusterArn: str,
         ControlPanelName: str,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateControlPanelResponseTypeDef:
         """
         Creates a new control panel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_control_panel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#create_control_panel)
         """
 
     async def create_routing_control(
         self,
         *,
         ClusterArn: str,
         RoutingControlName: str,
         ClientToken: str = ...,
-        ControlPanelArn: str = ...
+        ControlPanelArn: str = ...,
     ) -> CreateRoutingControlResponseTypeDef:
         """
         Creates a new routing control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_routing_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#create_routing_control)
         """
 
     async def create_safety_rule(
         self,
         *,
         AssertionRule: NewAssertionRuleTypeDef = ...,
         ClientToken: str = ...,
         GatingRule: NewGatingRuleTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateSafetyRuleResponseTypeDef:
         """
         Creates a safety rule in a control panel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_safety_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#create_safety_rule)
         """
@@ -369,15 +365,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#update_routing_control)
         """
 
     async def update_safety_rule(
         self,
         *,
         AssertionRuleUpdate: AssertionRuleUpdateTypeDef = ...,
-        GatingRuleUpdate: GatingRuleUpdateTypeDef = ...
+        GatingRuleUpdate: GatingRuleUpdateTypeDef = ...,
     ) -> UpdateSafetyRuleResponseTypeDef:
         """
         Update a safety rule (an assertion rule or gating rule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.update_safety_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#update_safety_rule)
         """
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/client.pyi` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,31 +64,34 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("Route53RecoveryControlConfigClient",)
 
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
 class Route53RecoveryControlConfigClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/)
     """
 
     meta: ClientMeta
@@ -130,45 +133,45 @@
 
     async def create_control_panel(
         self,
         *,
         ClusterArn: str,
         ControlPanelName: str,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateControlPanelResponseTypeDef:
         """
         Creates a new control panel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_control_panel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#create_control_panel)
         """
 
     async def create_routing_control(
         self,
         *,
         ClusterArn: str,
         RoutingControlName: str,
         ClientToken: str = ...,
-        ControlPanelArn: str = ...
+        ControlPanelArn: str = ...,
     ) -> CreateRoutingControlResponseTypeDef:
         """
         Creates a new routing control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_routing_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#create_routing_control)
         """
 
     async def create_safety_rule(
         self,
         *,
         AssertionRule: NewAssertionRuleTypeDef = ...,
         ClientToken: str = ...,
         GatingRule: NewGatingRuleTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateSafetyRuleResponseTypeDef:
         """
         Creates a safety rule in a control panel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.create_safety_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#create_safety_rule)
         """
@@ -365,15 +368,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#update_routing_control)
         """
 
     async def update_safety_rule(
         self,
         *,
         AssertionRuleUpdate: AssertionRuleUpdateTypeDef = ...,
-        GatingRuleUpdate: GatingRuleUpdateTypeDef = ...
+        GatingRuleUpdate: GatingRuleUpdateTypeDef = ...,
     ) -> UpdateSafetyRuleResponseTypeDef:
         """
         Update a safety rule (an assertion rule or gating rule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Client.update_safety_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/client/#update_safety_rule)
         """
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/literals.py` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/literals.py`

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
     "ClusterCreatedWaiterName",
     "ClusterDeletedWaiterName",
     "ControlPanelCreatedWaiterName",
     "ControlPanelDeletedWaiterName",
     "ListAssociatedRoute53HealthChecksPaginatorName",
     "ListClustersPaginatorName",
@@ -37,15 +36,14 @@
     "Route53RecoveryControlConfigServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
 )
 
-
 ClusterCreatedWaiterName = Literal["cluster_created"]
 ClusterDeletedWaiterName = Literal["cluster_deleted"]
 ControlPanelCreatedWaiterName = Literal["control_panel_created"]
 ControlPanelDeletedWaiterName = Literal["control_panel_deleted"]
 ListAssociatedRoute53HealthChecksPaginatorName = Literal["list_associated_route53_health_checks"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListControlPanelsPaginatorName = Literal["list_control_panels"]
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/literals.pyi` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/paginator.py` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListAssociatedRoute53HealthChecksPaginator",
     "ListClustersPaginator",
     "ListControlPanelsPaginator",
     "ListRoutingControlsPaginator",
     "ListSafetyRulesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/paginator.pyi` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/type_defs.py` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/type_defs.py`

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
     "RuleConfigTypeDef",
     "AssertionRuleUpdateTypeDef",
     "ClusterEndpointTypeDef",
     "ControlPanelTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/type_defs.pyi` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/waiter.py` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config/waiter.pyi` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-control-config
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/
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
 
 <a id="types-aiobotocore-route53-recovery-control-config"></a>
 
 # types-aiobotocore-route53-recovery-control-config
 
 [![PyPI - types-aiobotocore-route53-recovery-control-config](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-control-config)](https://pepy.tech/project/types-aiobotocore-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryControlConfig 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[aiobotocore.Route53RecoveryControlConfig 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.9.0/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-control-config-2.9.1/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

