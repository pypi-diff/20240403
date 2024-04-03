# Comparing `tmp/aioautomower-2024.3.5.tar.gz` & `tmp/aioautomower-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2024.3.5.tar", last modified: Sat Mar 30 20:40:29 2024, max compression
+gzip compressed data, was "aioautomower-2024.4.0.tar", last modified: Wed Apr  3 17:20:57 2024, max compression
```

## Comparing `aioautomower-2024.3.5.tar` & `aioautomower-2024.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:40:29.890077 aioautomower-2024.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-30 20:40:29.890077 aioautomower-2024.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:40:29.890077 aioautomower-2024.3.5/aioautomower/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/aioautomower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/aioautomower/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/aioautomower/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/aioautomower/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/aioautomower/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/aioautomower/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/aioautomower/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/aioautomower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:40:29.890077 aioautomower-2024.3.5/aioautomower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-30 20:40:29.000000 aioautomower-2024.3.5/aioautomower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-30 20:40:29.000000 aioautomower-2024.3.5/aioautomower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:40:29.000000 aioautomower-2024.3.5/aioautomower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:40:29.000000 aioautomower-2024.3.5/aioautomower.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-30 20:40:29.000000 aioautomower-2024.3.5/aioautomower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-30 20:40:29.000000 aioautomower-2024.3.5/aioautomower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-30 20:40:27.000000 aioautomower-2024.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 20:40:29.890077 aioautomower-2024.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:40:29.890077 aioautomower-2024.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/tests/test_error_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/tests/test_high_feature_mower_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/tests/test_jwt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-30 20:40:26.000000 aioautomower-2024.3.5/tests/test_low_feature_mower_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/aioautomower/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/aioautomower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:20:56.000000 aioautomower-2024.4.0/aioautomower.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 17:20:53.000000 aioautomower-2024.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/tests/test_error_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/tests/test_high_feature_mower_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/tests/test_jwt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/tests/test_low_feature_mower_model.py
```

### Comparing `aioautomower-2024.3.5/PKG-INFO` & `aioautomower-2024.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2024.3.5
+Version: 2024.4.0
 Summary: MPython module to talk to Husqvarna Automower.
 Author-email: Thomas Protzner <thomas.protzner@gmail.com>
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/Thomas55555/aioautomower
 Project-URL: Repository, https://github.com/Thomas55555/aioautomower
 Project-URL: Issues, https://github.com/Thomas55555/aioautomower/issues
 Platform: any
```

### Comparing `aioautomower-2024.3.5/README.md` & `aioautomower-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.3.5/aioautomower/auth.py` & `aioautomower-2024.4.0/aioautomower/auth.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.3.5/aioautomower/const.py` & `aioautomower-2024.4.0/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.3.5/aioautomower/example.py` & `aioautomower-2024.4.0/aioautomower/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """An example file to use this library."""
 
 import asyncio
 import logging
 import time
 from typing import cast
-
+import zoneinfo
 from aiohttp import ClientSession
-
 from aioautomower.auth import AbstractAuth
 from aioautomower.const import API_BASE_URL
 from aioautomower.session import AutomowerSession
 from aioautomower.model import MowerAttributes
