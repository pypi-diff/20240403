# Comparing `tmp/mypy-boto3-transfer-1.34.59.tar.gz` & `tmp/mypy-boto3-transfer-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.34.59.tar", last modified: Fri Mar  8 20:21:21 2024, max compression
+gzip compressed data, was "mypy-boto3-transfer-1.34.77.tar", last modified: Wed Apr  3 19:32:40 2024, max compression
```

## Comparing `mypy-boto3-transfer-1.34.59.tar` & `mypy-boto3-transfer-1.34.77.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:21.278134 mypy-boto3-transfer-1.34.59/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-08 20:21:07.000000 mypy-boto3-transfer-1.34.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-03-08 20:21:21.278134 mypy-boto3-transfer-1.34.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-03-08 20:21:07.000000 mypy-boto3-transfer-1.34.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:21.274134 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-08 20:21:07.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-08 20:21:07.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-08 20:21:07.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47383 2024-03-08 20:21:08.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    47380 2024-03-08 20:21:08.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13041 2024-03-08 20:21:08.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13041 2024-03-08 20:21:08.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-03-08 20:21:08.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-03-08 20:21:08.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:07.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    51272 2024-03-08 20:21:09.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51272 2024-03-08 20:21:09.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-08 20:21:07.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-08 20:21:08.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-08 20:21:08.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:21.278134 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-03-08 20:21:21.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-08 20:21:21.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:21:21.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:21:21.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-08 20:21:21.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-08 20:21:21.000000 mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 20:21:21.278134 mypy-boto3-transfer-1.34.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-08 20:21:07.000000 mypy-boto3-transfer-1.34.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47413 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47410 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2024-04-03 19:32:27.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2024-04-03 19:32:27.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/setup.py
```

### Comparing `mypy-boto3-transfer-1.34.59/LICENSE` & `mypy-boto3-transfer-1.34.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.59/PKG-INFO` & `mypy-boto3-transfer-1.34.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.34.59
-Summary: Type annotations for boto3.Transfer 1.34.59 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.Transfer 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.34.59/README.md` & `mypy-boto3-transfer-1.34.77/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/__init__.py` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/__init__.pyi` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/__main__.py` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.34.59\n"
-        "Version:         1.34.59\n"
+        "Type annotations for boto3.Transfer 1.34.77\n"
+        "Version:         1.34.77\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.59")
+    print("1.34.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/client.py` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,15 @@
         *,
         Url: str,
         AccessRole: str,
         As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SftpConfig: SftpConnectorConfigTypeDef = ...,
+        SecurityPolicyName: str = ...,
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for a connection for the
         AS2 or SFTP
         protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
@@ -461,17 +462,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_profile)
         """
 
     def describe_security_policy(
         self, *, SecurityPolicyName: str
     ) -> DescribeSecurityPolicyResponseTypeDef:
         """
-        Describes the security policy that is attached to your file transfer
-        protocol-enabled
-        server.
+        Describes the security policy that is attached to your server or SFTP connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_security_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_security_policy)
         """
 
     def describe_server(self, *, ServerId: str) -> DescribeServerResponseTypeDef:
         """
@@ -639,17 +638,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_profiles)
         """
 
     def list_security_policies(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSecurityPoliciesResponseTypeDef:
         """
-        Lists the security policies that are attached to your file transfer
-        protocol-enabled
-        servers.
+        Lists the security policies that are attached to your servers and SFTP
+        connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_security_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_security_policies)
         """
 
     def list_servers(
         self, *, MaxResults: int = ..., NextToken: str = ...
@@ -851,14 +849,15 @@
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
         LoggingRole: str = ...,
         SftpConfig: SftpConnectorConfigTypeDef = ...,
+        SecurityPolicyName: str = ...,
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_connector)
         """
```

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/client.pyi` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,15 @@
         *,
         Url: str,
         AccessRole: str,
         As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SftpConfig: SftpConnectorConfigTypeDef = ...,
