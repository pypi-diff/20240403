# Comparing `tmp/types-aiobotocore-bedrock-agent-2.9.0.tar.gz` & `tmp/types-aiobotocore-bedrock-agent-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-bedrock-agent-2.9.0.tar", last modified: Wed Dec 13 19:58:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-bedrock-agent-2.9.1.tar", last modified: Thu Jan 18 01:20:09 2024, max compression
```

## Comparing `types-aiobotocore-bedrock-agent-2.9.0.tar` & `types-aiobotocore-bedrock-agent-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:41.718036 types-aiobotocore-bedrock-agent-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14442 2023-12-13 19:58:41.718036 types-aiobotocore-bedrock-agent-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:41.718036 types-aiobotocore-bedrock-agent-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:41.718036 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40603 2023-12-13 19:41:43.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    40599 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2023-12-13 19:41:43.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2023-12-13 19:41:43.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10477 2023-12-13 19:41:43.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2023-12-13 19:41:43.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    40468 2023-12-13 19:41:43.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    40467 2023-12-13 19:41:43.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:41.718036 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14442 2023-12-13 19:58:41.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 19:58:41.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:41.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:41.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:41.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:58:41.000000 types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:09.189492 types-aiobotocore-bedrock-agent-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14462 2024-01-18 01:20:09.189492 types-aiobotocore-bedrock-agent-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:09.189492 types-aiobotocore-bedrock-agent-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:09.185492 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40617 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40614 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-01-18 01:03:41.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-01-18 01:03:41.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-01-18 01:03:41.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    40467 2024-01-18 01:03:42.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40467 2024-01-18 01:03:42.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:09.189492 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14462 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/LICENSE` & `types-aiobotocore-bedrock-agent-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/PKG-INFO` & `types-aiobotocore-bedrock-agent-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-bedrock-agent
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AgentsforBedrock 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AgentsforBedrock 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/
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
 
 <a id="types-aiobotocore-bedrock-agent"></a>
 
 # types-aiobotocore-bedrock-agent
 
 [![PyPI - types-aiobotocore-bedrock-agent](https://img.shields.io/pypi/v/types-aiobotocore-bedrock-agent.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock-agent)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bedrock-agent.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bedrock-agent)](https://pepy.tech/project/types-aiobotocore-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AgentsforBedrock 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[aiobotocore.AgentsforBedrock 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
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
 [types-aiobotocore-bedrock-agent docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/README.md` & `types-aiobotocore-bedrock-agent-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bedrock-agent.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bedrock-agent)](https://pepy.tech/project/types-aiobotocore-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AgentsforBedrock 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[aiobotocore.AgentsforBedrock 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
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
 [types-aiobotocore-bedrock-agent docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/setup.py` & `types-aiobotocore-bedrock-agent-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-bedrock-agent",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_bedrock_agent"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AgentsforBedrock 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AgentsforBedrock 2.9.1 service generated with"
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
     keywords="aiobotocore bedrock-agent type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_bedrock_agent": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/__init__.py` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListDataSourcesPaginator,
     ListIngestionJobsPaginator,
     ListKnowledgeBasesPaginator,
 )
 
 Client = AgentsforBedrockClient
 
-
 __all__ = (
     "AgentsforBedrockClient",
     "Client",
     "ListAgentActionGroupsPaginator",
     "ListAgentAliasesPaginator",
     "ListAgentKnowledgeBasesPaginator",
     "ListAgentVersionsPaginator",
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/__init__.pyi` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/__main__.py` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AgentsforBedrock 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AgentsforBedrock 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock\nOther"
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

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/client.py` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AgentsforBedrockClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -130,15 +129,15 @@
     async def associate_agent_knowledge_base(
         self,
         *,
         agentId: str,
         agentVersion: str,
         knowledgeBaseId: str,
         description: str,
-        knowledgeBaseState: KnowledgeBaseStateType = ...
+        knowledgeBaseState: KnowledgeBaseStateType = ...,
     ) -> AssociateAgentKnowledgeBaseResponseTypeDef:
         """
         Associate a Knowledge Base to an existing Amazon Bedrock Agent See also: [AWS
         API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/AssociateAgentKnowledgeBase).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.associate_agent_knowledge_base)
@@ -169,15 +168,15 @@
         clientToken: str = ...,
         instruction: str = ...,
         foundationModel: str = ...,
         description: str = ...,
         idleSessionTTLInSeconds: int = ...,
         customerEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
-        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...
+        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
     ) -> CreateAgentResponseTypeDef:
         """
         Creates an Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgent).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_agent)
@@ -190,15 +189,15 @@
         agentVersion: str,
         actionGroupName: str,
         clientToken: str = ...,
         description: str = ...,
         parentActionGroupSignature: Literal["AMAZON.UserInput"] = ...,
         actionGroupExecutor: ActionGroupExecutorTypeDef = ...,
         apiSchema: APISchemaTypeDef = ...,
-        actionGroupState: ActionGroupStateType = ...
+        actionGroupState: ActionGroupStateType = ...,
     ) -> CreateAgentActionGroupResponseTypeDef:
         """
         Creates an Action Group for existing Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgentActionGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_action_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_agent_action_group)
@@ -208,15 +207,15 @@
         self,
         *,
         agentId: str,
         agentAliasName: str,
         clientToken: str = ...,
         description: str = ...,
         routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAgentAliasResponseTypeDef:
         """
         Creates an Alias for an existing Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgentAlias).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_agent_alias)
