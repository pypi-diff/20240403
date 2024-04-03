# Comparing `tmp/types-aiobotocore-network-firewall-2.9.0.tar.gz` & `tmp/types-aiobotocore-network-firewall-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-network-firewall-2.9.0.tar", last modified: Wed Dec 13 20:00:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-network-firewall-2.9.1.tar", last modified: Thu Jan 18 01:21:22 2024, max compression
```

## Comparing `types-aiobotocore-network-firewall-2.9.0.tar` & `types-aiobotocore-network-firewall-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:01.345390 types-aiobotocore-network-firewall-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14127 2023-12-13 20:00:01.345390 types-aiobotocore-network-firewall-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12529 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:01.345390 types-aiobotocore-network-firewall-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:01.345390 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34252 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34248 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2023-12-13 19:50:52.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2023-12-13 19:50:52.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    41836 2023-12-13 19:50:52.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41835 2023-12-13 19:50:52.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:51.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:01.345390 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14127 2023-12-13 20:00:01.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 20:00:01.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:01.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:01.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:01.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 20:00:01.000000 types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.525152 types-aiobotocore-network-firewall-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-01-18 01:21:22.525152 types-aiobotocore-network-firewall-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:22.525152 types-aiobotocore-network-firewall-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.521152 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34269 2024-01-18 01:12:34.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34266 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-01-18 01:12:34.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-01-18 01:12:34.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-01-18 01:12:34.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-01-18 01:12:34.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    41835 2024-01-18 01:12:35.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41835 2024-01-18 01:12:35.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:31.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.525152 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-01-18 01:21:22.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:21:22.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:22.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:22.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:22.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:21:22.000000 types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/LICENSE` & `types-aiobotocore-network-firewall-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-network-firewall-2.9.0/PKG-INFO` & `types-aiobotocore-network-firewall-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-network-firewall
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.NetworkFirewall 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.NetworkFirewall 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/
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
 
 <a id="types-aiobotocore-network-firewall"></a>
 
 # types-aiobotocore-network-firewall
 
 [![PyPI - types-aiobotocore-network-firewall](https://img.shields.io/pypi/v/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-network-firewall)](https://pepy.tech/project/types-aiobotocore-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkFirewall 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[aiobotocore.NetworkFirewall 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [types-aiobotocore-network-firewall docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/README.md` & `types-aiobotocore-network-firewall-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-network-firewall)](https://pepy.tech/project/types-aiobotocore-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkFirewall 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[aiobotocore.NetworkFirewall 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [types-aiobotocore-network-firewall docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/setup.py` & `types-aiobotocore-network-firewall-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-network-firewall",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.NetworkFirewall 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.NetworkFirewall 2.9.1 service generated with"
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
     keywords="aiobotocore network-firewall type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_network_firewall": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/__init__.py` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/__init__.py`

 * *Files identical despite different names*

```diff
@@ -36,15 +36,14 @@
     ListRuleGroupsPaginator,
     ListTagsForResourcePaginator,
     ListTLSInspectionConfigurationsPaginator,
 )
 
 Client = NetworkFirewallClient
 
-
 __all__ = (
     "Client",
     "ListFirewallPoliciesPaginator",
     "ListFirewallsPaginator",
     "ListRuleGroupsPaginator",
     "ListTLSInspectionConfigurationsPaginator",
     "ListTagsForResourcePaginator",
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/__init__.pyi` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/client.py` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("NetworkFirewallClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -124,30 +123,30 @@
 
     async def associate_firewall_policy(
         self,
         *,
         FirewallPolicyArn: str,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> AssociateFirewallPolicyResponseTypeDef:
         """
         Associates a  FirewallPolicy to a  Firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#associate_firewall_policy)
         """
 
     async def associate_subnets(
         self,
         *,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> AssociateSubnetsResponseTypeDef:
         """
         Associates the specified subnets in the Amazon VPC to the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_subnets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#associate_subnets)
         """
@@ -176,15 +175,15 @@
         VpcId: str,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
         DeleteProtection: bool = ...,
         SubnetChangeProtection: bool = ...,
         FirewallPolicyChangeProtection: bool = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> CreateFirewallResponseTypeDef:
         """
         Creates an Network Firewall  Firewall and accompanying  FirewallStatus for a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall)
@@ -194,15 +193,15 @@
         self,
         *,
         FirewallPolicyName: str,
         FirewallPolicy: FirewallPolicyTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall_policy)
         """
@@ -216,15 +215,15 @@
         RuleGroup: RuleGroupTypeDef = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...,
-        AnalyzeRuleGroup: bool = ...
+        AnalyzeRuleGroup: bool = ...,
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates the specified stateless or stateful rule group, which includes the
         rules for network traffic inspection, a capacity setting, and
         tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
@@ -234,15 +233,15 @@
     async def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
         TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_tls_inspection_configuration)
         """
@@ -337,15 +336,15 @@
 
     async def describe_rule_group(
         self,
         *,
         RuleGroupName: str = ...,
         RuleGroupArn: str = ...,
         Type: RuleGroupTypeType = ...,
-        AnalyzeRuleGroup: bool = ...
+        AnalyzeRuleGroup: bool = ...,
     ) -> DescribeRuleGroupResponseTypeDef:
         """
         Returns the data objects for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_rule_group)
         """
@@ -374,15 +373,15 @@
 
     async def disassociate_subnets(
         self,
         *,
         SubnetIds: Sequence[str],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> DisassociateSubnetsResponseTypeDef:
         """
         Removes the specified subnet associations from the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.disassociate_subnets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#disassociate_subnets)
         """
@@ -424,15 +423,15 @@
     async def list_rule_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
-        Type: RuleGroupTypeType = ...
+        Type: RuleGroupTypeType = ...,
     ) -> ListRuleGroupsResponseTypeDef:
         """
         Retrieves the metadata for the rule groups that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_rule_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_rule_groups)
         """
@@ -484,15 +483,15 @@
 
     async def update_firewall_delete_protection(
         self,
         *,
         DeleteProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> UpdateFirewallDeleteProtectionResponseTypeDef:
         """
         Modifies the flag, `DeleteProtection`, which indicates whether it is possible
         to delete the
         firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_delete_protection)
@@ -501,30 +500,30 @@
 
     async def update_firewall_description(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateFirewallDescriptionResponseTypeDef:
         """
         Modifies the description for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_description)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_description)
         """
 
     async def update_firewall_encryption_configuration(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> UpdateFirewallEncryptionConfigurationResponseTypeDef:
         """
         A complex type that contains settings for encryption of your firewall resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_encryption_configuration)
         """
@@ -534,30 +533,30 @@
         *,
         UpdateToken: str,
         FirewallPolicy: FirewallPolicyTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
         Updates the properties of the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_policy)
         """
 
     async def update_firewall_policy_change_protection(
         self,
         *,
         FirewallPolicyChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> UpdateFirewallPolicyChangeProtectionResponseTypeDef:
         """
         Modifies the flag, `ChangeProtection`, which indicates whether it is possible
         to change the
         firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy_change_protection)
@@ -565,15 +564,15 @@
         """
 
     async def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: LoggingConfigurationTypeDef = ...
+        LoggingConfiguration: LoggingConfigurationTypeDef = ...,
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_logging_configuration)
         """
@@ -587,30 +586,30 @@
         RuleGroup: RuleGroupTypeDef = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...,
-        AnalyzeRuleGroup: bool = ...
+        AnalyzeRuleGroup: bool = ...,
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the rule settings for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_rule_group)
         """
 
     async def update_subnet_change_protection(
         self,
         *,
         SubnetChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> UpdateSubnetChangeProtectionResponseTypeDef:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/network-firewall-2020-11-12/UpdateSubnetChangeProtection).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_subnet_change_protection)
@@ -620,15 +619,15 @@
         self,
         *,
         TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
         Updates the TLS inspection configuration settings for the specified TLS
         inspection
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_tls_inspection_configuration)
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/client.pyi` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -120,30 +120,30 @@
 
     async def associate_firewall_policy(
         self,
         *,
         FirewallPolicyArn: str,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> AssociateFirewallPolicyResponseTypeDef:
         """
         Associates a  FirewallPolicy to a  Firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#associate_firewall_policy)
         """
 
     async def associate_subnets(
         self,
         *,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> AssociateSubnetsResponseTypeDef:
         """
         Associates the specified subnets in the Amazon VPC to the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_subnets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#associate_subnets)
         """
@@ -172,15 +172,15 @@
         VpcId: str,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
         DeleteProtection: bool = ...,
         SubnetChangeProtection: bool = ...,
         FirewallPolicyChangeProtection: bool = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> CreateFirewallResponseTypeDef:
         """
         Creates an Network Firewall  Firewall and accompanying  FirewallStatus for a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall)
@@ -190,15 +190,15 @@
         self,
         *,
         FirewallPolicyName: str,
         FirewallPolicy: FirewallPolicyTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall_policy)
         """
@@ -212,15 +212,15 @@
         RuleGroup: RuleGroupTypeDef = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...,
-        AnalyzeRuleGroup: bool = ...
+        AnalyzeRuleGroup: bool = ...,
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates the specified stateless or stateful rule group, which includes the
         rules for network traffic inspection, a capacity setting, and
         tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
@@ -230,15 +230,15 @@
     async def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
         TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_tls_inspection_configuration)
         """
@@ -333,15 +333,15 @@
 
     async def describe_rule_group(
         self,
         *,
         RuleGroupName: str = ...,
         RuleGroupArn: str = ...,
         Type: RuleGroupTypeType = ...,
-        AnalyzeRuleGroup: bool = ...
+        AnalyzeRuleGroup: bool = ...,
     ) -> DescribeRuleGroupResponseTypeDef:
         """
         Returns the data objects for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_rule_group)
         """
@@ -370,15 +370,15 @@
 
     async def disassociate_subnets(
         self,
         *,
         SubnetIds: Sequence[str],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> DisassociateSubnetsResponseTypeDef:
         """
         Removes the specified subnet associations from the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.disassociate_subnets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#disassociate_subnets)
         """
@@ -420,15 +420,15 @@
     async def list_rule_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
-        Type: RuleGroupTypeType = ...
+        Type: RuleGroupTypeType = ...,
     ) -> ListRuleGroupsResponseTypeDef:
         """
         Retrieves the metadata for the rule groups that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_rule_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_rule_groups)
         """
@@ -480,15 +480,15 @@
 
     async def update_firewall_delete_protection(
         self,
         *,
         DeleteProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> UpdateFirewallDeleteProtectionResponseTypeDef:
         """
         Modifies the flag, `DeleteProtection`, which indicates whether it is possible
         to delete the
         firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_delete_protection)
