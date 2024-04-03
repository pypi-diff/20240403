# Comparing `tmp/ledger_app_clients.ethereum-0.3.2.dev30.tar.gz` & `tmp/ledger_app_clients.ethereum-0.3.2.dev32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledger_app_clients.ethereum-0.3.2.dev30.tar", last modified: Thu Mar 28 16:34:05 2024, max compression
+gzip compressed data, was "ledger_app_clients.ethereum-0.3.2.dev32.tar", last modified: Wed Apr  3 09:05:19 2024, max compression
```

## Comparing `ledger_app_clients.ethereum-0.3.2.dev30.tar` & `ledger_app_clients.ethereum-0.3.2.dev32.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:34:05.560541 ledger_app_clients.ethereum-0.3.2.dev30/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-28 16:34:05.560541 ledger_app_clients.ethereum-0.3.2.dev30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 16:34:05.560541 ledger_app_clients.ethereum-0.3.2.dev30/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:34:05.552541 ledger_app_clients.ethereum-0.3.2.dev30/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:34:05.556541 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:34:05.556541 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-28 16:34:05.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/command_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:34:05.556541 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/eip712/
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/eip712/InputData.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/eip712/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:34:05.560541 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/keychain/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/keychain/cal.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/keychain/domain_name.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/keychain/nft.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/keychain/set_plugin.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/tlv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-28 16:33:53.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:34:05.560541 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients.ethereum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-28 16:34:05.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients.ethereum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-28 16:34:05.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 16:34:05.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients.ethereum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 16:34:05.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients.ethereum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 16:34:05.000000 ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients.ethereum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:05:19.228412 ledger_app_clients.ethereum-0.3.2.dev32/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 09:05:19.228412 ledger_app_clients.ethereum-0.3.2.dev32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:05:19.228412 ledger_app_clients.ethereum-0.3.2.dev32/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:05:19.224412 ledger_app_clients.ethereum-0.3.2.dev32/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:05:19.224412 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:05:19.228412 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 09:05:19.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/command_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:05:19.228412 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/eip712/
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/eip712/InputData.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/eip712/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:05:19.228412 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/keychain/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/keychain/cal.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/keychain/domain_name.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/keychain/nft.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/keychain/set_plugin.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/tlv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-03 09:05:12.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:05:19.228412 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients.ethereum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 09:05:19.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients.ethereum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 09:05:19.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:05:19.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients.ethereum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 09:05:19.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients.ethereum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 09:05:19.000000 ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients.ethereum.egg-info/top_level.txt
```

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/CHANGELOG.md` & `ledger_app_clients.ethereum-0.3.2.dev32/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/PKG-INFO` & `ledger_app_clients.ethereum-0.3.2.dev32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger_app_clients.ethereum
-Version: 0.3.2.dev30
+Version: 0.3.2.dev32
 Summary: Ledger Ethereum Python client
 Author-email: Ledger <hello@ledger.fr>
 Project-URL: Home, https://github.com/LedgerHQ/app-ethereum
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/pyproject.toml` & `ledger_app_clients.ethereum-0.3.2.dev32/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/client.py` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/client.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/command_builder.py` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/command_builder.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/eip712/InputData.py` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/eip712/InputData.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/keychain.py` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/keychain.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/response_parser.py` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/response_parser.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/settings.py` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/settings.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/tlv.py` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/tlv.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients/ethereum/utils.py` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients/ethereum/utils.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients.ethereum.egg-info/PKG-INFO` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients.ethereum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger_app_clients.ethereum
-Version: 0.3.2.dev30
+Version: 0.3.2.dev32
 Summary: Ledger Ethereum Python client
 Author-email: Ledger <hello@ledger.fr>
 Project-URL: Home, https://github.com/LedgerHQ/app-ethereum
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ledger_app_clients.ethereum-0.3.2.dev30/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt` & `ledger_app_clients.ethereum-0.3.2.dev32/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

