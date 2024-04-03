# Comparing `tmp/exchanges_wrapper-2.1.6.tar.gz` & `tmp/exchanges_wrapper-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges_wrapper-2.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exchanges_wrapper-2.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `exchanges_wrapper-2.1.6.tar` & `exchanges_wrapper-2.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1114 2024-03-31 10:17:24.229919 exchanges_wrapper-2.1.6/LICENSE.md
--rw-r--r--   0        0        0     7000 2024-03-31 10:17:24.229919 exchanges_wrapper-2.1.6/README.md
--rwxr-xr-x   0        0        0     1516 2024-03-31 10:17:24.229919 exchanges_wrapper-2.1.6/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    19230 2024-03-31 10:17:24.229919 exchanges_wrapper-2.1.6/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0    15978 2024-03-31 10:17:24.229919 exchanges_wrapper-2.1.6/exchanges_wrapper/bybit_parser.py
--rw-r--r--   0        0        0    78029 2024-03-31 10:17:24.229919 exchanges_wrapper-2.1.6/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2768 2024-03-31 10:17:24.229919 exchanges_wrapper-2.1.6/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2024-03-31 10:17:24.229919 exchanges_wrapper-2.1.6/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12512 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    36432 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     5597 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    13090 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    14390 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/huobi_parser.py
--rwxr-xr-x   0        0        0     2500 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/lib.py
--rw-r--r--   0        0        0    53745 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/martin/__init__.py
--rw-r--r--   0        0        0    16228 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    10683 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/proto/martin.proto
--rw-r--r--   0        0        0    27723 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0     1227 2024-03-31 10:17:24.233919 exchanges_wrapper-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     8017 1970-01-01 00:00:00.000000 exchanges_wrapper-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/LICENSE.md
+-rw-r--r--   0        0        0     7003 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/README.md
+-rwxr-xr-x   0        0        0     1516 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    19230 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0    15978 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/bybit_parser.py
+-rw-r--r--   0        0        0    78029 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2768 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12512 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    36432 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     5597 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    13216 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    14390 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/huobi_parser.py
+-rwxr-xr-x   0        0        0     2500 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/lib.py
+-rw-r--r--   0        0        0    53745 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/martin/__init__.py
+-rw-r--r--   0        0        0    16228 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    10683 2024-04-03 15:41:45.796099 exchanges_wrapper-2.1.7/exchanges_wrapper/proto/martin.proto
+-rw-r--r--   0        0        0    27723 2024-04-03 15:41:45.796099 exchanges_wrapper-2.1.7/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0     1227 2024-04-03 15:41:45.796099 exchanges_wrapper-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0     8020 1970-01-01 00:00:00.000000 exchanges_wrapper-2.1.7/PKG-INFO
```

### Comparing `exchanges_wrapper-2.1.6/LICENSE.md` & `exchanges_wrapper-2.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/README.md` & `exchanges_wrapper-2.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
  --restart=always \
  --name=exchanges-wrapper \
  exchanges-wrapper
 ```
 
 ### Documentations
 * Served methods and examples of their use are described at ```example/exch_client.py```
-* For [Protocol Buffers](https://developers.google.com/protocol-buffers/docs/overview) serializing structured data see ```proto/exchanges_wrapper/api.proto```
+* For [Protocol Buffers](https://developers.google.com/protocol-buffers/docs/overview) serializing structured data see ```exchanges_wrapper/proto/martin.proto```
 
 ## Donate
 *USDT* (TRC20) TN8F3Dz8BU8VwECRh3LTKi7FrsU8eWfsZz
 
 ## Powered by exchanges-wrapper
 <a><img align="middle" src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="50"></a>
 [martin-binance](https://github.com/DogsTailFarmer/martin-binance)
```

#### html2text {}

```diff
@@ -65,13 +65,13 @@
 python3 init.py && rm init.py && rm exch_srv_cfg.toml.template ``` #### Start
 server ```console docker run -itP \ --mount type=bind,source=/home/
 ubuntu/.MartinBinance,target=/home/appuser/.MartinBinance \ --network=host \ --
 restart=always \ --name=exchanges-wrapper \ exchanges-wrapper ``` ###
 Documentations * Served methods and examples of their use are described at
 ```example/exch_client.py``` * For [Protocol Buffers](https://
 developers.google.com/protocol-buffers/docs/overview) serializing structured
-data see ```proto/exchanges_wrapper/api.proto``` ## Donate *USDT* (TRC20)
+data see ```exchanges_wrapper/proto/martin.proto``` ## Donate *USDT* (TRC20)
 TN8F3Dz8BU8VwECRh3LTKi7FrsU8eWfsZz ## Powered by exchanges-wrapper [https://
 github.com/DogsTailFarmer/martin-binance/raw/public/doc/
 Modified%20martingale.svg][martin-binance](https://github.com/DogsTailFarmer/
 martin-binance) Free trading system for crypto exchanges SPOT markets. Adaptive
 customizable reverse grid strategy based on martingale.
