# Comparing `tmp/types-aiobotocore-artifact-2.12.1.tar.gz` & `tmp/types-aiobotocore-artifact-2.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-artifact-2.12.1.tar", last modified: Tue Mar  5 01:14:36 2024, max compression
+gzip compressed data, was "types-aiobotocore-artifact-2.12.2.tar", last modified: Wed Apr  3 01:14:40 2024, max compression
```

## Comparing `types-aiobotocore-artifact-2.12.1.tar` & `types-aiobotocore-artifact-2.12.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:14:36.484130 types-aiobotocore-artifact-2.12.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-03-05 01:14:36.484130 types-aiobotocore-artifact-2.12.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 01:14:36.484130 types-aiobotocore-artifact-2.12.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:14:36.484130 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-03-05 00:58:25.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-05 00:58:24.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:14:36.484130 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-03-05 01:14:36.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-05 01:14:36.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 01:14:36.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 01:14:36.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 01:14:36.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-05 01:14:36.000000 types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:40.903348 types-aiobotocore-artifact-2.12.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-03 01:14:40.903348 types-aiobotocore-artifact-2.12.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:14:40.903348 types-aiobotocore-artifact-2.12.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:40.903348 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 00:59:08.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:40.903348 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-03 01:14:40.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-03 01:14:40.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:14:40.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:14:40.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 01:14:40.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 01:14:40.000000 types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-artifact-2.12.1/LICENSE` & `types-aiobotocore-artifact-2.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/PKG-INFO` & `types-aiobotocore-artifact-2.12.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-artifact
-Version: 2.12.1
-Summary: Type annotations for aiobotocore.Artifact 2.12.1 service generated with mypy-boto3-builder 7.23.2
+Version: 2.12.2
+Summary: Type annotations for aiobotocore.Artifact 2.12.2 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-artifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-artifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-artifact)](https://pepy.tech/project/types-aiobotocore-artifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Artifact 2.12.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
+[aiobotocore.Artifact 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-artifact-2.12.1/README.md` & `types-aiobotocore-artifact-2.12.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-artifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-artifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-artifact)](https://pepy.tech/project/types-aiobotocore-artifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Artifact 2.12.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
+[aiobotocore.Artifact 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-artifact-2.12.1/setup.py` & `types-aiobotocore-artifact-2.12.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-artifact",
-    version="2.12.1",
+    version="2.12.2",
     packages=["types_aiobotocore_artifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore.Artifact 2.12.1 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for aiobotocore.Artifact 2.12.2 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/__init__.py` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/__init__.pyi` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/__main__.py` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Artifact 2.12.1\n"
-        "Version:         2.12.1\n"
+        "Type annotations for aiobotocore.Artifact 2.12.2\n"
+        "Version:         2.12.2\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact\n"
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

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/client.py` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/client.pyi` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/literals.py` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/literals.pyi` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/paginator.py` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/paginator.pyi` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/type_defs.py` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact/type_defs.pyi` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/PKG-INFO` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-artifact
-Version: 2.12.1
-Summary: Type annotations for aiobotocore.Artifact 2.12.1 service generated with mypy-boto3-builder 7.23.2
+Version: 2.12.2
+Summary: Type annotations for aiobotocore.Artifact 2.12.2 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-artifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-artifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-artifact)](https://pepy.tech/project/types-aiobotocore-artifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Artifact 2.12.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
+[aiobotocore.Artifact 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-artifact-2.12.1/types_aiobotocore_artifact.egg-info/SOURCES.txt` & `types-aiobotocore-artifact-2.12.2/types_aiobotocore_artifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