-from aioautomower.utils import async_get_access_token, structure_token
+from aioautomower.utils import (
+    async_get_access_token,
+    structure_token,
+    convert_timestamp_to_datetime_utc,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 
 CLIENT_ID = "1e33fa27-ca34-4762-9a9e-5967f873a733"
 CLIENT_SECRET = "763adf3c-1b16-4c3b-91cd-c07316243880"
 CLOCK_OUT_OF_SYNC_MAX_SEC = 20
@@ -86,14 +89,20 @@
     await websession.close()
 
 
 def callback(ws_data: dict[str, MowerAttributes]):
     """Process websocket callbacks and write them to the DataUpdateCoordinator."""
     for mower_id in ws_data:
         print(ws_data[mower_id])
+        print(
+            convert_timestamp_to_datetime_utc(
+                ws_data[mower_id].planner.next_start_timestamp,
+                zoneinfo.ZoneInfo("Europe/Berlin"),
+            )
+        )
 
 
 async def _client_listen(
     automower_client: AutomowerSession,
     reconnect_time: int = 2,
 ) -> None:
     """Listen with the client."""
```

### Comparing `aioautomower-2024.3.5/aioautomower/exceptions.py` & `aioautomower-2024.4.0/aioautomower/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.3.5/aioautomower/model.py` & `aioautomower-2024.4.0/aioautomower/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 """Models for Husqvarna Automower data."""
 
 from dataclasses import dataclass, field
 from datetime import UTC, datetime
 from enum import Enum, StrEnum
 from re import sub
-import time
-import os
 
 from mashumaro import DataClassDictMixin, field_options
 
 from .const import ERRORCODES
 
-os.environ["TZ"] = "UTC"
-time.tzset()
-
 
 def snake_case(string) -> str:
     """Convert an error text to snake case"""
     return "_".join(
         sub(
             "([A-Z][a-z][,]+)",
             r" \1",
@@ -101,19 +96,26 @@
             deserialize=lambda x: (None if x == 0 else snake_case(ERRORCODES.get(x))),
             alias="errorCode",
         ),
     )
     error_datetime: datetime | None = field(
         metadata=field_options(
             deserialize=lambda x: (
-                None if x == 0 else datetime.fromtimestamp(x / 1000)
+                None
+                if x == 0
+                else datetime.fromtimestamp(x / 1000, tz=UTC).replace(
+                    tzinfo=datetime.now(UTC).astimezone().tzinfo
+                )
             ),
             alias="errorCodeTimestamp",
         ),
     )
+    error_timestamp: int | None = field(
+        metadata=field_options(alias="errorCodeTimestamp")
+    )
 
 
 @dataclass
 class Calendar(DataClassDictMixin):
     """Information about the calendar tasks.
 
     An Automower can have several tasks. If the mower supports
@@ -153,20 +155,26 @@
 @dataclass
 class Planner(DataClassDictMixin):
     """DataClass for Planner values."""
 
     next_start_datetime: datetime | None = field(
         metadata=field_options(
             deserialize=lambda x: (
-                None if x == 0 else datetime.fromtimestamp(x / 1000)
+                None
+                if x == 0
+                else datetime.fromtimestamp(x / 1000, tz=UTC).replace(
+                    tzinfo=datetime.now(UTC).astimezone().tzinfo
+                )
             ),
             alias="nextStartTimestamp",
         ),
     )
-
+    next_start_timestamp: int | None = field(
+        metadata=field_options(alias="nextStartTimestamp")
+    )
     override: Override
     restricted_reason: str = field(metadata=field_options(alias="restrictedReason"))
 
 
 @dataclass
 class Metadata(DataClassDictMixin):
     """DataClass for Metadata values."""
```

### Comparing `aioautomower-2024.3.5/aioautomower/session.py` & `aioautomower-2024.4.0/aioautomower/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import asyncio
 import contextlib
 import logging
 from typing import Literal
 from dataclasses import dataclass
 from aiohttp import WSMsgType
-
 from .auth import AbstractAuth
 from .const import EVENT_TYPES, REST_POLL_CYCLE
 from .exceptions import NoDataAvailableException, TimeoutException
 from .model import HeadlightModes, MowerAttributes
 from .utils import mower_list_to_dictionary_dataclass
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `aioautomower-2024.3.5/aioautomower/utils.py` & `aioautomower-2024.4.0/aioautomower/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Utils for Husqvarna Automower."""
 
 import logging
 import time
 from urllib.parse import quote_plus, urlencode
+import datetime
+import zoneinfo
 import aiohttp
 import jwt
-
 from .const import AUTH_API_REVOKE_URL, AUTH_API_TOKEN_URL, AUTH_HEADERS
 from .exceptions import ApiException
 from .model import JWT, MowerAttributes, MowerList, snake_case
 from .const import ERRORCODES
 
+
 _LOGGER = logging.getLogger(__name__)
 
 
 def structure_token(access_token) -> JWT:
     """Decode JWT and convert to dataclass."""
     token_decoded = jwt.decode(access_token, options={"verify_signature": False})
     return JWT.from_dict(token_decoded)
@@ -102,7 +104,20 @@
 
 def error_key_dict() -> dict[str, str]:
     """Create a dictionary with error keys and a human friendly text"""
     codes = {}
     for error_text in ERRORCODES.values():
         codes[snake_case(error_text)] = error_text
     return codes
+
+
+def convert_timestamp_to_datetime_utc(
+    timestamp: int, time_zone: zoneinfo.ZoneInfo
+) -> datetime.datetime | None:
+    """Create datetime object in the requested timezone."""
+
+    if timestamp != 0:
+        local_datetime_unshifted = datetime.datetime.fromtimestamp(
+            timestamp / 1000, tz=time_zone
+        )
+        return local_datetime_unshifted - local_datetime_unshifted.utcoffset()
+    return None
```

### Comparing `aioautomower-2024.3.5/aioautomower.egg-info/PKG-INFO` & `aioautomower-2024.4.0/aioautomower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2024.3.5
+Version: 2024.4.0
 Summary: MPython module to talk to Husqvarna Automower.
 Author-email: Thomas Protzner <thomas.protzner@gmail.com>
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/Thomas55555/aioautomower
 Project-URL: Repository, https://github.com/Thomas55555/aioautomower
 Project-URL: Issues, https://github.com/Thomas55555/aioautomower/issues
 Platform: any
```

### Comparing `aioautomower-2024.3.5/aioautomower.egg-info/SOURCES.txt` & `aioautomower-2024.4.0/aioautomower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.3.5/pyproject.toml` & `aioautomower-2024.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=62.3",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioautomower"
-version = "2024.3.5"
+version = "2024.4.0"
 description = "MPython module to talk to Husqvarna Automower."
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "Thomas Protzner", email = "thomas.protzner@gmail.com" },
 ]
 classifiers = [
@@ -52,15 +52,15 @@
 mypy = "1.9.0"
 pre-commit = "3.7.0"
 pre-commit-hooks = "4.5.0"
 pylint = "3.1.0"
 pytest = "8.1.1"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
-ruff = "0.3.4"
+ruff = "0.3.5"
 safety = "3.1.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
 freezegun = "^1.4.0"
 
 [tool.poetry.group.dev.dependencies.coverage]
@@ -87,27 +87,27 @@
     "py.typed",
 ]
 
 [tool.ruff]
 fix = true
 show-fixes = true
 
-[tool.ruff.flake8-annotations]
+[tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
 suppress-dummy-args = true
 
-[tool.ruff.flake8-builtins]
+[tool.ruff.lint.flake8-builtins]
 builtins-ignorelist = [
     "id",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
-[tool.ruff.pylint]
+[tool.ruff.lint.pylint]
 max-branches = 25
 max-returns = 15
 max-args = 10
 max-statements = 50
 
 [tool.pylint]
 ignore = [
```

### Comparing `aioautomower-2024.3.5/tests/test_error_text.py` & `aioautomower-2024.4.0/tests/test_error_text.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.3.5/tests/test_high_feature_mower_model.py` & `aioautomower-2024.4.0/tests/test_high_feature_mower_model.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.3.5/tests/test_jwt_model.py` & `aioautomower-2024.4.0/tests/test_jwt_model.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.3.5/tests/test_low_feature_mower_model.py` & `aioautomower-2024.4.0/tests/test_low_feature_mower_model.py`

 * *Files identical despite different names*

