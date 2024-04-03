# Comparing `tmp/vxutils-20240401.tar.gz` & `tmp/vxutils-20240402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxutils-20240401.tar", max compression
+gzip compressed data, was "vxutils-20240402.tar", max compression
```

## Comparing `vxutils-20240401.tar` & `vxutils-20240402.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1998 2024-04-02 03:12:27.344434 vxutils-20240401/pyproject.toml
--rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240401/README.md
--rw-r--r--   0        0        0      421 2024-04-02 02:11:16.355963 vxutils-20240401/src/vxsched/__init__.py
--rw-r--r--   0        0        0     1370 2024-03-31 05:45:50.712223 vxutils-20240401/src/vxsched/__main__.py
--rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240401/src/vxsched/core.py
--rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240401/src/vxsched/event.py
--rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240401/src/vxsched/py.typed
--rw-r--r--   0        0        0     1202 2024-04-02 02:11:10.194079 vxutils-20240401/src/vxsched/subpubs.py
--rw-r--r--   0        0        0     1307 2024-03-31 05:45:44.565049 vxutils-20240401/src/vxutils/__init__.py
--rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240401/src/vxutils/context.py
--rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240401/src/vxutils/convertors.py
--rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240401/src/vxutils/datamodel/__init__.py
--rw-r--r--   0        0        0     4214 2024-02-18 02:09:20.092983 vxutils-20240401/src/vxutils/datamodel/adapter.py
--rw-r--r--   0        0        0     2369 2024-03-07 04:24:54.189680 vxutils-20240401/src/vxutils/datamodel/core.py
--rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240401/src/vxutils/datamodel/dborm.py
--rw-r--r--   0        0        0     7849 2024-04-02 03:12:05.121190 vxutils-20240401/src/vxutils/decorators.py
--rw-r--r--   0        0        0     5365 2024-03-11 02:27:17.709011 vxutils-20240401/src/vxutils/dtutils.py
--rw-r--r--   0        0        0     7344 2024-03-31 03:46:11.067709 vxutils-20240401/src/vxutils/logger.py
--rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240401/src/vxutils/networking/requests.py
--rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240401/src/vxutils/networking/wechat.py
--rw-r--r--   0        0        0     6173 2024-03-15 02:47:00.420052 vxutils-20240401/src/vxutils/provider.py
--rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240401/src/vxutils/py.typed
--rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240401/src/vxutils/typehints.py
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240401/PKG-INFO
+-rw-r--r--   0        0        0     1998 2024-04-02 06:38:01.792360 vxutils-20240402/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240402/README.md
+-rw-r--r--   0        0        0      421 2024-04-02 02:11:16.355963 vxutils-20240402/src/vxsched/__init__.py
+-rw-r--r--   0        0        0     1370 2024-03-31 05:45:50.712223 vxutils-20240402/src/vxsched/__main__.py
+-rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240402/src/vxsched/core.py
+-rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240402/src/vxsched/event.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240402/src/vxsched/py.typed
+-rw-r--r--   0        0        0     1202 2024-04-02 02:11:10.194079 vxutils-20240402/src/vxsched/subpubs.py
+-rw-r--r--   0        0        0     1300 2024-04-02 04:04:53.347572 vxutils-20240402/src/vxutils/__init__.py
+-rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240402/src/vxutils/context.py
+-rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240402/src/vxutils/convertors.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240402/src/vxutils/datamodel/__init__.py
+-rw-r--r--   0        0        0     4214 2024-02-18 02:09:20.092983 vxutils-20240402/src/vxutils/datamodel/adapter.py
+-rw-r--r--   0        0        0     2369 2024-03-07 04:24:54.189680 vxutils-20240402/src/vxutils/datamodel/core.py
+-rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240402/src/vxutils/datamodel/dborm.py
+-rw-r--r--   0        0        0     8658 2024-04-02 04:06:13.554527 vxutils-20240402/src/vxutils/decorators.py
+-rw-r--r--   0        0        0     5365 2024-03-11 02:27:17.709011 vxutils-20240402/src/vxutils/dtutils.py
+-rw-r--r--   0        0        0     7344 2024-03-31 03:46:11.067709 vxutils-20240402/src/vxutils/logger.py
+-rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240402/src/vxutils/networking/requests.py
+-rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240402/src/vxutils/networking/wechat.py
+-rw-r--r--   0        0        0     6173 2024-03-15 02:47:00.420052 vxutils-20240402/src/vxutils/provider.py
+-rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240402/src/vxutils/py.typed
+-rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240402/src/vxutils/typehints.py
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240402/PKG-INFO
```

### Comparing `vxutils-20240401/pyproject.toml` & `vxutils-20240402/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vxutils"
-version = "20240401"
+version = "20240402"
 description = "python 常用工具箱"
 license = "MIT"
 authors = ["vex1023 <vex1023@qq.com>"]
 homepage = "https://gitee.com/vxquant/vxutils"
 keywords = ["quant", "tools"]
 readme = "README.md"