@@ -497,30 +497,30 @@
 
     async def update_firewall_description(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateFirewallDescriptionResponseTypeDef:
         """
         Modifies the description for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_description)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_description)
         """
 
     async def update_firewall_encryption_configuration(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> UpdateFirewallEncryptionConfigurationResponseTypeDef:
         """
         A complex type that contains settings for encryption of your firewall resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_encryption_configuration)
         """
@@ -530,30 +530,30 @@
         *,
         UpdateToken: str,
         FirewallPolicy: FirewallPolicyTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
         Updates the properties of the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_policy)
         """
 
     async def update_firewall_policy_change_protection(
         self,
         *,
         FirewallPolicyChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> UpdateFirewallPolicyChangeProtectionResponseTypeDef:
         """
         Modifies the flag, `ChangeProtection`, which indicates whether it is possible
         to change the
         firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy_change_protection)
@@ -561,15 +561,15 @@
         """
 
     async def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: LoggingConfigurationTypeDef = ...
+        LoggingConfiguration: LoggingConfigurationTypeDef = ...,
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_logging_configuration)
         """
@@ -583,30 +583,30 @@
         RuleGroup: RuleGroupTypeDef = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...,
-        AnalyzeRuleGroup: bool = ...
+        AnalyzeRuleGroup: bool = ...,
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the rule settings for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_rule_group)
         """
 
     async def update_subnet_change_protection(
         self,
         *,
         SubnetChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
-        FirewallName: str = ...
+        FirewallName: str = ...,
     ) -> UpdateSubnetChangeProtectionResponseTypeDef:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/network-firewall-2020-11-12/UpdateSubnetChangeProtection).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_subnet_change_protection)
@@ -616,15 +616,15 @@
         self,
         *,
         TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
-        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
         Updates the TLS inspection configuration settings for the specified TLS
         inspection
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_tls_inspection_configuration)
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/literals.py` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/literals.py`

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
     "AttachmentStatusType",
     "ConfigurationSyncStateType",
     "EncryptionTypeType",
     "FirewallStatusValueType",
     "GeneratedRulesTypeType",
     "IPAddressTypeType",
@@ -52,15 +51,14 @@
     "NetworkFirewallServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AttachmentStatusType = Literal["CREATING", "DELETING", "ERROR", "FAILED", "READY", "SCALING"]
 ConfigurationSyncStateType = Literal["CAPACITY_CONSTRAINED", "IN_SYNC", "PENDING"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_KMS"]
 FirewallStatusValueType = Literal["DELETING", "PROVISIONING", "READY"]
 GeneratedRulesTypeType = Literal["ALLOWLIST", "DENYLIST"]
 IPAddressTypeType = Literal["DUALSTACK", "IPV4", "IPV6"]
 IdentifiedTypeType = Literal[
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/literals.pyi` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/paginator.py` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     "ListFirewallPoliciesPaginator",
     "ListFirewallsPaginator",
     "ListRuleGroupsPaginator",
     "ListTLSInspectionConfigurationsPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -101,15 +100,15 @@
 
     def paginate(
         self,
         *,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
         Type: RuleGroupTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listrulegroupspaginator)
         """
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/paginator.pyi` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     def paginate(
         self,
         *,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
         Type: RuleGroupTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listrulegroupspaginator)
         """
 
 class ListTLSInspectionConfigurationsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/type_defs.py` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "AnalysisResultTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SubnetMappingTypeDef",
     "AttachmentTypeDef",
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall/type_defs.pyi` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/PKG-INFO` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-network-firewall
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.NetworkFirewall 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.NetworkFirewall 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/
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
 
 <a id="types-aiobotocore-network-firewall"></a>
 
 # types-aiobotocore-network-firewall
 
 [![PyPI - types-aiobotocore-network-firewall](https://img.shields.io/pypi/v/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-network-firewall)](https://pepy.tech/project/types-aiobotocore-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkFirewall 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[aiobotocore.NetworkFirewall 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [types-aiobotocore-network-firewall docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-network-firewall-2.9.0/types_aiobotocore_network_firewall.egg-info/SOURCES.txt` & `types-aiobotocore-network-firewall-2.9.1/types_aiobotocore_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

