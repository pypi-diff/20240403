# Comparing `tmp/ftmscan_sdk-0.5.1.tar.gz` & `tmp/ftmscan_sdk-0.5.2.tar.gz`

## Comparing `ftmscan_sdk-0.5.1.tar` & `ftmscan_sdk-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/Pipfile
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/.github/workflows/isort.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/.vscode/extensions.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/client/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/account/__init__.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/account/account_module.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/account/account_typing.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/utils/custom_logger.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/Pipfile
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/.github/workflows/isort.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/.vscode/extensions.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/client/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/account/__init__.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/account/account_module.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/account/account_typing.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/utils/custom_logger.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/PKG-INFO
```

### Comparing `ftmscan_sdk-0.5.1/src/ftmscan_sdk/client/__init__.py` & `ftmscan_sdk-0.5.2/src/ftmscan_sdk/client/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import abc
 
 import aiohttp
 
-
 class BaseBlockExplorerClient(abc.ABC):
     def __init__(self, API_KEY, API_URL):
         self.API_KEY = API_KEY
         self.API_URL = API_URL
 
     @abc.abstractmethod
     def send_request(self, request_payload):
@@ -20,7 +19,8 @@
         super().__init__(API_KEY, API_URL)
 
     async def send_request(self, request_payload):
         request_payload["apikey"] = self.API_KEY
         async with aiohttp.ClientSession() as session:
             async with session.get(self.API_URL, params=request_payload) as response:
                 return await response.json()
+
```

### Comparing `ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/account/account_module.py` & `ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/account/account_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List
 
-from .client import FTMExplorerClient
-from .utils import logger as logging
+from ...client import FTMExplorerClient
+from ...utils import logger as logging
 
 from .account_typing import GetFtmBalanceAddressInterface
 
 
 class Account(FTMExplorerClient):
 
     async def get_ftm_balance_for_single_address(self, address: str) -> Dict:
```

### Comparing `ftmscan_sdk-0.5.1/src/ftmscan_sdk/utils/custom_logger.py` & `ftmscan_sdk-0.5.2/src/ftmscan_sdk/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.1/.gitignore` & `ftmscan_sdk-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.1/LICENSE` & `ftmscan_sdk-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.1/pyproject.toml` & `ftmscan_sdk-0.5.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "ftmscan-sdk"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Omid Shahsavarzadeh", email="omidsha@pm.me" },
   { name="Kianoush Mahboob", email="kianoushmhaboob@gmail.com" },
 ]
 description = "A sdk for interacting with ftmscan.com"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `ftmscan_sdk-0.5.1/PKG-INFO` & `ftmscan_sdk-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ftmscan-sdk
-Version: 0.5.1
+Version: 0.5.2
 Summary: A sdk for interacting with ftmscan.com
 Project-URL: Homepage, https://github.com/BoysOfCannabis/ftmscan-sdk
 Project-URL: Issues, https://github.com/BoysOfCannabis/ftmscan-sdk/issues
 Author-email: Omid Shahsavarzadeh <omidsha@pm.me>, Kianoush Mahboob <kianoushmhaboob@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

