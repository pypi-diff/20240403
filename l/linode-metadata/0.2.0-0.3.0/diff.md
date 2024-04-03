# Comparing `tmp/linode_metadata-0.2.0.tar.gz` & `tmp/linode_metadata-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linode_metadata-0.2.0.tar", last modified: Tue Jan 23 16:31:40 2024, max compression
+gzip compressed data, was "linode_metadata-0.3.0.tar", last modified: Wed Apr  3 16:27:20 2024, max compression
```

## Comparing `linode_metadata-0.2.0.tar` & `linode_metadata-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:31:40.565384 linode_metadata-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-23 16:31:40.565384 linode_metadata-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:31:40.561384 linode_metadata-0.2.0/linode_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/metadata_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:31:40.561384 linode_metadata-0.2.0/linode_metadata/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/objects/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/objects/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/objects/networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/objects/response_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/objects/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/linode_metadata/objects/token.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-23 16:31:33.000000 linode_metadata-0.2.0/linode_metadata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:31:40.561384 linode_metadata-0.2.0/linode_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-23 16:31:40.000000 linode_metadata-0.2.0/linode_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-23 16:31:40.000000 linode_metadata-0.2.0/linode_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 16:31:40.000000 linode_metadata-0.2.0/linode_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-23 16:31:40.000000 linode_metadata-0.2.0/linode_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-23 16:31:40.000000 linode_metadata-0.2.0/linode_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 16:31:40.565384 linode_metadata-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-23 16:31:32.000000 linode_metadata-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:20.698784 linode_metadata-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-03 16:27:20.698784 linode_metadata-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:20.694784 linode_metadata-0.3.0/linode_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/metadata_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:20.694784 linode_metadata-0.3.0/linode_metadata/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/objects/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/objects/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/objects/networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/objects/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/objects/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/objects/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 16:27:14.000000 linode_metadata-0.3.0/linode_metadata/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18475 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/linode_metadata/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:20.694784 linode_metadata-0.3.0/linode_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-03 16:27:20.000000 linode_metadata-0.3.0/linode_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-03 16:27:20.000000 linode_metadata-0.3.0/linode_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:27:20.000000 linode_metadata-0.3.0/linode_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 16:27:20.000000 linode_metadata-0.3.0/linode_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 16:27:20.000000 linode_metadata-0.3.0/linode_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:27:20.698784 linode_metadata-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 16:27:13.000000 linode_metadata-0.3.0/setup.py
```

### Comparing `linode_metadata-0.2.0/LICENSE` & `linode_metadata-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linode_metadata-0.2.0/PKG-INFO` & `linode_metadata-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,128 @@
-Metadata-Version: 2.1
-Name: linode_metadata
-Version: 0.2.0
-Summary: A client to interact with the Linode Metadata service in Python.
-Author-email: Linode <developers@linode.com>
-License: BSD-3-Clause
-Project-URL: homepage, https://github.com/linode/py-metadata
-Project-URL: repository, https://github.com/linode/py-metadata.git
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: autoflake; extra == "dev"
-Requires-Dist: Sphinx>=7.2.6; extra == "dev"
-
 # Linode Metadata Client for Python
 