@@ -227,15 +226,15 @@
         *,
         knowledgeBaseId: str,
         name: str,
         dataSourceConfiguration: DataSourceConfigurationTypeDef,
         clientToken: str = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...
+        vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Create a new data source See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateDataSource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_data_source)
@@ -246,15 +245,15 @@
         *,
         name: str,
         roleArn: str,
         knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,
         storageConfiguration: StorageConfigurationTypeDef,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Create a new knowledge base See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateKnowledgeBase).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_knowledge_base)
@@ -273,15 +272,15 @@
 
     async def delete_agent_action_group(
         self,
         *,
         agentId: str,
         agentVersion: str,
         actionGroupId: str,
-        skipResourceInUseCheck: bool = ...
+        skipResourceInUseCheck: bool = ...,
     ) -> Dict[str, Any]:
         """
         Deletes an Action Group for existing Amazon Bedrock Agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent_action_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#delete_agent_action_group)
         """
@@ -514,15 +513,15 @@
         self,
         *,
         knowledgeBaseId: str,
         dataSourceId: str,
         filters: Sequence[IngestionJobFilterTypeDef] = ...,
         sortBy: IngestionJobSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIngestionJobsResponseTypeDef:
         """
         List ingestion jobs See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListIngestionJobs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_ingestion_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#list_ingestion_jobs)
@@ -562,15 +561,15 @@
 
     async def start_ingestion_job(
         self,
         *,
         knowledgeBaseId: str,
         dataSourceId: str,
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> StartIngestionJobResponseTypeDef:
         """
         Start a new ingestion job See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/StartIngestionJob).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.start_ingestion_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#start_ingestion_job)
@@ -601,15 +600,15 @@
         agentName: str,
         agentResourceRoleArn: str,
         instruction: str = ...,
         foundationModel: str = ...,
         description: str = ...,
         idleSessionTTLInSeconds: int = ...,
         customerEncryptionKeyArn: str = ...,
-        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...
+        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
     ) -> UpdateAgentResponseTypeDef:
         """
         Updates an existing Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgent).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_agent)
@@ -622,15 +621,15 @@
         agentVersion: str,
         actionGroupId: str,
         actionGroupName: str,
         description: str = ...,
         parentActionGroupSignature: Literal["AMAZON.UserInput"] = ...,
         actionGroupExecutor: ActionGroupExecutorTypeDef = ...,
         actionGroupState: ActionGroupStateType = ...,
-        apiSchema: APISchemaTypeDef = ...
+        apiSchema: APISchemaTypeDef = ...,
     ) -> UpdateAgentActionGroupResponseTypeDef:
         """
         Updates an existing Action Group for Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentActionGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_action_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_agent_action_group)
@@ -639,15 +638,15 @@
     async def update_agent_alias(
         self,
         *,
         agentId: str,
         agentAliasId: str,
         agentAliasName: str,
         description: str = ...,
-        routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...
+        routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...,
     ) -> UpdateAgentAliasResponseTypeDef:
         """
         Updates an existing Alias for an Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentAlias).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_agent_alias)
@@ -656,15 +655,15 @@
     async def update_agent_knowledge_base(
         self,
         *,
         agentId: str,
         agentVersion: str,
         knowledgeBaseId: str,
         description: str = ...,
-        knowledgeBaseState: KnowledgeBaseStateType = ...
+        knowledgeBaseState: KnowledgeBaseStateType = ...,
     ) -> UpdateAgentKnowledgeBaseResponseTypeDef:
         """
         Updates an existing Knowledge Base associated to an Amazon Bedrock Agent See
         also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentKnowledgeBase).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_knowledge_base)
@@ -676,15 +675,15 @@
         *,
         knowledgeBaseId: str,
         dataSourceId: str,
         name: str,
         dataSourceConfiguration: DataSourceConfigurationTypeDef,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...
