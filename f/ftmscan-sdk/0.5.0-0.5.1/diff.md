# Comparing `tmp/ftmscan_sdk-0.5.0.tar.gz` & `tmp/ftmscan_sdk-0.5.1.tar.gz`

## Comparing `ftmscan_sdk-0.5.0.tar` & `ftmscan_sdk-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/Pipfile
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/.github/workflows/isort.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/.vscode/extensions.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/src/ftmscan_sdk/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/src/ftmscan_sdk/client/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/src/ftmscan_sdk/modules/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/src/ftmscan_sdk/modules/account/__init__.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/src/ftmscan_sdk/modules/account/account_module.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/src/ftmscan_sdk/modules/account/account_typing.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/src/ftmscan_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/src/ftmscan_sdk/utils/custom_logger.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/Pipfile
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/.github/workflows/isort.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/.vscode/extensions.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/client/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/account/__init__.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/account/account_module.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/account/account_typing.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/src/ftmscan_sdk/utils/custom_logger.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.1/PKG-INFO
```

### Comparing `ftmscan_sdk-0.5.0/src/ftmscan_sdk/client/__init__.py` & `ftmscan_sdk-0.5.1/src/ftmscan_sdk/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.0/src/ftmscan_sdk/modules/account/account_module.py` & `ftmscan_sdk-0.5.1/src/ftmscan_sdk/modules/account/account_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List
 
-from client import FTMExplorerClient
-from utils import logger as logging
+from .client import FTMExplorerClient
+from .utils import logger as logging
 
 from .account_typing import GetFtmBalanceAddressInterface
 
 
 class Account(FTMExplorerClient):
 
     async def get_ftm_balance_for_single_address(self, address: str) -> Dict:
```

### Comparing `ftmscan_sdk-0.5.0/src/ftmscan_sdk/utils/custom_logger.py` & `ftmscan_sdk-0.5.1/src/ftmscan_sdk/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.0/.gitignore` & `ftmscan_sdk-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.0/LICENSE` & `ftmscan_sdk-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.0/pyproject.toml` & `ftmscan_sdk-0.5.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-
-[project]
-name = "ftmscan-sdk"
-version = "0.5.0"
-authors = [
-  { name="Omid Shahsavarzadeh", email="omidsha@pm.me" },
-  { name="Kianoush Mahboob", email="kianoushmhaboob@gmail.com" },
-]
-description = "A sdk for interacting with ftmscan.com"
-readme = "README.md"
-requires-python = ">=3.11"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/BoysOfCannabis/ftmscan-sdk"
-Issues = "https://github.com/BoysOfCannabis/ftmscan-sdk/issues"
+Metadata-Version: 2.3
+Name: ftmscan-sdk
+Version: 0.5.1
+Summary: A sdk for interacting with ftmscan.com
+Project-URL: Homepage, https://github.com/BoysOfCannabis/ftmscan-sdk
+Project-URL: Issues, https://github.com/BoysOfCannabis/ftmscan-sdk/issues
+Author-email: Omid Shahsavarzadeh <omidsha@pm.me>, Kianoush Mahboob <kianoushmhaboob@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
+# ftmscan-sdk
+An Asynchrounos API Wrapper for python
+
+## Todo
+- [] Teransaction API support
+- [] Initiate documantation
```

