# Comparing `tmp/didabox-2.3.0.tar.gz` & `tmp/didabox-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didabox-2.3.0.tar", max compression
+gzip compressed data, was "didabox-2.4.0.tar", max compression
```

## Comparing `didabox-2.3.0.tar` & `didabox-2.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1082 2024-03-29 03:41:43.513060 didabox-2.3.0/LICENSE
--rw-r--r--   0        0        0      325 2024-03-29 06:03:03.749013 didabox-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      107 2024-03-29 03:41:43.514059 didabox-2.3.0/README.md
--rw-r--r--   0        0        0      146 2024-03-29 03:41:43.515059 didabox-2.3.0/src/didabox/__init__.py
--rw-r--r--   0        0        0      712 2024-03-29 03:41:43.516059 didabox-2.3.0/src/didabox/check.py
--rw-r--r--   0        0        0      569 2024-03-29 05:40:32.236949 didabox-2.3.0/src/didabox/info.py
--rw-r--r--   0        0        0      591 2024-03-29 03:41:43.516059 didabox-2.3.0/src/didabox/login.py
--rw-r--r--   0        0        0     1662 2024-03-29 05:54:24.199283 didabox-2.3.0/src/didabox/main.py
--rw-r--r--   0        0        0     1412 2024-03-29 03:41:43.516059 didabox-2.3.0/src/didabox/request.py
--rw-r--r--   0        0        0     2022 2024-03-29 03:41:43.517060 didabox-2.3.0/src/didabox/task.py
--rw-r--r--   0        0        0     1999 2024-03-29 03:41:43.517060 didabox-2.3.0/src/didabox/utils.py
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 didabox-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-03-29 03:41:43.513060 didabox-2.4.0/LICENSE
+-rw-r--r--   0        0        0      350 2024-04-03 05:56:12.759240 didabox-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-03-29 03:41:43.514059 didabox-2.4.0/README.md
+-rw-r--r--   0        0        0      146 2024-03-29 03:41:43.515059 didabox-2.4.0/src/didabox/__init__.py
+-rw-r--r--   0        0        0      712 2024-03-29 03:41:43.516059 didabox-2.4.0/src/didabox/check.py
+-rw-r--r--   0        0        0      600 2024-04-03 05:26:21.967501 didabox-2.4.0/src/didabox/info.py
+-rw-r--r--   0        0        0      591 2024-03-29 03:41:43.516059 didabox-2.4.0/src/didabox/login.py
+-rw-r--r--   0        0        0     2136 2024-04-03 05:51:46.631101 didabox-2.4.0/src/didabox/main.py
+-rw-r--r--   0        0        0     1412 2024-03-29 03:41:43.516059 didabox-2.4.0/src/didabox/request.py
+-rw-r--r--   0        0        0     2520 2024-04-03 05:50:08.649210 didabox-2.4.0/src/didabox/task.py
+-rw-r--r--   0        0        0     1999 2024-03-29 03:41:43.517060 didabox-2.4.0/src/didabox/utils.py
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 didabox-2.4.0/PKG-INFO
```

### Comparing `didabox-2.3.0/LICENSE` & `didabox-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `didabox-2.3.0/src/didabox/check.py` & `didabox-2.4.0/src/didabox/check.py`

 * *Files identical despite different names*

### Comparing `didabox-2.3.0/src/didabox/info.py` & `didabox-2.4.0/src/didabox/info.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 
     def base_info(self) -> Response:
         """ 清单的基本信息:
         * 清单: 清单名称、清单id
         * 清单文件夹:
         * 过滤器:
         * 标签:
+        * 未完成的任务:
         * ...
         """
         response = self.req.get('https://api.dida365.com/api/v2/batch/check/0', params={})
         return response
```

### Comparing `didabox-2.3.0/src/didabox/login.py` & `didabox-2.4.0/src/didabox/login.py`

 * *Files identical despite different names*

### Comparing `didabox-2.3.0/src/didabox/request.py` & `didabox-2.4.0/src/didabox/request.py`

 * *Files identical despite different names*

### Comparing `didabox-2.3.0/src/didabox/utils.py` & `didabox-2.4.0/src/didabox/utils.py`

 * *Files identical despite different names*

### Comparing `didabox-2.3.0/PKG-INFO` & `didabox-2.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: didabox
-Version: 2.3.0
+Version: 2.4.0
 Summary: dida api
 License: MIT
 Author: luke9012
 Author-email: luke781520097@163.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pytz (>=2023.3.post1)
 Requires-Dist: requests (>=2.27.1)
 Description-Content-Type: text/markdown
 
 # didabox
 滴答清单接口封装, python版
 
 接口参考: https://github.com/luke1879012/dida_api
```

