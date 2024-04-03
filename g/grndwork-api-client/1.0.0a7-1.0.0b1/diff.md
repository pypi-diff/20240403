# Comparing `tmp/grndwork-api-client-1.0.0a7.tar.gz` & `tmp/grndwork-api-client-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grndwork-api-client-1.0.0a7.tar", last modified: Fri Jun 17 17:16:54 2022, max compression
+gzip compressed data, was "grndwork-api-client-1.0.0b1.tar", last modified: Wed Apr  3 19:40:21 2024, max compression
```

## Comparing `grndwork-api-client-1.0.0a7.tar` & `grndwork-api-client-1.0.0b1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 17:16:54.921306 grndwork-api-client-1.0.0a7/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1082 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9175 2022-06-17 17:16:54.921306 grndwork-api-client-1.0.0a7/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8621 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2022-06-17 17:16:54.921306 grndwork-api-client-1.0.0a7/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 17:16:54.917306 grndwork-api-client-1.0.0a7/src_py/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 17:16:54.921306 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      931 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1448 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/access_tokens.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2043 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      874 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      616 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/content_range.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1760 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/interfaces.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/make_paginated_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1246 2022-06-17 17:15:53.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/make_request.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 17:16:54.921306 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9175 2022-06-17 17:16:54.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      629 2022-06-17 17:16:54.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-17 17:16:54.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2022-06-17 17:16:54.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2022-06-17 17:16:54.000000 grndwork-api-client-1.0.0a7/src_py/grndwork_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 19:40:21.307938 grndwork-api-client-1.0.0b1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1082 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24287 2024-04-03 19:40:21.307938 grndwork-api-client-1.0.0b1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23676 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2024-04-03 19:40:21.307938 grndwork-api-client-1.0.0b1/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 19:40:21.303938 grndwork-api-client-1.0.0b1/src_py/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 19:40:21.303938 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1411 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1439 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/access_tokens.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16762 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/content_range.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/download_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/interfaces.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1408 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/make_paginated_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3063 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/make_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/run_concurrently.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-04-03 19:39:47.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 19:40:21.307938 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24287 2024-04-03 19:40:21.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      756 2024-04-03 19:40:21.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-03 19:40:21.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2024-04-03 19:40:21.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2024-04-03 19:40:21.000000 grndwork-api-client-1.0.0b1/src_py/grndwork_api_client.egg-info/top_level.txt
```

### Comparing `grndwork-api-client-1.0.0a7/LICENSE` & `grndwork-api-client-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `grndwork-api-client-1.0.0a7/setup.cfg` & `grndwork-api-client-1.0.0b1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = grndwork-api-client
-version = 1.0.0-alpha.7
+version = 1.0.0-beta.1
 author = GroundWork Renewables
 author_email = pypi@grndwork.com
 description = Groundwork API Client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GroundWorkRenewables/grndwork-api-client
 project_urls = 
@@ -14,18 +14,18 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src_py
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 install_requires = 
-	pyjwt ~= 2.4
-	requests ~= 2.27
+	pyjwt ~= 2.8
+	requests ~= 2.31
 
 [options.packages.find]
 where = src_py
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/__init__.py` & `grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,46 @@
+from typing import Optional
+
 from .client import Client
 from .config import get_refresh_token
 from .interfaces import (
+    ClientOptions,
     DataFile,
     DataFileHeaders,
+    DataFileWithRecords,
     DataRecord,
+    GetDataFilesQuery,
+    GetDataQCQuery,
     GetDataQuery,
+    GetDataRecordsQuery,
     GetStationsQuery,
     PostDataFile,
     PostDataPayload,
+    PostDataRecord,
+    ProjectManager,
+    QCRecord,
     RefreshToken,
     Station,
     StationDataFile,
+    StationWithDataFiles,
 )
 from .make_request import RequestError
 
 LOGGERNET_PLATFORM = 'loggernet'
 TRACE_PLATFORM = 'trace'
 
 
-def create_client(platform: str = LOGGERNET_PLATFORM) -> Client:
+def create_client(
+    platform: Optional[str] = None,
+    options: Optional[ClientOptions] = None,
+) -> Client:
     return Client(
-        refresh_token=get_refresh_token(),
-        platform=platform,
+        get_refresh_token(),
+        platform or LOGGERNET_PLATFORM,
+        options or {},
     )
 
 
 __all__ = [
     # Api client
     'create_client',
     'Client',
@@ -33,19 +48,27 @@
     # Platform constants
     'LOGGERNET_PLATFORM',
     'TRACE_PLATFORM',
 
     # Interfaces
     'DataFile',
     'DataFileHeaders',
+    'DataFileWithRecords',
     'DataRecord',
+    'GetDataFilesQuery',
+    'GetDataQCQuery',
     'GetDataQuery',
+    'GetDataRecordsQuery',
     'GetStationsQuery',
     'PostDataFile',
     'PostDataPayload',
+    'PostDataRecord',
+    'ProjectManager',
+    'QCRecord',
     'RefreshToken',
     'Station',
     'StationDataFile',
+    'StationWithDataFiles',
 
     # Errors
     'RequestError',
 ]
```