+[![Unit Tests](https://github.com/linode/py-metadata/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/linode/py-metadata/actions/workflows/unit-tests.yml)
+[![E2E Tests](https://github.com/linode/py-metadata/actions/workflows/e2e-suite.yml/badge.svg?branch=main)](https://github.com/linode/py-metadata/actions/workflows/e2e-suite.yml)
+[![PyPI version](https://badge.fury.io/py/linode-metadata.svg)](https://badge.fury.io/py/linode-metadata)
+[![Documentation Status](https://readthedocs.org/projects/linode-metadata/badge/?version=latest)](https://linode-metadata.readthedocs.io/en/latest/?badge=latest)
+
 This package allows Python projects to easily interact with the [Linode Metadata Service](https://www.linode.com/docs/products/compute/compute-instances/guides/metadata/?tabs=linode-api).
 
 ## Getting Started
 
-### Prerequisites 
+### Prerequisites
 
 - Python >= 3.8
 - A running [Linode Instance](https://www.linode.com/docs/api/linode-instances/)
 
 ### Installation
 
 ```bash
 pip install linode_metadata
 ```
 
 ### Building from Source
+
 To build and install this package:
 
 - Clone this repository
 - `make install`
 
-### Basic Example
+## Examples
 
-The following sample shows a simple Python project that initializes a new metadata client and retrieves various information
-about the current Linode.
+The following code snippets show multiple different ways to use the metadata
+client and retrieves various metadata of the current Linode.
 
+### Basic Usage
 
 ```python
 from linode_metadata import MetadataClient
 
 client = MetadataClient()
 
-# All of these responses are handled as DataClasses,
-# allowing IDEs to properly use completions.
 instance_info = client.get_instance()
 network_info = client.get_network()
 ssh_info = client.get_ssh_keys()
 user_data = client.get_user_data()
 
 print("Instance ID:", instance_info.id)
 print("Public IPv4:", network_info.ipv4.public[0])
 print("SSH Keys:", "; ".join(ssh_info.users.root))
 print("User Data:", user_data)
 ```
 
+### Asynchronous I/O and Context Manager Support
+
+You can also use the context manager to ensure the HTTP client will be properly closed, and the
+`asyncio` enabled client is also available.
+
+```python
+import asyncio
+from linode_metadata import AsyncMetadataClient
+
+async def get_metadata():
+    with AsyncMetadataClient() as client:
+        instance_info = await client.get_instance()
+        print("Instance ID:", instance_info.id)
+
+asyncio.run(get_metadata())
+```
+
+### Watchers
+
+Watchers are useful for monitor changes in the metadata, e.g. newly added IP address to the Linode.
+
+```python
+import asyncio
+from linode_metadata import AsyncMetadataClient
+
+async def get_metadata():
+    async with AsyncMetadataClient() as client:
+        watcher = client.get_watcher()
+        async for new_network_info in watcher.watch_network():
+            print(new_network_info)
+
+asyncio.run(get_metadata())
+```
+
 ## Testing
 
-Before running tests on this project, please ensure you have a 
+Before running tests on this project, please ensure you have a
 [Linode Personal Access Token](https://www.linode.com/docs/products/tools/api/guides/manage-api-tokens/)
 exported under the `LINODE_TOKEN` environment variable.
 
 ### End-to-End Testing Using Ansible
 
-This project contains an Ansible playbook to automatically deploy the necessary infrastructure 
+This project contains an Ansible playbook to automatically deploy the necessary infrastructure
 and run end-to-end tests on it.
 
 To install the dependencies for this playbook, ensure you have Python 3 installed and run the following:
 
 ```bash
 make test-deps
 ```
 
 After all dependencies have been installed, you can run the end-to-end test suite by running the following:
 
 ```bash
-make e2e
+make int-test
 ```
 
-If your local SSH public key is stored in a location other than `~/.ssh/id_rsa.pub`, 
+If your local SSH public key is stored in a location other than `~/.ssh/id_rsa.pub`,
 you may need to override the `TEST_PUBKEY` argument:
 
 ```bash
-make TEST_PUBKEY=/path/to/my/pubkey e2e
+make TEST_PUBKEY=/path/to/my/pubkey int-test
 ```
 
-**NOTE: To speed up subsequent test runs, the infrastructure provisioned for testing will persist after the test run is complete. 
+**NOTE: To speed up subsequent test runs, the infrastructure provisioned for testing will persist after the test run is complete.
 This infrastructure is safe to manually remove.**
 
 ### Manual End-to-End Testing
 
-End-to-end tests can also be manually run using the `make e2e-local` target.
+End-to-end tests can also be manually run using the `make int-test-local` target.
 This test suite is expected to run from within a Linode instance and will likely 
 fail in other environments.
 
 ## License
 
 This software is Copyright Akamai Technologies, Inc. and is released under the [Apache 2.0 license](./LICENSE).
```

### Comparing `linode_metadata-0.2.0/linode_metadata/objects/error.py` & `linode_metadata-0.3.0/linode_metadata/objects/error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 """
 Data classes related to error handling.
 """
+
 from builtins import super
+from typing import Optional
 
 
 class ApiError(RuntimeError):
     """
     An API Error is any error returned from the API.  These
     typically have a status code in the 400s or 500s.  Most
     often, this will be caused by invalid input to the API.
     """
 
-    def __init__(self, message, status=400, json=None):
+    def __init__(
+        self, message: str, status: int = 400, json: Optional[dict] = None
+    ):
         super().__init__(message)
         self.status = status
         self.json = json
         self.errors = []
         if json and "errors" in json and isinstance(json["errors"], list):
             self.errors = [e["reason"] for e in json["errors"]]
+
+
+class ApiTimeoutError(RuntimeError):
+    """A Linode Metadata API call timeout error"""
+
+    def __init__(self, message: str):
+        super().__init__(message)
```

### Comparing `linode_metadata-0.2.0/linode_metadata/objects/instance.py` & `linode_metadata-0.3.0/linode_metadata/objects/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Data classes related to Linode instances.
 """
+
 from dataclasses import dataclass
 from typing import List, Optional
 
 from .response_base import ResponseBase
 
 
 @dataclass(init=False)
```

### Comparing `linode_metadata-0.2.0/linode_metadata/objects/networking.py` & `linode_metadata-0.3.0/linode_metadata/objects/networking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Data classes related to Networking.
 """
+
 from dataclasses import dataclass, field
 from typing import List, Optional
 
 from .response_base import ResponseBase
 
 
 @dataclass(init=False)
```

### Comparing `linode_metadata-0.2.0/linode_metadata/objects/response_base.py` & `linode_metadata-0.3.0/linode_metadata/objects/response_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 This class is the base class for response classes.
 It includes basic methods for handling JSON responses.
 """
+
 import dataclasses
 from dataclasses import dataclass
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 
 @dataclass(init=False)
 class ResponseBase:
     """
     The base class for responses from the Linode Metadata Service.
     :param json_data: The JSON data that will be used to build an instance of a response class.
     :type json_data: Dict[str, Any]
     """
 
-    def __init__(self, json_data: Dict[str, Any] = None):
+    def __init__(self, json_data: Optional[Dict[str, Any]] = None):
         if json_data is not None:
             self.populate(json_data)
 
     def populate(self, json_data):
         """
         Populates the fields in a response dataclass using the passed JSON data.
         """
```

### Comparing `linode_metadata-0.2.0/linode_metadata.egg-info/PKG-INFO` & `linode_metadata-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linode_metadata
-Version: 0.2.0
+Version: 0.3.0
 Summary: A client to interact with the Linode Metadata service in Python.
 Author-email: Linode <developers@linode.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/linode/py-metadata
 Project-URL: repository, https://github.com/linode/py-metadata.git
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,105 +16,148 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
+Requires-Dist: httpx
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: autoflake; extra == "dev"
 Requires-Dist: Sphinx>=7.2.6; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: sphinx-lint; extra == "dev"
+Provides-Extra: doc
+Requires-Dist: Sphinx>=7.2.6; extra == "doc"
 
 # Linode Metadata Client for Python
 
+[![Unit Tests](https://github.com/linode/py-metadata/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/linode/py-metadata/actions/workflows/unit-tests.yml)
+[![E2E Tests](https://github.com/linode/py-metadata/actions/workflows/e2e-suite.yml/badge.svg?branch=main)](https://github.com/linode/py-metadata/actions/workflows/e2e-suite.yml)
+[![PyPI version](https://badge.fury.io/py/linode-metadata.svg)](https://badge.fury.io/py/linode-metadata)
+[![Documentation Status](https://readthedocs.org/projects/linode-metadata/badge/?version=latest)](https://linode-metadata.readthedocs.io/en/latest/?badge=latest)
+
 This package allows Python projects to easily interact with the [Linode Metadata Service](https://www.linode.com/docs/products/compute/compute-instances/guides/metadata/?tabs=linode-api).
 
 ## Getting Started
 
-### Prerequisites 
+### Prerequisites
 
 - Python >= 3.8
 - A running [Linode Instance](https://www.linode.com/docs/api/linode-instances/)
 
 ### Installation
 
 ```bash
 pip install linode_metadata
 ```
 
 ### Building from Source
+
 To build and install this package:
 
 - Clone this repository
 - `make install`
 
-### Basic Example
+## Examples
 
-The following sample shows a simple Python project that initializes a new metadata client and retrieves various information
-about the current Linode.
+The following code snippets show multiple different ways to use the metadata
+client and retrieves various metadata of the current Linode.
 
+### Basic Usage
 
 ```python
 from linode_metadata import MetadataClient
 
 client = MetadataClient()
 
-# All of these responses are handled as DataClasses,
-# allowing IDEs to properly use completions.
 instance_info = client.get_instance()
 network_info = client.get_network()
 ssh_info = client.get_ssh_keys()
 user_data = client.get_user_data()
 
 print("Instance ID:", instance_info.id)
 print("Public IPv4:", network_info.ipv4.public[0])
 print("SSH Keys:", "; ".join(ssh_info.users.root))
 print("User Data:", user_data)
 ```
 
+### Asynchronous I/O and Context Manager Support
+
+You can also use the context manager to ensure the HTTP client will be properly closed, and the
+`asyncio` enabled client is also available.
+
+```python
+import asyncio
+from linode_metadata import AsyncMetadataClient
+
+async def get_metadata():
+    with AsyncMetadataClient() as client:
+        instance_info = await client.get_instance()
+        print("Instance ID:", instance_info.id)
+
+asyncio.run(get_metadata())
+```
+
+### Watchers
+
+Watchers are useful for monitor changes in the metadata, e.g. newly added IP address to the Linode.
+
+```python
+import asyncio
+from linode_metadata import AsyncMetadataClient
+
+async def get_metadata():
+    async with AsyncMetadataClient() as client:
+        watcher = client.get_watcher()
+        async for new_network_info in watcher.watch_network():
+            print(new_network_info)
+
+asyncio.run(get_metadata())
+```
+
 ## Testing
 
-Before running tests on this project, please ensure you have a 
+Before running tests on this project, please ensure you have a
 [Linode Personal Access Token](https://www.linode.com/docs/products/tools/api/guides/manage-api-tokens/)
 exported under the `LINODE_TOKEN` environment variable.
 
 ### End-to-End Testing Using Ansible
 
-This project contains an Ansible playbook to automatically deploy the necessary infrastructure 
+This project contains an Ansible playbook to automatically deploy the necessary infrastructure
 and run end-to-end tests on it.
 
 To install the dependencies for this playbook, ensure you have Python 3 installed and run the following:
 
 ```bash
 make test-deps
 ```
 
 After all dependencies have been installed, you can run the end-to-end test suite by running the following:
 
 ```bash
-make e2e
+make int-test
 ```
 
-If your local SSH public key is stored in a location other than `~/.ssh/id_rsa.pub`, 
+If your local SSH public key is stored in a location other than `~/.ssh/id_rsa.pub`,
 you may need to override the `TEST_PUBKEY` argument:
 
 ```bash
-make TEST_PUBKEY=/path/to/my/pubkey e2e
+make TEST_PUBKEY=/path/to/my/pubkey int-test
 ```
 
-**NOTE: To speed up subsequent test runs, the infrastructure provisioned for testing will persist after the test run is complete. 
+**NOTE: To speed up subsequent test runs, the infrastructure provisioned for testing will persist after the test run is complete.
 This infrastructure is safe to manually remove.**
 
 ### Manual End-to-End Testing
 
-End-to-end tests can also be manually run using the `make e2e-local` target.
+End-to-end tests can also be manually run using the `make int-test-local` target.
 This test suite is expected to run from within a Linode instance and will likely 
 fail in other environments.
 
 ## License
 
 This software is Copyright Akamai Technologies, Inc. and is released under the [Apache 2.0 license](./LICENSE).
```

### Comparing `linode_metadata-0.2.0/linode_metadata.egg-info/SOURCES.txt` & `linode_metadata-0.3.0/linode_metadata.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 linode_metadata/__init__.py
+linode_metadata/constants.py
 linode_metadata/metadata_client.py
 linode_metadata/version.py
+linode_metadata/watcher.py
 linode_metadata.egg-info/PKG-INFO
 linode_metadata.egg-info/SOURCES.txt
 linode_metadata.egg-info/dependency_links.txt
 linode_metadata.egg-info/requires.txt
 linode_metadata.egg-info/top_level.txt
 linode_metadata/objects/__init__.py
 linode_metadata/objects/error.py
```

### Comparing `linode_metadata-0.2.0/pyproject.toml` & `linode_metadata-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,30 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-dependencies = ["requests"]
+dependencies = ["httpx"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["pytest", "black", "isort", "pylint", "autoflake", "Sphinx>=7.2.6"]
+dev = [
+    "pytest",
+    "black",
+    "isort",
+    "pylint",
+    "autoflake",
+    "Sphinx>=7.2.6",
+    "pytest-asyncio",
+    "sphinx-lint",
+]
+
+doc = ["Sphinx>=7.2.6"]
 
 [project.urls]
 homepage = "https://github.com/linode/py-metadata"
 repository = "https://github.com/linode/py-metadata.git"
 
 [tool.setuptools.dynamic]
 version = { attr = "linode_metadata.version.__version__" }
```