+        vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Update an existing data source See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateDataSource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_data_source)
@@ -694,15 +693,15 @@
         self,
         *,
         knowledgeBaseId: str,
         name: str,
         roleArn: str,
         knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,
         storageConfiguration: StorageConfigurationTypeDef,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateKnowledgeBaseResponseTypeDef:
         """
         Update an existing knowledge base See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateKnowledgeBase).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_knowledge_base)
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/client.pyi` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     async def associate_agent_knowledge_base(
         self,
         *,
         agentId: str,
         agentVersion: str,
         knowledgeBaseId: str,
         description: str,
-        knowledgeBaseState: KnowledgeBaseStateType = ...
+        knowledgeBaseState: KnowledgeBaseStateType = ...,
     ) -> AssociateAgentKnowledgeBaseResponseTypeDef:
         """
         Associate a Knowledge Base to an existing Amazon Bedrock Agent See also: [AWS
         API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/AssociateAgentKnowledgeBase).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.associate_agent_knowledge_base)
@@ -165,15 +165,15 @@
         clientToken: str = ...,
         instruction: str = ...,
         foundationModel: str = ...,
         description: str = ...,
         idleSessionTTLInSeconds: int = ...,
         customerEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
-        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...
+        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
     ) -> CreateAgentResponseTypeDef:
         """
         Creates an Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgent).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_agent)
@@ -186,15 +186,15 @@
         agentVersion: str,
         actionGroupName: str,
         clientToken: str = ...,
         description: str = ...,
         parentActionGroupSignature: Literal["AMAZON.UserInput"] = ...,
         actionGroupExecutor: ActionGroupExecutorTypeDef = ...,
         apiSchema: APISchemaTypeDef = ...,
-        actionGroupState: ActionGroupStateType = ...
+        actionGroupState: ActionGroupStateType = ...,
     ) -> CreateAgentActionGroupResponseTypeDef:
         """
         Creates an Action Group for existing Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgentActionGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_action_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_agent_action_group)
@@ -204,15 +204,15 @@
         self,
         *,
         agentId: str,
         agentAliasName: str,
         clientToken: str = ...,
         description: str = ...,
         routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAgentAliasResponseTypeDef:
         """
         Creates an Alias for an existing Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgentAlias).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_agent_alias)
@@ -223,15 +223,15 @@
         *,
         knowledgeBaseId: str,
         name: str,
         dataSourceConfiguration: DataSourceConfigurationTypeDef,
         clientToken: str = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...
+        vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Create a new data source See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateDataSource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_data_source)
@@ -242,15 +242,15 @@
         *,
         name: str,
         roleArn: str,
         knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,
         storageConfiguration: StorageConfigurationTypeDef,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Create a new knowledge base See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateKnowledgeBase).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#create_knowledge_base)
@@ -269,15 +269,15 @@
 
     async def delete_agent_action_group(
         self,
         *,
         agentId: str,
         agentVersion: str,
         actionGroupId: str,
-        skipResourceInUseCheck: bool = ...
+        skipResourceInUseCheck: bool = ...,
     ) -> Dict[str, Any]:
         """
         Deletes an Action Group for existing Amazon Bedrock Agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent_action_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#delete_agent_action_group)
         """
@@ -510,15 +510,15 @@
         self,
         *,
         knowledgeBaseId: str,
         dataSourceId: str,
         filters: Sequence[IngestionJobFilterTypeDef] = ...,
         sortBy: IngestionJobSortByTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIngestionJobsResponseTypeDef:
         """
         List ingestion jobs See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListIngestionJobs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_ingestion_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#list_ingestion_jobs)
@@ -558,15 +558,15 @@
 
     async def start_ingestion_job(
         self,
         *,
         knowledgeBaseId: str,
         dataSourceId: str,
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> StartIngestionJobResponseTypeDef:
         """
         Start a new ingestion job See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/StartIngestionJob).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.start_ingestion_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#start_ingestion_job)
@@ -597,15 +597,15 @@
         agentName: str,
         agentResourceRoleArn: str,
         instruction: str = ...,
         foundationModel: str = ...,
         description: str = ...,
         idleSessionTTLInSeconds: int = ...,
         customerEncryptionKeyArn: str = ...,
-        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...
+        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
     ) -> UpdateAgentResponseTypeDef:
         """
         Updates an existing Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgent).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_agent)
@@ -618,15 +618,15 @@
         agentVersion: str,
         actionGroupId: str,
         actionGroupName: str,
         description: str = ...,
         parentActionGroupSignature: Literal["AMAZON.UserInput"] = ...,
         actionGroupExecutor: ActionGroupExecutorTypeDef = ...,
         actionGroupState: ActionGroupStateType = ...,