```

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/__init__.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "2.1.6"
+__version__ = "2.1.7"
 
 from pathlib import Path
 import shutil
 
 from grpclib.server import Server, GRPCError, Status
 from grpclib.client import Channel
 from grpclib.utils import graceful_exit
```

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/bitfinex_parser.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/bybit_parser.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/bybit_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/client.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/definitions.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/errors.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/events.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/exch_srv.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/exch_srv.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges_wrapper-2.1.7/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/http_client.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,20 +80,22 @@
                 raise HTTPError(f"Malformed request: {payload}:{response.reason}:{response.text}")
 
         if self.exchange == 'bybit' and payload:
             if payload.get('retCode') == 0:
                 return payload.get('result'), payload.get('time')
             elif payload.get('retCode') == 10002:
                 raise ExchangeError(ERR_TIMESTAMP_OUTSIDE_RECV_WINDOW)
+            else:
+                raise ExchangeError(f"API request failed: {response.status}:{response.reason}:{payload}")
         elif self.exchange == 'huobi' and payload and (payload.get('status') == 'ok' or payload.get('ok')):
             return payload.get('data', payload.get('tick'))
         elif self.exchange == 'okx' and payload and payload.get('code') == '0':
             return payload.get('data', [])
-        elif (self.exchange not in ('binance', 'bitfinex') or
-              (self.exchange == 'binance' and payload and "code" in payload)):
+        elif self.exchange not in ('binance', 'bitfinex') \
+                or (self.exchange == 'binance' and payload and "code" in payload):
             raise ExchangeError(f"API request failed: {response.status}:{response.reason}:{payload}")
         else:
             return payload
 
     async def send_api_call(self,
                             path,
                             method="GET",
```

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/huobi_parser.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/lib.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/lib.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/martin/__init__.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/martin/__init__.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/okx_parser.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/proto/martin.proto` & `exchanges_wrapper-2.1.7/exchanges_wrapper/proto/martin.proto`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/exchanges_wrapper/web_sockets.py` & `exchanges_wrapper-2.1.7/exchanges_wrapper/web_sockets.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/pyproject.toml` & `exchanges_wrapper-2.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.6/PKG-INFO` & `exchanges_wrapper-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 2.1.6
+Version: 2.1.7
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -138,15 +138,15 @@
  --restart=always \
  --name=exchanges-wrapper \
  exchanges-wrapper
 ```
 
 ### Documentations
 * Served methods and examples of their use are described at ```example/exch_client.py```
-* For [Protocol Buffers](https://developers.google.com/protocol-buffers/docs/overview) serializing structured data see ```proto/exchanges_wrapper/api.proto```
+* For [Protocol Buffers](https://developers.google.com/protocol-buffers/docs/overview) serializing structured data see ```exchanges_wrapper/proto/martin.proto```
 
 ## Donate
 *USDT* (TRC20) TN8F3Dz8BU8VwECRh3LTKi7FrsU8eWfsZz
 
 ## Powered by exchanges-wrapper
 <a><img align="middle" src="https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/Modified%20martingale.svg" width="50"></a>
 [martin-binance](https://github.com/DogsTailFarmer/martin-binance)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 2.1.6 Summary: REST API
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 2.1.7 Summary: REST API
 and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
 email: Thomas Marchand
 tuta.io>, Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
@@ -80,13 +80,13 @@
 python3 init.py && rm init.py && rm exch_srv_cfg.toml.template ``` #### Start
 server ```console docker run -itP \ --mount type=bind,source=/home/
 ubuntu/.MartinBinance,target=/home/appuser/.MartinBinance \ --network=host \ --
 restart=always \ --name=exchanges-wrapper \ exchanges-wrapper ``` ###
 Documentations * Served methods and examples of their use are described at
 ```example/exch_client.py``` * For [Protocol Buffers](https://
 developers.google.com/protocol-buffers/docs/overview) serializing structured
-data see ```proto/exchanges_wrapper/api.proto``` ## Donate *USDT* (TRC20)
+data see ```exchanges_wrapper/proto/martin.proto``` ## Donate *USDT* (TRC20)
 TN8F3Dz8BU8VwECRh3LTKi7FrsU8eWfsZz ## Powered by exchanges-wrapper [https://
 github.com/DogsTailFarmer/martin-binance/raw/public/doc/
 Modified%20martingale.svg][martin-binance](https://github.com/DogsTailFarmer/
 martin-binance) Free trading system for crypto exchanges SPOT markets. Adaptive
 customizable reverse grid strategy based on martingale.
```

