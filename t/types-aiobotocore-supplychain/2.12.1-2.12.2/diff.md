# Comparing `tmp/types-aiobotocore-supplychain-2.12.1.tar.gz` & `tmp/types-aiobotocore-supplychain-2.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-supplychain-2.12.1.tar", last modified: Tue Mar  5 01:16:28 2024, max compression
+gzip compressed data, was "types-aiobotocore-supplychain-2.12.2.tar", last modified: Wed Apr  3 01:16:32 2024, max compression
```

## Comparing `types-aiobotocore-supplychain-2.12.1.tar` & `types-aiobotocore-supplychain-2.12.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:16:28.775543 types-aiobotocore-supplychain-2.12.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-03-05 01:16:28.775543 types-aiobotocore-supplychain-2.12.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 01:16:28.775543 types-aiobotocore-supplychain-2.12.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:16:28.775543 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-03-05 01:13:14.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-03-05 01:13:14.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-05 01:13:14.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-05 01:13:14.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-05 01:13:13.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:16:28.775543 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-03-05 01:16:28.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-05 01:16:28.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 01:16:28.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 01:16:28.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 01:16:28.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-05 01:16:28.000000 types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:16:32.099492 types-aiobotocore-supplychain-2.12.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 01:13:18.000000 types-aiobotocore-supplychain-2.12.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-03 01:16:32.099492 types-aiobotocore-supplychain-2.12.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-03 01:13:18.000000 types-aiobotocore-supplychain-2.12.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:16:32.099492 types-aiobotocore-supplychain-2.12.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-03 01:13:18.000000 types-aiobotocore-supplychain-2.12.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:16:32.099492 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-03 01:13:19.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 01:13:18.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:16:32.099492 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-03 01:16:32.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-03 01:16:32.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:16:32.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:16:32.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 01:16:32.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 01:16:32.000000 types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-supplychain-2.12.1/LICENSE` & `types-aiobotocore-supplychain-2.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-supplychain-2.12.1/PKG-INFO` & `types-aiobotocore-supplychain-2.12.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-supplychain
-Version: 2.12.1
-Summary: Type annotations for aiobotocore.SupplyChain 2.12.1 service generated with mypy-boto3-builder 7.23.2
+Version: 2.12.2
+Summary: Type annotations for aiobotocore.SupplyChain 2.12.2 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_supplychain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-supplychain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-supplychain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_supplychain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-supplychain)](https://pepy.tech/project/types-aiobotocore-supplychain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupplyChain 2.12.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
+[aiobotocore.SupplyChain 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-supplychain-2.12.1/README.md` & `types-aiobotocore-supplychain-2.12.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-supplychain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-supplychain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_supplychain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-supplychain)](https://pepy.tech/project/types-aiobotocore-supplychain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupplyChain 2.12.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
+[aiobotocore.SupplyChain 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-supplychain-2.12.1/setup.py` & `types-aiobotocore-supplychain-2.12.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-supplychain",
-    version="2.12.1",
+    version="2.12.2",
     packages=["types_aiobotocore_supplychain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore.SupplyChain 2.12.1 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for aiobotocore.SupplyChain 2.12.2 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/__main__.py` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SupplyChain 2.12.1\n"
-        "Version:         2.12.1\n"
+        "Type annotations for aiobotocore.SupplyChain 2.12.2\n"
+        "Version:         2.12.2\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_supplychain//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.12.1")
+    print("2.12.2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/client.py` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/client.pyi` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/literals.py` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/literals.pyi` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/type_defs.py` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain/type_defs.pyi` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/PKG-INFO` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-supplychain
-Version: 2.12.1
-Summary: Type annotations for aiobotocore.SupplyChain 2.12.1 service generated with mypy-boto3-builder 7.23.2
+Version: 2.12.2
+Summary: Type annotations for aiobotocore.SupplyChain 2.12.2 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_supplychain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-supplychain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-supplychain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_supplychain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-supplychain)](https://pepy.tech/project/types-aiobotocore-supplychain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupplyChain 2.12.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
+[aiobotocore.SupplyChain 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-supplychain-2.12.1/types_aiobotocore_supplychain.egg-info/SOURCES.txt` & `types-aiobotocore-supplychain-2.12.2/types_aiobotocore_supplychain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