+        SecurityPolicyName: str = ...,
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for a connection for the
         AS2 or SFTP
         protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
@@ -458,17 +459,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_profile)
         """
 
     def describe_security_policy(
         self, *, SecurityPolicyName: str
     ) -> DescribeSecurityPolicyResponseTypeDef:
         """
-        Describes the security policy that is attached to your file transfer
-        protocol-enabled
-        server.
+        Describes the security policy that is attached to your server or SFTP connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_security_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_security_policy)
         """
 
     def describe_server(self, *, ServerId: str) -> DescribeServerResponseTypeDef:
         """
@@ -636,17 +635,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_profiles)
         """
 
     def list_security_policies(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSecurityPoliciesResponseTypeDef:
         """
-        Lists the security policies that are attached to your file transfer
-        protocol-enabled
-        servers.
+        Lists the security policies that are attached to your servers and SFTP
+        connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_security_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_security_policies)
         """
 
     def list_servers(
         self, *, MaxResults: int = ..., NextToken: str = ...
@@ -848,14 +846,15 @@
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
         LoggingRole: str = ...,
         SftpConfig: SftpConnectorConfigTypeDef = ...,
+        SecurityPolicyName: str = ...,
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_connector)
         """
```

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/literals.py` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     "ListWorkflowsPaginatorName",
     "MapTypeType",
     "MdnResponseType",
     "MdnSigningAlgType",
     "OverwriteExistingType",
     "ProfileTypeType",
     "ProtocolType",
+    "SecurityPolicyProtocolType",
+    "SecurityPolicyResourceTypeType",
     "ServerOfflineWaiterName",
     "ServerOnlineWaiterName",
     "SetStatOptionType",
     "SftpAuthenticationMethodsType",
     "SigningAlgType",
     "StateType",
     "TlsSessionResumptionModeType",
@@ -109,14 +111,16 @@
 ListWorkflowsPaginatorName = Literal["list_workflows"]
 MapTypeType = Literal["DIRECTORY", "FILE"]
 MdnResponseType = Literal["NONE", "SYNC"]
 MdnSigningAlgType = Literal["DEFAULT", "NONE", "SHA1", "SHA256", "SHA384", "SHA512"]
 OverwriteExistingType = Literal["FALSE", "TRUE"]
 ProfileTypeType = Literal["LOCAL", "PARTNER"]
 ProtocolType = Literal["AS2", "FTP", "FTPS", "SFTP"]
+SecurityPolicyProtocolType = Literal["FTPS", "SFTP"]
+SecurityPolicyResourceTypeType = Literal["CONNECTOR", "SERVER"]
 ServerOfflineWaiterName = Literal["server_offline"]
 ServerOnlineWaiterName = Literal["server_online"]
 SetStatOptionType = Literal["DEFAULT", "ENABLE_NO_OP"]
 SftpAuthenticationMethodsType = Literal[
     "PASSWORD", "PUBLIC_KEY", "PUBLIC_KEY_AND_PASSWORD", "PUBLIC_KEY_OR_PASSWORD"
 ]
 SigningAlgType = Literal["NONE", "SHA1", "SHA256", "SHA384", "SHA512"]
