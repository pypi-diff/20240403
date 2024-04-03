# Comparing `tmp/deribit_wrapper-0.2.1.tar.gz` & `tmp/deribit_wrapper-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deribit_wrapper-0.2.1.tar", last modified: Tue Apr  2 16:16:58 2024, max compression
+gzip compressed data, was "deribit_wrapper-0.2.3.tar", last modified: Wed Apr  3 17:30:01 2024, max compression
```

## Comparing `deribit_wrapper-0.2.1.tar` & `deribit_wrapper-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:16:58.254553 deribit_wrapper-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-02 16:16:58.254553 deribit_wrapper-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:16:58.250553 deribit_wrapper-0.2.1/deribit_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/market_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/deribit_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:16:58.254553 deribit_wrapper-0.2.1/deribit_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-02 16:16:58.000000 deribit_wrapper-0.2.1/deribit_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-02 16:16:58.000000 deribit_wrapper-0.2.1/deribit_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:16:58.000000 deribit_wrapper-0.2.1/deribit_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 16:16:58.000000 deribit_wrapper-0.2.1/deribit_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 16:16:58.000000 deribit_wrapper-0.2.1/deribit_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:16:58.254553 deribit_wrapper-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-02 16:16:43.000000 deribit_wrapper-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:01.265299 deribit_wrapper-0.2.3/deribit_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/tests/test_base.py
```

### Comparing `deribit_wrapper-0.2.1/LICENSE` & `deribit_wrapper-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.1/PKG-INFO` & `deribit_wrapper-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit_wrapper
-Version: 0.2.1
+Version: 0.2.3
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.2.1/README.md` & `deribit_wrapper-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.1/deribit_wrapper/account_management.py` & `deribit_wrapper-0.2.3/deribit_wrapper/account_management.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.1/deribit_wrapper/base.py` & `deribit_wrapper-0.2.3/deribit_wrapper/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,26 @@
 
 class DeribitBase(object):
     __ENVS = {
         'test': 'https://test.deribit.com',
         'prod': 'https://www.deribit.com'
     }
     __API_URL = '/api/v2'
+    _instance_count = 0  # Class variable to keep track of the instance number
 
-    def __init__(self, env: str = 'prod'):
+    def __init__(self, env: str = 'prod', instance_name: str = None):
         super().__init__()
         if env not in self.__ENVS:
             raise ValueError(f'Environment \'{env}\' not supported. Supported environments: {self.__ENVS.keys()}')
         self._env = env
+        if instance_name is None:
+            DeribitBase._instance_count += 1
+            self.instance_name = f"Instance_{DeribitBase._instance_count}"
+        else:
+            self.instance_name = instance_name
 
     @property
     def env(self):
         return self._env
 
     @env.setter
     def env(self, value):
```

### Comparing `deribit_wrapper-0.2.1/deribit_wrapper/core.py` & `deribit_wrapper-0.2.3/deribit_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.1/deribit_wrapper/market_data.py` & `deribit_wrapper-0.2.3/deribit_wrapper/market_data.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.1/deribit_wrapper/trading.py` & `deribit_wrapper-0.2.3/deribit_wrapper/trading.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,26 +60,27 @@
             results.append(self._request(uri, params))
         ret = pd.DataFrame(results)
         return ret
 
     def add_order_data(self, trades: pd.DataFrame) -> pd.DataFrame:
         order_ids = list(set(trades['order_id']))
         orders = self.get_orders(order_ids)
-        trades = trades.merge(orders, how='left', on='order_id', suffixes=(None, '_duplicate'))
+        trades = trades.merge(orders, how='left', on='order_id', suffixes=(None, '_duplicate_from_orders_data'))
         return trades
 
     def get_trade_history(self, start: str | datetime = None, end: str | datetime = None,
                           currency: str | list[str] = None, include_order_data: bool = False) -> pd.DataFrame:
         start = start or DEFAULT_START
         end = end or DEFAULT_END
         results = self.get_transaction_log(start, end, currency, query='trade')
         if not results.empty:
             if include_order_data:
                 results = self.add_order_data(results)
         results.sort_values('timestamp', inplace=True)
+        results['id'] = results['id'].astype(int, errors='ignore')
         return results
 
     def get_entire_trade_history(self, include_order_data: bool = False) -> pd.DataFrame:
         return self.get_trade_history(include_order_data=include_order_data)
 
     def _error_handler(self, ret: dict, uri: str, params: dict, exclude_codes: list[int] = None) -> dict:
         exclude_codes = exclude_codes or []
@@ -110,15 +111,15 @@
                 print('Settlement in progress. Waiting 1 second...')
                 time.sleep(1)
                 ret = self._order_with_error_handling(uri, params, exclude_codes=[10041])
                 code = ret.get('code')
                 if code != 10041:
                     break
 
-        else:
+        elif code not in exclude_codes:
             print(f'Error code {code} not handled yet.')
 
         return ret
 
     def _order_with_error_handling(self, uri: str, params: dict, handle_error: bool = True,
                                    exclude_codes: list[int] = None) -> dict:
         ret = self._request(uri, params)
```

### Comparing `deribit_wrapper-0.2.1/deribit_wrapper.egg-info/PKG-INFO` & `deribit_wrapper-0.2.3/deribit_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit-wrapper
-Version: 0.2.1
+Version: 0.2.3
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.2.1/setup.py` & `deribit_wrapper-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='deribit_wrapper',
-    version='0.2.1',
+    version='0.2.3',
     packages=find_packages(),
     description='A Python wrapper for seamless integration with Deribit\'s trading API, offering easy access to '
                 'market data, account management, and trading operations.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
```

