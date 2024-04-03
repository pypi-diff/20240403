# Comparing `tmp/google_sheets_sdk-0.1.0.tar.gz` & `tmp/google_sheets_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_sheets_sdk-0.1.0.tar", max compression
+gzip compressed data, was "google_sheets_sdk-0.1.1.tar", max compression
```

## Comparing `google_sheets_sdk-0.1.0.tar` & `google_sheets_sdk-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-01 19:10:29.127500 google_sheets_sdk-0.1.0/README.md
--rw-r--r--   0        0        0       58 2024-04-01 19:18:01.048348 google_sheets_sdk-0.1.0/google_sheets_sdk/__init__.py
--rw-r--r--   0        0        0     2844 2024-04-01 19:18:33.360008 google_sheets_sdk-0.1.0/google_sheets_sdk/client.py
--rw-r--r--   0        0        0      617 2024-04-01 19:18:07.778334 google_sheets_sdk-0.1.0/google_sheets_sdk/helpers.py
--rw-r--r--   0        0        0      294 2024-04-01 19:14:11.517327 google_sheets_sdk-0.1.0/google_sheets_sdk/schemas.py
--rw-r--r--   0        0        0      432 2024-04-01 19:14:01.797309 google_sheets_sdk-0.1.0/google_sheets_sdk/settings.py
--rw-r--r--   0        0        0      407 2024-04-01 19:18:45.131380 google_sheets_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-01 19:10:29.127500 google_sheets_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0       74 2024-04-03 17:18:45.705883 google_sheets_sdk-0.1.1/google_sheets_sdk/__init__.py
+-rw-r--r--   0        0        0     2745 2024-04-03 17:18:12.204401 google_sheets_sdk-0.1.1/google_sheets_sdk/client.py
+-rw-r--r--   0        0        0      617 2024-04-01 19:18:07.778334 google_sheets_sdk-0.1.1/google_sheets_sdk/helpers.py
+-rw-r--r--   0        0        0      195 2024-04-03 17:19:12.947132 google_sheets_sdk-0.1.1/google_sheets_sdk/schemas.py
+-rw-r--r--   0        0        0      317 2024-04-03 17:17:23.401547 google_sheets_sdk-0.1.1/google_sheets_sdk/settings.py
+-rw-r--r--   0        0        0      407 2024-04-03 17:20:05.888516 google_sheets_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.1/PKG-INFO
```

### Comparing `google_sheets_sdk-0.1.0/google_sheets_sdk/client.py` & `google_sheets_sdk-0.1.1/google_sheets_sdk/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import time as t
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, ClassVar
+from typing import Any, ClassVar
 
-from httpx import HTTPStatusError
+from httpx import AsyncClient, HTTPStatusError
 from jose import jwt
 
+from google_sheets_sdk import Settings
 from google_sheets_sdk.helpers import check_token_expiration
 from google_sheets_sdk.schemas import TokenData
-from google_sheets_sdk.settings import get_settings
-
-if TYPE_CHECKING:
-    from google_sheets_sdk import Settings
-    from httpx import AsyncClient
 
 
 @dataclass
 class Client:
-    settings: ClassVar["Settings"] = get_settings()
+    settings: ClassVar["Settings"] = Settings()  # type: ignore
     base_url: ClassVar[str] = "https://sheets.googleapis.com/"
     token_data: ClassVar[TokenData] = TokenData(
         iss=settings.CLIENT_EMAIL,
         sub=settings.CLIENT_EMAIL,
         aud=f"{base_url}",
         scope=settings.SCOPE,
     )
```

### Comparing `google_sheets_sdk-0.1.0/google_sheets_sdk/helpers.py` & `google_sheets_sdk-0.1.1/google_sheets_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `google_sheets_sdk-0.1.0/PKG-INFO` & `google_sheets_sdk-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheets-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Marco Carmona
 Author-email: marcocarmonapy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