@@ -191,14 +195,15 @@
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
@@ -221,14 +226,15 @@
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
@@ -289,15 +295,14 @@
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
@@ -477,14 +482,15 @@
     "sts",
     "supplychain",
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

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/literals.pyi` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     "ListWorkflowsPaginatorName",
     "MapTypeType",
     "MdnResponseType",
     "MdnSigningAlgType",
     "OverwriteExistingType",
     "ProfileTypeType",
     "ProtocolType",
+    "SecurityPolicyProtocolType",
+    "SecurityPolicyResourceTypeType",
     "ServerOfflineWaiterName",
     "ServerOnlineWaiterName",
     "SetStatOptionType",
     "SftpAuthenticationMethodsType",
     "SigningAlgType",
     "StateType",
     "TlsSessionResumptionModeType",
@@ -109,14 +111,16 @@
 ListWorkflowsPaginatorName = Literal["list_workflows"]
 MapTypeType = Literal["DIRECTORY", "FILE"]
 MdnResponseType = Literal["NONE", "SYNC"]
 MdnSigningAlgType = Literal["DEFAULT", "NONE", "SHA1", "SHA256", "SHA384", "SHA512"]
 OverwriteExistingType = Literal["FALSE", "TRUE"]
 ProfileTypeType = Literal["LOCAL", "PARTNER"]
 ProtocolType = Literal["AS2", "FTP", "FTPS", "SFTP"]
+SecurityPolicyProtocolType = Literal["FTPS", "SFTP"]
+SecurityPolicyResourceTypeType = Literal["CONNECTOR", "SERVER"]
 ServerOfflineWaiterName = Literal["server_offline"]
 ServerOnlineWaiterName = Literal["server_online"]
 SetStatOptionType = Literal["DEFAULT", "ENABLE_NO_OP"]
 SftpAuthenticationMethodsType = Literal[
     "PASSWORD", "PUBLIC_KEY", "PUBLIC_KEY_AND_PASSWORD", "PUBLIC_KEY_OR_PASSWORD"
 ]
 SigningAlgType = Literal["NONE", "SHA1", "SHA256", "SHA384", "SHA512"]
@@ -191,14 +195,15 @@
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
@@ -221,14 +226,15 @@
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
@@ -289,15 +295,14 @@
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
@@ -477,14 +482,15 @@
     "sts",
     "supplychain",
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

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/paginator.py` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/paginator.pyi` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/type_defs.py` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     IdentityProviderTypeType,
     MapTypeType,
     MdnResponseType,
     MdnSigningAlgType,
     OverwriteExistingType,
     ProfileTypeType,
     ProtocolType,
+    SecurityPolicyProtocolType,
+    SecurityPolicyResourceTypeType,
     SetStatOptionType,
     SftpAuthenticationMethodsType,
     SigningAlgType,
     StateType,
     TlsSessionResumptionModeType,
     WorkflowStepTypeType,
 )
