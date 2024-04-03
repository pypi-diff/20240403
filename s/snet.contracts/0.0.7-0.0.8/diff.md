# Comparing `tmp/snet.contracts-0.0.7.tar.gz` & `tmp/snet.contracts-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snet.contracts-0.0.7.tar", last modified: Tue Mar 19 01:27:12 2024, max compression
+gzip compressed data, was "snet.contracts-0.0.8.tar", last modified: Wed Apr  3 14:07:40 2024, max compression
```

## Comparing `snet.contracts-0.0.7.tar` & `snet.contracts-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 01:27:12.740100 snet.contracts-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     1071 2024-03-19 01:27:01.000000 snet.contracts-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1418 2024-03-19 01:27:12.740100 snet.contracts-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1054 2024-03-19 01:27:01.000000 snet.contracts-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 01:27:12.740100 snet.contracts-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      911 2024-03-19 01:27:01.000000 snet.contracts-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 01:27:12.740100 snet.contracts-0.0.7/snet/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 01:27:12.740100 snet.contracts-0.0.7/snet/contracts/
--rw-r--r--   0 root         (0) root         (0)       20 2024-03-19 01:27:01.000000 snet.contracts-0.0.7/snet/contracts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-03-19 01:27:01.000000 snet.contracts-0.0.7/snet/contracts/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 01:27:12.740100 snet.contracts-0.0.7/snet.contracts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1418 2024-03-19 01:27:12.000000 snet.contracts-0.0.7/snet.contracts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2024-03-19 01:27:12.000000 snet.contracts-0.0.7/snet.contracts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 01:27:12.000000 snet.contracts-0.0.7/snet.contracts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-19 01:27:12.000000 snet.contracts-0.0.7/snet.contracts.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-19 01:27:12.000000 snet.contracts-0.0.7/snet.contracts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-19 01:27:12.000000 snet.contracts-0.0.7/snet.contracts.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.769120 snet.contracts-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 14:07:40.769120 snet.contracts-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      911 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/abi/
+-rw-r--r--   0 root         (0) root         (0)     8656 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)     5433 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/Registry.json
+-rw-r--r--   0 root         (0) root         (0)     7461 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)     4215 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)     9861 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/abi/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/bytecode/
+-rw-r--r--   0 root         (0) root         (0)    15025 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)    14575 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/Registry.json
+-rw-r--r--   0 root         (0) root         (0)    15169 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)     8967 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)    22353 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/bytecode/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/
+-rw-r--r--   0 root         (0) root         (0)    26292 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)    21210 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/Registry.json
+-rw-r--r--   0 root         (0) root         (0)    17268 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)    30657 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/AGIX/
+-rw-r--r--   0 root         (0) root         (0)    14351 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/CGV/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/NTX/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/RJV/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/snet/contracts/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:07:40.765120 snet.contracts-0.0.8/snet.contracts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-03 14:07:40.000000 snet.contracts-0.0.8/snet.contracts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-03 14:07:28.000000 snet.contracts-0.0.8/version.py
```

### Comparing `snet.contracts-0.0.7/LICENSE` & `snet.contracts-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.7/PKG-INFO` & `snet.contracts-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: snet.contracts
-Version: 0.0.7
+Version: 0.0.8
 Summary: SingularityNET Ecosystem Contracts
 Home-page: https://github.com/singnet/snet-ecosystem-contracts
 Author: SingularityNET Foundation
 Author-email: info@singularitynet.io
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: web3==6.11.1
 
 # SingularityNET Ecosystem Contracts Package
 
-The package was created to easily work with SingularityNET ecosystem EVM contracts with Python
+The package was created to easily work with SingularityNET ecosystem EVM contracts
 
-### Usage
+## Python
+### Usage 
   
 Easily get an instance of the contract you need from any SingularityNET product with just one call to one of the functions
 
 Install:
 ```bash
 pip install snet.contracts
 ```
@@ -51,7 +52,46 @@
 
 ```bash
 python -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 python3 test/unit_test.py
 ```
+
+## Golang
+
+### Install
+```bash
+go get -u github.com/singnet/snet-ecosystem-contracts
+```
+
+### Usage
+
+```go
+package main
+
+import (
+	"fmt"
+	"github.com/singnet/snet-ecosystem-contracts"
+)
+
+func main() {
+
+	// get list of all contracts
+	fmt.Println(contracts.List)
+	
+	// get ABI of contract Registry
+	fmt.Println(string(contracts.GetABI(contracts.Registry)))
+
+	// get bytecode of contract SingularityNetToken
+	fmt.Println(string(contracts.GetBytecode(contracts.SingularityNetToken)))
+
+	// get addresses, events, and more for smart contracts for different networks
+	fmt.Println(string(contracts.GetNetworks(contracts.Registry)))
+
+	// clean methods returns content without spaces and line breaks
+	fmt.Println(string(contracts.GetABIClean(contracts.SingularityNetToken)))
+	fmt.Println(string(contracts.GetBytecodeClean(contracts.Registry)))
+	fmt.Println(string(contracts.GetNetworksClean(contracts.SingularityNetToken)))
+}
+
+```
```

### Comparing `snet.contracts-0.0.7/setup.py` & `snet.contracts-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.7/snet/contracts/utils.py` & `snet.contracts-0.0.8/snet/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.7/snet.contracts.egg-info/PKG-INFO` & `snet.contracts-0.0.8/snet.contracts.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: snet.contracts
-Version: 0.0.7
+Version: 0.0.8
 Summary: SingularityNET Ecosystem Contracts
 Home-page: https://github.com/singnet/snet-ecosystem-contracts
 Author: SingularityNET Foundation
 Author-email: info@singularitynet.io
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: web3==6.11.1
 
 # SingularityNET Ecosystem Contracts Package
 
-The package was created to easily work with SingularityNET ecosystem EVM contracts with Python
+The package was created to easily work with SingularityNET ecosystem EVM contracts
 
-### Usage
+## Python
+### Usage 
   
 Easily get an instance of the contract you need from any SingularityNET product with just one call to one of the functions
 
 Install:
 ```bash
 pip install snet.contracts
 ```
@@ -51,7 +52,46 @@
 
 ```bash
 python -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 python3 test/unit_test.py
 ```
+
+## Golang
+
+### Install
+```bash
+go get -u github.com/singnet/snet-ecosystem-contracts
+```
+
+### Usage
+
+```go
+package main
+
+import (
+	"fmt"
+	"github.com/singnet/snet-ecosystem-contracts"
+)
+
+func main() {
+
+	// get list of all contracts
+	fmt.Println(contracts.List)
+	
+	// get ABI of contract Registry
+	fmt.Println(string(contracts.GetABI(contracts.Registry)))
+
+	// get bytecode of contract SingularityNetToken
+	fmt.Println(string(contracts.GetBytecode(contracts.SingularityNetToken)))
+
+	// get addresses, events, and more for smart contracts for different networks
+	fmt.Println(string(contracts.GetNetworks(contracts.Registry)))
+
+	// clean methods returns content without spaces and line breaks
+	fmt.Println(string(contracts.GetABIClean(contracts.SingularityNetToken)))
+	fmt.Println(string(contracts.GetBytecodeClean(contracts.Registry)))
+	fmt.Println(string(contracts.GetNetworksClean(contracts.SingularityNetToken)))
+}
+
+```
```

