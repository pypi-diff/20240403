# Comparing `tmp/xoadmin-1.0.0.tar.gz` & `tmp/xoadmin-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoadmin-1.0.0.tar", max compression
+gzip compressed data, was "xoadmin-1.1.0.tar", max compression
```

## Comparing `xoadmin-1.0.0.tar` & `xoadmin-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0    11336 2024-03-28 14:36:34.222496 xoadmin-1.0.0/LICENSE
--rw-r--r--   0        0        0     1904 2024-03-28 14:36:34.222496 xoadmin-1.0.0/README.md
--rw-r--r--   0        0        0      676 2024-03-28 14:36:34.222496 xoadmin-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/__init__.py
--rw-r--r--   0        0        0     4531 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/api.py
--rw-r--r--   0        0        0      389 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/error.py
--rw-r--r--   0        0        0     1245 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/host.py
--rw-r--r--   0        0        0     5114 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/manager.py
--rw-r--r--   0        0        0      812 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/storage.py
--rw-r--r--   0        0        0     2373 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/user.py
--rw-r--r--   0        0        0     1822 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/utils.py
--rw-r--r--   0        0        0     1519 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/vm.py
--rw-r--r--   0        0        0     5730 2024-03-28 14:36:34.222496 xoadmin-1.0.0/src/xoadmin/websocket.py
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 xoadmin-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-03 17:41:50.542843 xoadmin-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1904 2024-04-03 17:41:50.542843 xoadmin-1.1.0/README.md
+-rw-r--r--   0        0        0      786 2024-04-03 17:41:50.542843 xoadmin-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/__main__.py
+-rw-r--r--   0        0        0     4536 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/api.py
+-rw-r--r--   0        0        0      389 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/error.py
+-rw-r--r--   0        0        0     1249 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/host.py
+-rw-r--r--   0        0        0     5138 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/manager.py
+-rw-r--r--   0        0        0      816 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/storage.py
+-rw-r--r--   0        0        0     2381 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/user.py
+-rw-r--r--   0        0        0     1523 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/vm.py
+-rw-r--r--   0        0        0     5719 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/websocket.py
+-rw-r--r--   0        0        0        0 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/configurator/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/configurator/config.py
+-rw-r--r--   0        0        0     1287 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/configurator/configurator.py
+-rw-r--r--   0        0        0      274 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/configurator/loader.py
+-rw-r--r--   0        0        0     1822 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/utils.py
+-rw-r--r--   0        0        0     2772 1970-01-01 00:00:00.000000 xoadmin-1.1.0/PKG-INFO
```

### Comparing `xoadmin-1.0.0/LICENSE` & `xoadmin-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xoadmin-1.0.0/README.md` & `xoadmin-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xoadmin-1.0.0/src/xoadmin/api.py` & `xoadmin-1.1.0/src/xoadmin/api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Dict, Optional
 
 import httpx
 
+from xoadmin.api.websocket import XOSocket
+
 # Assuming you've set up get_logger in .utils
 from xoadmin.utils import get_logger
-from xoadmin.websocket import XOSocket
 
 logger = get_logger(__name__)
 
 
 class AuthenticationError(Exception):
     """Custom exception for authentication errors."""
```

### Comparing `xoadmin-1.0.0/src/xoadmin/host.py` & `xoadmin-1.1.0/src/xoadmin/api/host.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # src/xoadmin/host.py
 
-from xoadmin.api import XOAPI
+from xoadmin.api.api import XOAPI
 
 
 class HostManagement:
     def __init__(self, xo_api: XOAPI) -> None:
         self.xo_api = xo_api
 
     async def add_host(
```

### Comparing `xoadmin-1.0.0/src/xoadmin/manager.py` & `xoadmin-1.1.0/src/xoadmin/api/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
 from typing import Any
 
-from xoadmin.api import XOAPI
-from xoadmin.error import AuthenticationError, ServerError, XOSocketError
-from xoadmin.host import HostManagement
-from xoadmin.storage import StorageManagement
-from xoadmin.user import UserManagement
+from xoadmin.api.api import XOAPI
+from xoadmin.api.error import AuthenticationError, ServerError, XOSocketError
+from xoadmin.api.host import HostManagement
+from xoadmin.api.storage import StorageManagement
+from xoadmin.api.user import UserManagement
 from xoadmin.utils import get_logger
-from xoadmin.vm import VMManagement
+from xoadmin.api.vm import VMManagement
 
 logger = get_logger(__name__)
 
 
 class XOAManager:
     """
     A manager class for orchestrating interactions with the Xen Orchestra API,
```

### Comparing `xoadmin-1.0.0/src/xoadmin/storage.py` & `xoadmin-1.1.0/src/xoadmin/api/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List
 
-from xoadmin.api import XOAPI
+from xoadmin.api.api import XOAPI
 
 
 class StorageManagement:
     """Manage storage operations within Xen Orchestra."""
 
     def __init__(self, api: XOAPI) -> None:
         self.api = api
```

### Comparing `xoadmin-1.0.0/src/xoadmin/user.py` & `xoadmin-1.1.0/src/xoadmin/api/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List
 
-from xoadmin.api import XOAPI
-from xoadmin.error import XOSocketError
+from xoadmin.api.api import XOAPI
+from xoadmin.api.error import XOSocketError
 from xoadmin.utils import get_logger
 
 logger = get_logger(__name__)
 
 
 class UserManagement:
     """Manage user operations within Xen Orchestra."""
```

### Comparing `xoadmin-1.0.0/src/xoadmin/utils.py` & `xoadmin-1.1.0/src/xoadmin/utils.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.0.0/src/xoadmin/vm.py` & `xoadmin-1.1.0/src/xoadmin/api/vm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List
 
-from xoadmin.api import XOAPI
+from xoadmin.api.api import XOAPI
 
 
 class VMManagement:
     """Handles VM operations within Xen Orchestra."""
 
     def __init__(self, api: XOAPI) -> None:
         self.api = api
```

### Comparing `xoadmin-1.0.0/src/xoadmin/websocket.py` & `xoadmin-1.1.0/src/xoadmin/api/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import asyncio
 import json
 import ssl
+import websockets
 import uuid
 from typing import Dict
 from uuid import uuid4
 
-import websockets
 
-from xoadmin.error import AuthenticationError, ServerError, XOSocketError
+from xoadmin.api.error import AuthenticationError, ServerError, XOSocketError
 from xoadmin.utils import get_logger
 
 logger = get_logger()
 
 
 class XOSocket:
     """
```

### Comparing `xoadmin-1.0.0/PKG-INFO` & `xoadmin-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: xoadmin
-Version: 1.0.0
+Version: 1.1.0
 Summary: bindings and wrappers to manage an XOA instance
 License: Apache 2.0
 Author: dennis
 Author-email: it.admin@elnissi.co.id
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorlog (>=6.8.2,<7.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
 
 # xoadmin
 
 xoadmin is an asynchronous Python client for interacting with Xen Orchestra's REST API and WebSocket. It enables the management of VMs, users, storage, and more, through Xen Orchestra.
```

