# Comparing `tmp/mypy-boto3-docdb-1.34.13.tar.gz` & `tmp/mypy-boto3-docdb-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-docdb-1.34.13.tar", last modified: Thu Jan  4 21:07:09 2024, max compression
+gzip compressed data, was "mypy-boto3-docdb-1.34.77.tar", last modified: Wed Apr  3 19:32:39 2024, max compression
```

## Comparing `mypy-boto3-docdb-1.34.13.tar` & `mypy-boto3-docdb-1.34.77.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 21:07:09.040185 mypy-boto3-docdb-1.34.13/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-04 21:06:20.000000 mypy-boto3-docdb-1.34.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-01-04 21:07:09.040185 mypy-boto3-docdb-1.34.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-01-04 21:06:20.000000 mypy-boto3-docdb-1.34.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 21:07:09.036185 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-01-04 21:06:20.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-01-04 21:06:20.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-04 21:06:20.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51508 2024-01-04 21:06:21.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    51505 2024-01-04 21:06:21.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-04 21:06:21.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-04 21:06:21.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17379 2024-01-04 21:06:21.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-01-04 21:06:21.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 21:06:20.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56567 2024-01-04 21:06:22.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56567 2024-01-04 21:06:22.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-04 21:06:20.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-01-04 21:06:21.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-01-04 21:06:21.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 21:07:09.040185 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-01-04 21:07:09.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-04 21:07:09.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 21:07:09.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 21:07:09.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-04 21:07:09.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-04 21:07:09.000000 mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-04 21:07:09.040185 mypy-boto3-docdb-1.34.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-04 21:06:20.000000 mypy-boto3-docdb-1.34.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:39.200161 mypy-boto3-docdb-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15453 2024-04-03 19:32:39.200161 mypy-boto3-docdb-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:39.200161 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52201 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52198 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-03 19:32:10.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17379 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57092 2024-04-03 19:32:10.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57092 2024-04-03 19:32:10.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:39.200161 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15453 2024-04-03 19:32:39.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-03 19:32:39.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:39.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:39.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:39.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 19:32:39.000000 mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:39.200161 mypy-boto3-docdb-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-03 19:32:09.000000 mypy-boto3-docdb-1.34.77/setup.py
```

### Comparing `mypy-boto3-docdb-1.34.13/LICENSE` & `mypy-boto3-docdb-1.34.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.34.13/PKG-INFO` & `mypy-boto3-docdb-1.34.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.34.13
-Summary: Type annotations for boto3.DocDB 1.34.13 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.77
+Summary: Type annotations for boto3.DocDB 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.34.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-docdb-1.34.13/README.md` & `mypy-boto3-docdb-1.34.77/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.34.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/__init__.py` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/__init__.pyi` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/__main__.py` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DocDB 1.34.13\nVersion:         1.34.13\nBuilder version:"
-        " 7.23.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.DocDB 1.34.77\n"
+        "Version:         1.34.77\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.13")
+    print("1.34.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/client.py` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     RebootDBInstanceResultTypeDef,
     RemoveFromGlobalClusterResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
     StartDBClusterResultTypeDef,
     StopDBClusterResultTypeDef,
+    SwitchoverGlobalClusterResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 12):
@@ -1009,14 +1010,26 @@
         """
         Stops the running cluster that is specified by `DBClusterIdentifier`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.stop_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#stop_db_cluster)
         """
 
