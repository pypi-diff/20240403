# Comparing `tmp/ftmscan_sdk-0.5.2.tar.gz` & `tmp/ftmscan_sdk-0.5.3.tar.gz`

## Comparing `ftmscan_sdk-0.5.2.tar` & `ftmscan_sdk-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/Pipfile
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/.github/workflows/isort.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/.vscode/extensions.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/client/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/account/__init__.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/account/account_module.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/account/account_typing.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/src/ftmscan_sdk/utils/custom_logger.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/Pipfile
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/.github/workflows/isort.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/.vscode/extensions.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/client/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/account/__init__.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/account/account_module.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/account/account_typing.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/src/ftmscan_sdk/utils/custom_logger.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 ftmscan_sdk-0.5.3/PKG-INFO
```

### Comparing `ftmscan_sdk-0.5.2/src/ftmscan_sdk/client/__init__.py` & `ftmscan_sdk-0.5.3/src/ftmscan_sdk/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.2/src/ftmscan_sdk/modules/account/account_module.py` & `ftmscan_sdk-0.5.3/src/ftmscan_sdk/modules/account/account_module.py`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.2/.gitignore` & `ftmscan_sdk-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.2/LICENSE` & `ftmscan_sdk-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmscan_sdk-0.5.2/pyproject.toml` & `ftmscan_sdk-0.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "ftmscan-sdk"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Omid Shahsavarzadeh", email="omidsha@pm.me" },
   { name="Kianoush Mahboob", email="kianoushmhaboob@gmail.com" },
 ]
 description = "A sdk for interacting with ftmscan.com"
 readme = "README.md"
 requires-python = ">=3.11"
@@ -17,8 +17,9 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/BoysOfCannabis/ftmscan-sdk"
-Issues = "https://github.com/BoysOfCannabis/ftmscan-sdk/issues"
+Issues = "https://github.com/BoysOfCannabis/ftmscan-sdk/issues"
+Repository  = "https://github.com/BoysOfCannabis/ftmscan-sdk.git"
```