@@ -461,14 +463,17 @@
     {
         "SecurityPolicyName": str,
         "Fips": NotRequired[bool],
         "SshCiphers": NotRequired[List[str]],
         "SshKexs": NotRequired[List[str]],
         "SshMacs": NotRequired[List[str]],
         "TlsCiphers": NotRequired[List[str]],
+        "SshHostKeyAlgorithms": NotRequired[List[str]],
+        "Type": NotRequired[SecurityPolicyResourceTypeType],
+        "Protocols": NotRequired[List[SecurityPolicyProtocolType]],
     },
 )
 DescribeServerRequestRequestTypeDef = TypedDict(
     "DescribeServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
@@ -1193,39 +1198,42 @@
     {
         "Url": str,
         "AccessRole": str,
         "As2Config": NotRequired[As2ConnectorConfigTypeDef],
         "LoggingRole": NotRequired[str],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "SftpConfig": NotRequired[SftpConnectorConfigTypeDef],
+        "SecurityPolicyName": NotRequired[str],
     },
 )
 DescribedConnectorTypeDef = TypedDict(
     "DescribedConnectorTypeDef",
     {
         "Arn": str,
         "ConnectorId": NotRequired[str],
         "Url": NotRequired[str],
         "As2Config": NotRequired[As2ConnectorConfigTypeDef],
         "AccessRole": NotRequired[str],
         "LoggingRole": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "SftpConfig": NotRequired[SftpConnectorConfigTypeDef],
         "ServiceManagedEgressIpAddresses": NotRequired[List[str]],
+        "SecurityPolicyName": NotRequired[str],
     },
 )
 UpdateConnectorRequestRequestTypeDef = TypedDict(
     "UpdateConnectorRequestRequestTypeDef",
     {
         "ConnectorId": str,
         "Url": NotRequired[str],
         "As2Config": NotRequired[As2ConnectorConfigTypeDef],
         "AccessRole": NotRequired[str],
         "LoggingRole": NotRequired[str],
         "SftpConfig": NotRequired[SftpConnectorConfigTypeDef],
+        "SecurityPolicyName": NotRequired[str],
     },
 )
 DescribeSecurityPolicyResponseTypeDef = TypedDict(
     "DescribeSecurityPolicyResponseTypeDef",
     {
         "SecurityPolicy": DescribedSecurityPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/type_defs.pyi` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     IdentityProviderTypeType,
     MapTypeType,
     MdnResponseType,
     MdnSigningAlgType,
     OverwriteExistingType,
     ProfileTypeType,
     ProtocolType,
+    SecurityPolicyProtocolType,
+    SecurityPolicyResourceTypeType,
     SetStatOptionType,
     SftpAuthenticationMethodsType,
     SigningAlgType,
     StateType,
     TlsSessionResumptionModeType,
     WorkflowStepTypeType,
 )
@@ -461,14 +463,17 @@
     {
         "SecurityPolicyName": str,
         "Fips": NotRequired[bool],
         "SshCiphers": NotRequired[List[str]],
         "SshKexs": NotRequired[List[str]],
         "SshMacs": NotRequired[List[str]],
         "TlsCiphers": NotRequired[List[str]],
+        "SshHostKeyAlgorithms": NotRequired[List[str]],
+        "Type": NotRequired[SecurityPolicyResourceTypeType],
+        "Protocols": NotRequired[List[SecurityPolicyProtocolType]],
     },
 )
 DescribeServerRequestRequestTypeDef = TypedDict(
     "DescribeServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
@@ -1193,39 +1198,42 @@
     {
         "Url": str,
         "AccessRole": str,
         "As2Config": NotRequired[As2ConnectorConfigTypeDef],
         "LoggingRole": NotRequired[str],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "SftpConfig": NotRequired[SftpConnectorConfigTypeDef],
+        "SecurityPolicyName": NotRequired[str],
     },
 )
 DescribedConnectorTypeDef = TypedDict(
     "DescribedConnectorTypeDef",
     {
         "Arn": str,
         "ConnectorId": NotRequired[str],
         "Url": NotRequired[str],
         "As2Config": NotRequired[As2ConnectorConfigTypeDef],
         "AccessRole": NotRequired[str],
         "LoggingRole": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "SftpConfig": NotRequired[SftpConnectorConfigTypeDef],
         "ServiceManagedEgressIpAddresses": NotRequired[List[str]],
+        "SecurityPolicyName": NotRequired[str],
     },
 )
 UpdateConnectorRequestRequestTypeDef = TypedDict(
     "UpdateConnectorRequestRequestTypeDef",
     {
         "ConnectorId": str,
         "Url": NotRequired[str],
         "As2Config": NotRequired[As2ConnectorConfigTypeDef],
         "AccessRole": NotRequired[str],
         "LoggingRole": NotRequired[str],
         "SftpConfig": NotRequired[SftpConnectorConfigTypeDef],
+        "SecurityPolicyName": NotRequired[str],
     },
 )
 DescribeSecurityPolicyResponseTypeDef = TypedDict(
     "DescribeSecurityPolicyResponseTypeDef",
     {
         "SecurityPolicy": DescribedSecurityPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/waiter.py` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer/waiter.pyi` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.34.59
-Summary: Type annotations for boto3.Transfer 1.34.59 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.Transfer 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.34.59/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.59/setup.py` & `mypy-boto3-transfer-1.34.77/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.34.59",
+    version="1.34.77",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Transfer 1.34.59 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Transfer 1.34.77 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