+    def switchover_global_cluster(
+        self, *, GlobalClusterIdentifier: str, TargetDbClusterIdentifier: str
+    ) -> SwitchoverGlobalClusterResultTypeDef:
+        """
+        Switches over the specified secondary Amazon DocumentDB cluster to be the new
+        primary Amazon DocumentDB cluster in the global database
+        cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.switchover_global_cluster)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#switchover_global_cluster)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_certificates"]
     ) -> DescribeCertificatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#get_paginator)
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/client.pyi` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     RebootDBInstanceResultTypeDef,
     RemoveFromGlobalClusterResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
     StartDBClusterResultTypeDef,
     StopDBClusterResultTypeDef,
+    SwitchoverGlobalClusterResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 12):
@@ -1006,14 +1007,26 @@
         """
         Stops the running cluster that is specified by `DBClusterIdentifier`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.stop_db_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#stop_db_cluster)
         """
 
+    def switchover_global_cluster(
+        self, *, GlobalClusterIdentifier: str, TargetDbClusterIdentifier: str
+    ) -> SwitchoverGlobalClusterResultTypeDef:
+        """
+        Switches over the specified secondary Amazon DocumentDB cluster to be the new
+        primary Amazon DocumentDB cluster in the global database
+        cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.switchover_global_cluster)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#switchover_global_cluster)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_certificates"]
     ) -> DescribeCertificatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#get_paginator)
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/literals.py` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -110,14 +111,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -135,14 +137,15 @@
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
@@ -165,14 +168,15 @@
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
@@ -233,15 +237,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -415,19 +418,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/literals.pyi` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -110,14 +111,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -135,14 +137,15 @@
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
@@ -165,14 +168,15 @@
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
@@ -233,15 +237,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -415,19 +418,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/paginator.py` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/paginator.pyi` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/type_defs.py` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
+    "SwitchoverGlobalClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
@@ -167,14 +168,15 @@
     "StopDBClusterResultTypeDef",
     "DBEngineVersionMessageTypeDef",
     "CreateGlobalClusterResultTypeDef",
     "DeleteGlobalClusterResultTypeDef",
     "GlobalClustersMessageTypeDef",
     "ModifyGlobalClusterResultTypeDef",
     "RemoveFromGlobalClusterResultTypeDef",
+    "SwitchoverGlobalClusterResultTypeDef",
     "ApplyPendingMaintenanceActionResultTypeDef",
     "PendingMaintenanceActionsMessageTypeDef",
     "CreateDBSubnetGroupResultTypeDef",
     "DBInstanceTypeDef",
     "DBSubnetGroupMessageTypeDef",
     "ModifyDBSubnetGroupResultTypeDef",
     "CreateDBInstanceResultTypeDef",
@@ -206,18 +208,18 @@
         "EventSubscriptionArn": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": NotRequired[str],
         "Value": NotRequired[str],
@@ -590,14 +592,21 @@
 )
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
+SwitchoverGlobalClusterMessageRequestTypeDef = TypedDict(
+    "SwitchoverGlobalClusterMessageRequestTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "TargetDbClusterIdentifier": str,
+    },
+)
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1499,14 +1508,21 @@
 RemoveFromGlobalClusterResultTypeDef = TypedDict(
     "RemoveFromGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SwitchoverGlobalClusterResultTypeDef = TypedDict(
+    "SwitchoverGlobalClusterResultTypeDef",
+    {
+        "GlobalCluster": GlobalClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/type_defs.pyi` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
+    "SwitchoverGlobalClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
@@ -167,14 +168,15 @@
     "StopDBClusterResultTypeDef",
     "DBEngineVersionMessageTypeDef",
     "CreateGlobalClusterResultTypeDef",
     "DeleteGlobalClusterResultTypeDef",
     "GlobalClustersMessageTypeDef",
     "ModifyGlobalClusterResultTypeDef",
     "RemoveFromGlobalClusterResultTypeDef",
+    "SwitchoverGlobalClusterResultTypeDef",
     "ApplyPendingMaintenanceActionResultTypeDef",
     "PendingMaintenanceActionsMessageTypeDef",
     "CreateDBSubnetGroupResultTypeDef",
     "DBInstanceTypeDef",
     "DBSubnetGroupMessageTypeDef",
     "ModifyDBSubnetGroupResultTypeDef",
     "CreateDBInstanceResultTypeDef",
@@ -206,18 +208,18 @@
         "EventSubscriptionArn": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": NotRequired[str],
         "Value": NotRequired[str],
@@ -590,14 +592,21 @@
 )
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
+SwitchoverGlobalClusterMessageRequestTypeDef = TypedDict(
+    "SwitchoverGlobalClusterMessageRequestTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "TargetDbClusterIdentifier": str,
+    },
+)
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1499,14 +1508,21 @@
 RemoveFromGlobalClusterResultTypeDef = TypedDict(
     "RemoveFromGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SwitchoverGlobalClusterResultTypeDef = TypedDict(
+    "SwitchoverGlobalClusterResultTypeDef",
+    {
+        "GlobalCluster": GlobalClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/waiter.py` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb/waiter.pyi` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/PKG-INFO` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.34.13
-Summary: Type annotations for boto3.DocDB 1.34.13 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.77
+Summary: Type annotations for boto3.DocDB 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.34.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-docdb-1.34.13/mypy_boto3_docdb.egg-info/SOURCES.txt` & `mypy-boto3-docdb-1.34.77/mypy_boto3_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.34.13/setup.py` & `mypy-boto3-docdb-1.34.77/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-docdb",
-    version="1.34.13",
+    version="1.34.77",
     packages=["mypy_boto3_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.DocDB 1.34.13 service generated with mypy-boto3-builder 7.23.0"
-    ),
+    description="Type annotations for boto3.DocDB 1.34.77 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