-        apiSchema: APISchemaTypeDef = ...
+        apiSchema: APISchemaTypeDef = ...,
     ) -> UpdateAgentActionGroupResponseTypeDef:
         """
         Updates an existing Action Group for Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentActionGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_action_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_agent_action_group)
@@ -635,15 +635,15 @@
     async def update_agent_alias(
         self,
         *,
         agentId: str,
         agentAliasId: str,
         agentAliasName: str,
         description: str = ...,
-        routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...
+        routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...,
     ) -> UpdateAgentAliasResponseTypeDef:
         """
         Updates an existing Alias for an Amazon Bedrock Agent See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentAlias).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_agent_alias)
@@ -652,15 +652,15 @@
     async def update_agent_knowledge_base(
         self,
         *,
         agentId: str,
         agentVersion: str,
         knowledgeBaseId: str,
         description: str = ...,
-        knowledgeBaseState: KnowledgeBaseStateType = ...
+        knowledgeBaseState: KnowledgeBaseStateType = ...,
     ) -> UpdateAgentKnowledgeBaseResponseTypeDef:
         """
         Updates an existing Knowledge Base associated to an Amazon Bedrock Agent See
         also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentKnowledgeBase).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_knowledge_base)
@@ -672,15 +672,15 @@
         *,
         knowledgeBaseId: str,
         dataSourceId: str,
         name: str,
         dataSourceConfiguration: DataSourceConfigurationTypeDef,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...
+        vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Update an existing data source See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateDataSource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_data_source)
@@ -690,15 +690,15 @@
         self,
         *,
         knowledgeBaseId: str,
         name: str,
         roleArn: str,
         knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,
         storageConfiguration: StorageConfigurationTypeDef,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateKnowledgeBaseResponseTypeDef:
         """
         Update an existing knowledge base See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateKnowledgeBase).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/client/#update_knowledge_base)
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/literals.py` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/literals.py`

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
     "ActionGroupSignatureType",
     "ActionGroupStateType",
     "AgentAliasStatusType",
     "AgentStatusType",
     "ChunkingStrategyType",
     "CreationModeType",
@@ -50,15 +49,14 @@
     "SortOrderType",
     "AgentsforBedrockServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ActionGroupSignatureType = Literal["AMAZON.UserInput"]
 ActionGroupStateType = Literal["DISABLED", "ENABLED"]
 AgentAliasStatusType = Literal["CREATING", "DELETING", "FAILED", "PREPARED", "UPDATING"]
 AgentStatusType = Literal[
     "CREATING",
     "DELETING",
     "FAILED",
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/literals.pyi` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/paginator.py` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     "ListAgentVersionsPaginator",
     "ListAgentsPaginator",
     "ListDataSourcesPaginator",
     "ListIngestionJobsPaginator",
     "ListKnowledgeBasesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -175,15 +174,15 @@
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         dataSourceId: str,
         filters: Sequence[IngestionJobFilterTypeDef] = ...,
         sortBy: IngestionJobSortByTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIngestionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Paginator.ListIngestionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/paginators/#listingestionjobspaginator)
         """
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/paginator.pyi` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         dataSourceId: str,
         filters: Sequence[IngestionJobFilterTypeDef] = ...,
         sortBy: IngestionJobSortByTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIngestionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Paginator.ListIngestionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/paginators/#listingestionjobspaginator)
         """
 
 class ListKnowledgeBasesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/type_defs.py` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "S3IdentifierTypeDef",
     "ActionGroupExecutorTypeDef",
     "ActionGroupSummaryTypeDef",
     "AgentAliasRoutingConfigurationListItemTypeDef",
     "AgentKnowledgeBaseSummaryTypeDef",
     "AgentKnowledgeBaseTypeDef",
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent/type_defs.pyi` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/PKG-INFO` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-bedrock-agent
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AgentsforBedrock 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AgentsforBedrock 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/
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
 
 <a id="types-aiobotocore-bedrock-agent"></a>
 
 # types-aiobotocore-bedrock-agent
 
 [![PyPI - types-aiobotocore-bedrock-agent](https://img.shields.io/pypi/v/types-aiobotocore-bedrock-agent.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock-agent)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bedrock-agent.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bedrock-agent)](https://pepy.tech/project/types-aiobotocore-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AgentsforBedrock 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[aiobotocore.AgentsforBedrock 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
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
 [types-aiobotocore-bedrock-agent docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock_agent/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bedrock-agent-2.9.0/types_aiobotocore_bedrock_agent.egg-info/SOURCES.txt` & `types-aiobotocore-bedrock-agent-2.9.1/types_aiobotocore_bedrock_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

