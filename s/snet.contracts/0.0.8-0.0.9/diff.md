# Comparing `tmp/snet.contracts-0.0.8.tar.gz` & `tmp/snet.contracts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snet.contracts-0.0.8.tar", last modified: Wed Apr  3 14:07:40 2024, max compression
+gzip compressed data, was "snet.contracts-0.0.9.tar", last modified: Wed Apr  3 15:26:43 2024, max compression
```

## Comparing `snet.contracts-0.0.8.tar` & `snet.contracts-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.769120 snet.contracts-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2339 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1975 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 14:07:40.769120 snet.contracts-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      911 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/abi/
--rw-r--r--   0 root         (0) root         (0)     8656 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/MultiPartyEscrow.json
--rw-r--r--   0 root         (0) root         (0)     5433 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/Registry.json
--rw-r--r--   0 root         (0) root         (0)     7461 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/SingularityNetToken.json
--rw-r--r--   0 root         (0) root         (0)     4215 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/TokenConversionManager.json
--rw-r--r--   0 root         (0) root         (0)     9861 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/TokenStake.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/bytecode/
--rw-r--r--   0 root         (0) root         (0)    15025 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/MultiPartyEscrow.json
--rw-r--r--   0 root         (0) root         (0)    14575 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/Registry.json
--rw-r--r--   0 root         (0) root         (0)    15169 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/SingularityNetToken.json
--rw-r--r--   0 root         (0) root         (0)     8967 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/TokenConversionManager.json
--rw-r--r--   0 root         (0) root         (0)    22353 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/TokenStake.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/
--rw-r--r--   0 root         (0) root         (0)    26292 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/MultiPartyEscrow.json
--rw-r--r--   0 root         (0) root         (0)    21210 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/Registry.json
--rw-r--r--   0 root         (0) root         (0)    17268 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/SingularityNetToken.json
--rw-r--r--   0 root         (0) root         (0)    30657 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/TokenStake.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/AGIX/
--rw-r--r--   0 root         (0) root         (0)    14351 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/CGV/
--rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/NTX/
--rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/RJV/
--rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json
--rw-r--r--   0 root         (0) root         (0)     1525 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet.contracts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2339 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1396 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      911 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.679327 snet.contracts-0.0.9/snet/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.679327 snet.contracts-0.0.9/snet/contracts/
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.679327 snet.contracts-0.0.9/snet/contracts/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/abi/
+-rw-r--r--   0 root         (0) root         (0)     8656 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)     5433 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/Registry.json
+-rw-r--r--   0 root         (0) root         (0)     7461 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)     4215 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)     9861 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/bytecode/
+-rw-r--r--   0 root         (0) root         (0)    15025 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)    14575 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/Registry.json
+-rw-r--r--   0 root         (0) root         (0)    15169 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)     8967 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)    22353 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/
+-rw-r--r--   0 root         (0) root         (0)    26292 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)    21210 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/Registry.json
+-rw-r--r--   0 root         (0) root         (0)    17268 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)    30657 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.679327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/AGIX/
+-rw-r--r--   0 root         (0) root         (0)    14351 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/CGV/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/NTX/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/RJV/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet.contracts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/version.py
```

### Comparing `snet.contracts-0.0.8/LICENSE` & `snet.contracts-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/PKG-INFO` & `snet.contracts-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snet.contracts
-Version: 0.0.8
+Version: 0.0.9
 Summary: SingularityNET Ecosystem Contracts
 Home-page: https://github.com/singnet/snet-ecosystem-contracts
 Author: SingularityNET Foundation
 Author-email: info@singularitynet.io
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `snet.contracts-0.0.8/README.md` & `snet.contracts-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/setup.py` & `snet.contracts-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/abi/MultiPartyEscrow.json` & `snet.contracts-0.0.9/snet/contracts/resources/abi/MultiPartyEscrow.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/abi/Registry.json` & `snet.contracts-0.0.9/snet/contracts/resources/abi/Registry.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/abi/SingularityNetToken.json` & `snet.contracts-0.0.9/snet/contracts/resources/abi/SingularityNetToken.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/abi/TokenConversionManager.json` & `snet.contracts-0.0.9/snet/contracts/resources/abi/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/abi/TokenStake.json` & `snet.contracts-0.0.9/snet/contracts/resources/abi/TokenStake.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/bytecode/MultiPartyEscrow.json` & `snet.contracts-0.0.9/snet/contracts/resources/bytecode/MultiPartyEscrow.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/bytecode/Registry.json` & `snet.contracts-0.0.9/snet/contracts/resources/bytecode/Registry.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/bytecode/SingularityNetToken.json` & `snet.contracts-0.0.9/snet/contracts/resources/bytecode/SingularityNetToken.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/bytecode/TokenConversionManager.json` & `snet.contracts-0.0.9/snet/contracts/resources/bytecode/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/bytecode/TokenStake.json` & `snet.contracts-0.0.9/snet/contracts/resources/bytecode/TokenStake.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/networks/MultiPartyEscrow.json` & `snet.contracts-0.0.9/snet/contracts/resources/networks/MultiPartyEscrow.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/networks/Registry.json` & `snet.contracts-0.0.9/snet/contracts/resources/networks/Registry.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/networks/SingularityNetToken.json` & `snet.contracts-0.0.9/snet/contracts/resources/networks/SingularityNetToken.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/networks/TokenStake.json` & `snet.contracts-0.0.9/snet/contracts/resources/networks/TokenStake.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json` & `snet.contracts-0.0.9/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json` & `snet.contracts-0.0.9/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json` & `snet.contracts-0.0.9/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json` & `snet.contracts-0.0.9/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet/contracts/utils.py` & `snet.contracts-0.0.9/snet/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.8/snet.contracts.egg-info/PKG-INFO` & `snet.contracts-0.0.9/snet.contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snet.contracts
-Version: 0.0.8
+Version: 0.0.9
 Summary: SingularityNET Ecosystem Contracts
 Home-page: https://github.com/singnet/snet-ecosystem-contracts
 Author: SingularityNET Foundation
 Author-email: info@singularitynet.io
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `snet.contracts-0.0.8/snet.contracts.egg-info/SOURCES.txt` & `snet.contracts-0.0.9/snet.contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

