# Comparing `tmp/types-aiobotocore-lite-2.9.0.tar.gz` & `tmp/types-aiobotocore-lite-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lite-2.9.0.tar", last modified: Wed Dec 13 19:58:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-lite-2.9.1.tar", last modified: Thu Jan 18 01:19:56 2024, max compression
```

## Comparing `types-aiobotocore-lite-2.9.0.tar` & `types-aiobotocore-lite-2.9.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:28.030151 types-aiobotocore-lite-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:32.000000 types-aiobotocore-lite-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    87245 2023-12-13 19:58:28.030151 types-aiobotocore-lite-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    74949 2023-12-13 19:40:32.000000 types-aiobotocore-lite-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:28.030151 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/args.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/awsrequest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/configprovider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/eventstream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/httpchecksum.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/httpsession.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/paginate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/parsers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:32.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/regions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/retryhandler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/signers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/tokens.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/aiobotocore-stubs/waiter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:28.030151 types-aiobotocore-lite-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    54011 2023-12-13 19:40:31.000000 types-aiobotocore-lite-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:28.030151 types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    87245 2023-12-13 19:58:28.000000 types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-13 19:58:28.000000 types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:28.000000 types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:28.000000 types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    40320 2023-12-13 19:58:28.000000 types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-13 19:58:28.000000 types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:56.657544 types-aiobotocore-lite-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:31.000000 types-aiobotocore-lite-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   148414 2024-01-18 01:19:56.653544 types-aiobotocore-lite-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    74949 2024-01-18 01:02:31.000000 types-aiobotocore-lite-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:56.557545 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/args.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/awsrequest.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/configprovider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/eventstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/httpchecksum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/httpsession.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/paginate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/parsers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:31.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/regions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/retryhandler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/signers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/stub.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/tokens.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-18 01:02:30.000000 types-aiobotocore-lite-2.9.1/aiobotocore-stubs/waiter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:56.657544 types-aiobotocore-lite-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    53962 2024-01-18 01:02:31.000000 types-aiobotocore-lite-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:56.557545 types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)   148414 2024-01-18 01:19:56.000000 types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-18 01:19:56.000000 types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:56.000000 types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:56.000000 types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-01-18 01:19:56.000000 types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-18 01:19:56.000000 types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lite-2.9.0/LICENSE` & `types-aiobotocore-lite-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lite-2.9.0/README.md` & `types-aiobotocore-lite-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lite.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lite)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lite)](https://pepy.tech/project/types-aiobotocore-lite)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore 2.9.0](https://github.com/aio-libs/aiobotocore) compatible with
+[aiobotocore 2.9.1](https://github.com/aio-libs/aiobotocore) compatible with
 [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [types-aiobotocore-lite docs](https://youtype.github.io/types_aiobotocore_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/args.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/args.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/client.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/credentials.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/credentials.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 class AioDeferredRefreshableCredentials(AioRefreshableCredentials):
     method: Any
     def __init__(self, refresh_using: Any, method: Any, time_fetcher: Any = ...) -> None: ...
     def refresh_needed(self, refresh_in: Optional[Any] = ...) -> bool: ...
 
 class AioCachedCredentialFetcher(CachedCredentialFetcher):
-    async def fetch_credentials(self) -> Any: ...
+    async def fetch_credentials(self) -> Any: ...  # type: ignore [override]
 
 class AioBaseAssumeRoleCredentialFetcher(
     BaseAssumeRoleCredentialFetcher, AioCachedCredentialFetcher
 ): ...
 class AioAssumeRoleCredentialFetcher(
     AssumeRoleCredentialFetcher, AioBaseAssumeRoleCredentialFetcher
 ): ...
@@ -95,30 +95,30 @@
         extra_args: Optional[Any] = ...,
         cache: Optional[Any] = ...,
         expiry_window_seconds: Optional[Any] = ...,
     ) -> None: ...
 
 class AioProcessProvider(ProcessProvider):
     def __init__(self, *args: Any, popen: Any = ..., **kwargs: Any) -> None: ...
-    async def load(self) -> AioCredentials: ...
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioInstanceMetadataProvider(InstanceMetadataProvider):
-    async def load(self) -> AioRefreshableCredentials: ...
+    async def load(self) -> AioRefreshableCredentials: ...  # type: ignore [override]
 
 class AioEnvProvider(EnvProvider):
-    async def load(self) -> Any: ...
+    async def load(self) -> Any: ...  # type: ignore [override]
 
 class AioOriginalEC2Provider(OriginalEC2Provider):
-    async def load(self) -> AioCredentials: ...
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioSharedCredentialProvider(SharedCredentialProvider):
-    async def load(self) -> AioCredentials: ...
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioConfigProvider(ConfigProvider):
-    async def load(self) -> AioCredentials: ...
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioBotoProvider(BotoProvider):
     async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioAssumeRoleProvider(AssumeRoleProvider):
     async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore [override]
```

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/endpoint.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/handlers.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/handlers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/httpchecksum.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/httpchecksum.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/httpsession.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/paginate.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/paginate.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/parsers.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/regions.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/regions.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/response.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/retryhandler.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/retryhandler.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/session.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/signers.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/signers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/tokens.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/tokens.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/utils.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Mapping, Optional
 
 from botocore.utils import DEFAULT_METADATA_SERVICE_TIMEOUT as DEFAULT_METADATA_SERVICE_TIMEOUT
 from botocore.utils import METADATA_BASE_URL as METADATA_BASE_URL
 from botocore.utils import (
     ContainerMetadataFetcher,
     IMDSFetcher,
     IMDSRegionProvider,
@@ -36,24 +36,24 @@
 
 class AioInstanceMetadataRegionFetcher(AioIMDSFetcher, InstanceMetadataRegionFetcher):
     async def retrieve_region(self) -> Optional[str]: ...  # type: ignore [override]
 
 class AioS3RegionRedirectorv2(S3RegionRedirectorv2):
     async def redirect_from_error(
         self,
-        request_dict: Dict[str, Any],
+        request_dict: Mapping[str, Any],
         response: Response,
         operation: Any,
         **kwargs: Any,
     ) -> None: ...
     async def get_bucket_region(self, bucket: Any, response: Response) -> Any: ...
 
 class AioS3RegionRedirector(S3RegionRedirector):
     async def redirect_from_error(
-        self, request_dict: Dict[str, Any], response: Response, operation: Any, **kwargs: Any
+        self, request_dict: Mapping[str, Any], response: Response, operation: Any, **kwargs: Any
     ) -> Optional[int]: ...
     async def get_bucket_region(self, bucket: str, response: Response) -> str: ...
 
 class AioContainerMetadataFetcher(ContainerMetadataFetcher):
     def __init__(self, session: Optional[Any] = ..., sleep: Any = ...) -> None: ...
     async def retrieve_full_uri(self, full_url: str, headers: Optional[Any] = ...) -> str: ...
     async def retrieve_uri(self, relative_uri: str) -> Any: ...
```

### Comparing `types-aiobotocore-lite-2.9.0/aiobotocore-stubs/waiter.pyi` & `types-aiobotocore-lite-2.9.1/aiobotocore-stubs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.9.0/setup.py` & `types-aiobotocore-lite-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lite",
-    version="2.9.0",
+    version="2.9.1",
     packages=["aiobotocore-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore 2.9.0 generated with mypy-boto3-builder 7.21.0",
+    description="Type annotations for aiobotocore 2.9.1 generated with mypy-boto3-builder 7.23.1",
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
@@ -39,15 +38,15 @@
     ],
     keywords=(
         "aiobotocore type-annotations aiobotocore-stubs botocore-stubs mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"aiobotocore-stubs": ["py.typed", "*.pyi", "*/*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         "botocore-stubs",
@@ -435,15 +434,15 @@
             "types-aiobotocore-dynamodb>=2.9.0, <2.10.0",
             "types-aiobotocore-ec2>=2.9.0, <2.10.0",
             "types-aiobotocore-lambda>=2.9.0, <2.10.0",
             "types-aiobotocore-rds>=2.9.0, <2.10.0",
             "types-aiobotocore-s3>=2.9.0, <2.10.0",
             "types-aiobotocore-sqs>=2.9.0, <2.10.0",
         ],
-        "aiobotocore": ["aiobotocore==2.9.0", "botocore==1.33.13"],
+        "aiobotocore": ["aiobotocore==2.9.1", "botocore==1.33.13"],
         "accessanalyzer": ["types-aiobotocore-accessanalyzer>=2.9.0, <2.10.0"],
         "account": ["types-aiobotocore-account>=2.9.0, <2.10.0"],
         "acm": ["types-aiobotocore-acm>=2.9.0, <2.10.0"],
         "acm-pca": ["types-aiobotocore-acm-pca>=2.9.0, <2.10.0"],
         "alexaforbusiness": ["types-aiobotocore-alexaforbusiness>=2.9.0, <2.10.0"],
         "amp": ["types-aiobotocore-amp>=2.9.0, <2.10.0"],
         "amplify": ["types-aiobotocore-amplify>=2.9.0, <2.10.0"],
```

### Comparing `types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/SOURCES.txt` & `types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 aiobotocore-stubs/parsers.pyi
 aiobotocore-stubs/py.typed
 aiobotocore-stubs/regions.pyi
 aiobotocore-stubs/response.pyi
 aiobotocore-stubs/retryhandler.pyi
 aiobotocore-stubs/session.pyi
 aiobotocore-stubs/signers.pyi
+aiobotocore-stubs/stub.pyi
 aiobotocore-stubs/tokens.pyi
 aiobotocore-stubs/utils.pyi
 aiobotocore-stubs/waiter.pyi
 types_aiobotocore_lite.egg-info/PKG-INFO
 types_aiobotocore_lite.egg-info/SOURCES.txt
 types_aiobotocore_lite.egg-info/dependency_links.txt
 types_aiobotocore_lite.egg-info/not-zip-safe
```

### Comparing `types-aiobotocore-lite-2.9.0/types_aiobotocore_lite.egg-info/requires.txt` & `types-aiobotocore-lite-2.9.1/types_aiobotocore_lite.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [acm]
 types-aiobotocore-acm<2.10.0,>=2.9.0
 
 [acm-pca]
 types-aiobotocore-acm-pca<2.10.0,>=2.9.0
 
 [aiobotocore]
-aiobotocore==2.9.0
+aiobotocore==2.9.1
 botocore==1.33.13
 
 [alexaforbusiness]
 types-aiobotocore-alexaforbusiness<2.10.0,>=2.9.0
 
 [all]
 types-aiobotocore-accessanalyzer<2.10.0,>=2.9.0
```