```

### Comparing `vxutils-20240401/src/vxsched/__main__.py` & `vxutils-20240402/src/vxsched/__main__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxsched/core.py` & `vxutils-20240402/src/vxsched/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxsched/event.py` & `vxutils-20240402/src/vxsched/event.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxsched/subpubs.py` & `vxutils-20240402/src/vxsched/subpubs.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/__init__.py` & `vxutils-20240402/src/vxutils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 )
 from .decorators import (
     singleton,
     async_task,
     retry,
     timeit,
     timeout,
-    TimeoutError,
+    timer,
     VXAsyncResult,
 )
 from .context import VXContext
 from .provider import (
     AbstractProviderCollection,
     ProviderConfig,
     AbstractProvider,
```

### Comparing `vxutils-20240401/src/vxutils/context.py` & `vxutils-20240402/src/vxutils/context.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/convertors.py` & `vxutils-20240402/src/vxutils/convertors.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/datamodel/adapter.py` & `vxutils-20240402/src/vxutils/datamodel/adapter.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/datamodel/core.py` & `vxutils-20240402/src/vxutils/datamodel/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/datamodel/dborm.py` & `vxutils-20240402/src/vxutils/datamodel/dborm.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/decorators.py` & `vxutils-20240402/src/vxutils/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from functools import wraps
 
 __all__ = [
     "retry",
     "timeit",
     "singleton",
     "timeout",
+    "async_task",
+    "timer",
+    "VXAsyncResult",
 ]
 
 
 ###################################
 # 错误重试方法实现
 # @retry(tries, CatchExceptions=(Exception,), delay=0.01, backoff=2)
 ###################################
@@ -125,14 +128,33 @@
                         kwargs,
                         cost * 1000,
                     )
 
         return wrapper
 
 
+class timer:
+    """计时器"""
+
+    def __init__(self, descriptions: str = "", *, warnning: float = 0) -> None:
+        self._descriptions = descriptions
+        self._start = 0.0
+        self._warnning = warnning
+
+    def __enter__(self) -> None:
+        self._start = time.perf_counter()
+
+    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
+        cost = (time.perf_counter() - self._start) * 1000
+        if cost > self._warnning > 0:
+            logging.warning(f"{self._descriptions} used : {cost:.2f}ms")
+        else:
+            logging.info(f"{self._descriptions} used : {cost:.2f}ms")
+
+
 ###################################
 # Singleton 实现
 # @singleton
 ###################################
 
 
 class singleton(object):
@@ -161,16 +183,16 @@
 
 ###################################
 # 限制超时时间
 # @timeout(seconds, error_message='Function call timed out')
 ###################################
 
 
-class TimeoutError(Exception):
-    pass
+# class TimeoutError(Exception):
+#    pass
 
 
 class timeout:
 
     def __init__(
         self, seconds: float = 1, *, timeout_msg: str = "Function %s call time out."
     ) -> None:
@@ -298,7 +320,11 @@
     def test(i: int) -> int:
         print("test", i, end="\n")
         time.sleep(1)
         return i + 1
 
     results = [test(i) for i in range(10)]
     print([result for result in results])
+    with timer("test", warnning=0.5):
+        time.sleep(1)
+        with timer("test1", warnning=1):
+            time.sleep(1)
```

### Comparing `vxutils-20240401/src/vxutils/dtutils.py` & `vxutils-20240402/src/vxutils/dtutils.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/logger.py` & `vxutils-20240402/src/vxutils/logger.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/networking/requests.py` & `vxutils-20240402/src/vxutils/networking/requests.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/networking/wechat.py` & `vxutils-20240402/src/vxutils/networking/wechat.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/src/vxutils/provider.py` & `vxutils-20240402/src/vxutils/provider.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240401/PKG-INFO` & `vxutils-20240402/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxutils
-Version: 20240401
+Version: 20240402
 Summary: python 常用工具箱
 Home-page: https://gitee.com/vxquant/vxutils
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
```

