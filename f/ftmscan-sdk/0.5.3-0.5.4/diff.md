# Comparing `tmp/ftmscan_sdk-0.5.3.tar.gz` & `tmp/ftmscan_sdk-0.5.4.tar.gz`

## Comparing `ftmscan_sdk-0.5.3.tar` & `ftmscan_sdk-0.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/Pipfile
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/.github/workflows/isort.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/.vscode/extensions.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/client/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/account/__init__.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/account/account_module.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/account/account_typing.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/utils/custom_logger.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/Pipfile
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/.github/workflows/isort.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/.vscode/extensions.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/src/ftmscan_sdk/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/src/ftmscan_sdk/client/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/src/ftmscan_sdk/modules/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/src/ftmscan_sdk/modules/account/__init__.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/src/ftmscan_sdk/modules/account/account_module.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/src/ftmscan_sdk/modules/account/account_typing.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/src/ftmscan_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/src/ftmscan_sdk/utils/custom_logger.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.4/PKG-INFO
```

### Comparing `ftmscan_sdk-0.5.3/src/ftmscan_sdk/client/__init__.py` & `ftmscan_sdk-0.5.4/src/ftmscan_sdk/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/account/account_module.py` & `ftmscan_sdk-0.5.4/src/ftmscan_sdk/modules/account/account_module.py`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.3/.gitignore` & `ftmscan_sdk-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.3/LICENSE` & `ftmscan_sdk-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.3/pyproject.toml` & `ftmscan_sdk-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "ftmscan-sdk"
-version = "0.5.3"
+version = "0.5.4"
 authors = [
   { name="Omid Shahsavarzadeh", email="omidsha@pm.me" },
   { name="Kianoush Mahboob", email="kianoushmhaboob@gmail.com" },
 ]
 description = "A sdk for interacting with ftmscan.com"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `ftmscan_sdk-0.5.3/PKG-INFO` & `ftmscan_sdk-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ftmscan-sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: A sdk for interacting with ftmscan.com
 Project-URL: Homepage, https://github.com/BoysOfCannabis/ftmscan-sdk
 Project-URL: Issues, https://github.com/BoysOfCannabis/ftmscan-sdk/issues
 Project-URL: Repository, https://github.com/BoysOfCannabis/ftmscan-sdk.git
 Author-email: Omid Shahsavarzadeh <omidsha@pm.me>, Kianoush Mahboob <kianoushmhaboob@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```