### Comparing `grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/access_tokens.py` & `grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/access_tokens.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,46 +22,46 @@
     scope: str,
 ) -> str:
     cache_key = f'{platform}:{scope}'
 
     access_token = access_token_cache.get(cache_key)
 
     if not access_token or has_expired(access_token):
-        access_token = create_access_token(refresh_token, platform, scope)
+        access_token = request_access_token(refresh_token, platform, scope)
         access_token_cache[cache_key] = access_token
 
     return access_token
 
 
-def create_access_token(
+def request_access_token(
     refresh_token: RefreshToken,
     platform: str,
     scope: str,
 ) -> str:
-    result, _ = make_request(
+    result = make_request(
         url=TOKENS_URL,
         method='POST',
         token=refresh_token['token'],
         body={
             'subject': refresh_token['subject'],
             'platform': platform,
             'scope': scope,
         },
-    )
+    )[0]
 
-    return cast(str, result.get('token'))
+    return cast(str, result['token'])
 
 
 def has_expired(token: str) -> bool:
     decoded_token = jwt.decode(
         token,
         algorithms=['HS256'],
         options={'verify_signature': False},
     )
 
     expiration = int(decoded_token.get('exp', 0))
-    now = int(time.time() * 1000)
+    now = int(time.time())
 
     if expiration and now - expiration >= 0:
         return True
 
     return False
```

### Comparing `grndwork-api-client-1.0.0a7/src_py/grndwork_api_client/config.py` & `grndwork-api-client-1.0.0b1/src_py/grndwork_api_client/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import json
 import os
 from typing import cast
 
 from .interfaces import RefreshToken
 
 API_URL = os.environ.get('GROUNDWORK_API_URL', 'https://api.grndwork.com')
-TOKENS_URL = f'{ API_URL }/v1/tokens'
-STATIONS_URL = f'{ API_URL }/v1/stations'
-DATA_URL = f'{ API_URL }/v1/data'
+
+TOKENS_URL = f'{API_URL}/v1/tokens'
+STATIONS_URL = f'{API_URL}/v1/stations'
+REPORTS_URL = f'{API_URL}/v1/reports'
+EXPORTS_URL = f'{API_URL}/v1/exports'
+FILES_URL = f'{API_URL}/v1/files'
+DATA_URL = f'{API_URL}/v1/data'
+QC_URL = f'{API_URL}/v1/qc'
 
 
 def get_refresh_token() -> RefreshToken:
     groundwork_token_path = os.environ.get('GROUNDWORK_TOKEN_PATH')
     groundwork_subject = os.environ.get('GROUNDWORK_SUBJECT')
     groundwork_token = os.environ.get('GROUNDWORK_TOKEN')
```

### Comparing `grndwork-api-client-1.0.0a7/src_py/grndwork_api_client.egg-info/SOURCES.txt` & `grndwork-api-client-1.0.0b1/src_py/grndwork_api_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 pyproject.toml
 setup.cfg
 src_py/grndwork_api_client/__init__.py
 src_py/grndwork_api_client/access_tokens.py
 src_py/grndwork_api_client/client.py
 src_py/grndwork_api_client/config.py
 src_py/grndwork_api_client/content_range.py
+src_py/grndwork_api_client/download_file.py
 src_py/grndwork_api_client/interfaces.py
 src_py/grndwork_api_client/make_paginated_request.py
 src_py/grndwork_api_client/make_request.py
+src_py/grndwork_api_client/run_concurrently.py
+src_py/grndwork_api_client/utils.py
 src_py/grndwork_api_client.egg-info/PKG-INFO
 src_py/grndwork_api_client.egg-info/SOURCES.txt
 src_py/grndwork_api_client.egg-info/dependency_links.txt
 src_py/grndwork_api_client.egg-info/requires.txt
 src_py/grndwork_api_client.egg-info/top_level.txt
```

