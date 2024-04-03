# Comparing `tmp/lazyofapi-0.1.4.tar.gz` & `tmp/lazyofapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyofapi-0.1.4.tar", max compression
+gzip compressed data, was "lazyofapi-0.1.5.tar", max compression
```

## Comparing `lazyofapi-0.1.4.tar` & `lazyofapi-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-10-05 09:53:48.630073 lazyofapi-0.1.4/lazyOfAPI/__init__.py
--rw-r--r--   0        0        0    11458 2024-03-31 12:50:03.317581 lazyofapi-0.1.4/lazyOfAPI/OpenFrpAPI.py
--rw-r--r--   0        0        0    35182 2023-10-05 10:26:54.751105 lazyofapi-0.1.4/LICENSE
--rw-r--r--   0        0        0      454 2024-03-31 15:25:06.880203 lazyofapi-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3523 2024-03-30 07:29:53.297450 lazyofapi-0.1.4/README.md
--rw-r--r--   0        0        0     4284 1970-01-01 00:00:00.000000 lazyofapi-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-10-05 09:53:48.630073 lazyofapi-0.1.5/lazyOfAPI/__init__.py
+-rw-r--r--   0        0        0    11509 2024-04-03 13:45:10.148689 lazyofapi-0.1.5/lazyOfAPI/OpenFrpAPI.py
+-rw-r--r--   0        0        0    35182 2023-10-05 10:26:54.751105 lazyofapi-0.1.5/LICENSE
+-rw-r--r--   0        0        0      454 2024-04-03 13:57:24.942242 lazyofapi-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3523 2024-03-30 07:29:53.297450 lazyofapi-0.1.5/README.md
+-rw-r--r--   0        0        0     4284 1970-01-01 00:00:00.000000 lazyofapi-0.1.5/PKG-INFO
```

### Comparing `lazyofapi-0.1.4/lazyOfAPI/OpenFrpAPI.py` & `lazyofapi-0.1.5/lazyOfAPI/OpenFrpAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,17 @@
             if item.get("proxyName") == name:
                 return item
 
     def remove_proxy(self, proxy_id: int) -> bool:
         """删除隧道"""
         url = self.base_url + "/frp/api/removeProxy"
         data = {"proxy_id": proxy_id}
-        response = self.request.post(url, data=data, headers=self.headers, proxies=self.proxy)
+        response = self.request.post(url, json=data, headers=self.headers, proxies=self.proxy)
+        print(data)
+        print(response.json())
         return response.json().get("flag", False)
 
     def get_node_list(self, classify: int = 0, group: list = ()) -> list:
         """获取节点列表"""
         url = self.base_url + "/frp/api/getNodeList"
         response = self.request.post(url, headers=self.headers, proxies=self.proxy)
         res = response.json().get("data").get("list")
```

### Comparing `lazyofapi-0.1.4/LICENSE` & `lazyofapi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyofapi-0.1.4/README.md` & `lazyofapi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lazyofapi-0.1.4/PKG-INFO` & `lazyofapi-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyOfAPI
-Version: 0.1.4
+Version: 0.1.5
 Summary: 一个简单的用于请求OpenFrp API的库
 License: AGPLv3
 Author: MojaveHao
 Author-email: HTTcode2020@126.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

