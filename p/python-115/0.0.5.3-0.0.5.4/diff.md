# Comparing `tmp/python_115-0.0.5.3.tar.gz` & `tmp/python_115-0.0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.5.3.tar", max compression
+gzip compressed data, was "python_115-0.0.5.4.tar", max compression
```

## Comparing `python_115-0.0.5.3.tar` & `python_115-0.0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.3/LICENSE
--rw-r--r--   0        0        0   253816 2024-04-03 05:37:00.295957 python_115-0.0.5.3/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.3/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.3/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.3/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.3/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.3/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.3/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.3/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.3/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.3/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.3/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.3/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.3/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.3/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.3/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.3/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.3/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.3/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.3/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.3/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.3/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-03 05:34:30.162787 python_115-0.0.5.3/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.3/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.4/LICENSE
+-rw-r--r--   0        0        0   256072 2024-04-03 06:35:19.651313 python_115-0.0.5.4/p115/__init__.py
+-rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.4/p115/__main__.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.4/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.4/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.4/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.4/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.4/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.4/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.4/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.4/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.4/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.4/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.4/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.4/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.4/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.4/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.4/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.4/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.4/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.4/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.4/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-03 06:36:29.551065 python_115-0.0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.4/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.4/PKG-INFO
```

### Comparing `python_115-0.0.5.3/LICENSE` & `python_115-0.0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/__init__.py` & `python_115-0.0.5.4/p115/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3468,20 +3468,26 @@
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """添加一个离线任务
         POST https://115.com/web/lixian/?ct=lixian&ac=add_task_url
         payload:
             - url: str
+            - sign: str = <default>
+            - time: int = <default>
             - savepath: str = <default>
             - wp_path_id: int | str = <default>
         """
         api = "https://115.com/web/lixian/?ct=lixian&ac=add_task_url"
         if isinstance(payload, str):
             payload = {"url": payload}
+        if "sign" not in payload:
+            info = self.offline_info()
+            payload["sign"] = info["sign"]
+            payload["time"] = info["time"]
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def offline_add_urls(
         self, 
         payload: Iterable[str] | dict, 
         /, 
         async_: bool = False, 
@@ -3489,40 +3495,52 @@
     ) -> dict:
         """添加一组离线任务
         POST https://115.com/web/lixian/?ct=lixian&ac=add_task_urls
         payload:
             - url[0]: str
             - url[1]: str
             - ...
+            - sign: str = <default>
+            - time: int = <default>
             - savepath: str = <default>
             - wp_path_id: int | str = <default>
         """
         api = "https://115.com/web/lixian/?ct=lixian&ac=add_task_urls"
         if not isinstance(payload, dict):
             payload = {f"url[{i}]": url for i, url in enumerate(payload)}
             if not payload:
                 raise ValueError("no `url` specified")
+        if "sign" not in payload:
+            info = self.offline_info()
+            payload["sign"] = info["sign"]
+            payload["time"] = info["time"]
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def offline_add_torrent(
         self, 
         payload: dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """添加一个种子作为离线任务
         POST https://115.com/web/lixian/?ct=lixian&ac=add_task_bt
         payload:
             - info_hash: str
             - wanted: str
+            - sign: str = <default>
+            - time: int = <default>
             - savepath: str = <default>
             - wp_path_id: int | str = <default>
         """
         api = "https://115.com/web/lixian/?ct=lixian&ac=add_task_bt"
+        if "sign" not in payload:
+            info = self.offline_info()
+            payload["sign"] = info["sign"]
+            payload["time"] = info["time"]
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def offline_torrent_info(
         self, 
         payload: str | dict, 
         /, 
         async_: bool = False, 
@@ -3547,19 +3565,25 @@
     ) -> dict:
         """删除一组离线任务（无论是否已经完成）
         POST https://lixian.115.com/lixian/?ct=lixian&ac=task_del
         payload:
             - hash[0]: str
             - hash[1]: str
             - ...
+            - sign: str = <default>
+            - time: int = <default>
             - flag: 0 | 1 = <default> # 是否删除源文件
         """
         api = "https://lixian.115.com/lixian/?ct=lixian&ac=task_del"
         if isinstance(payload, str):
             payload = {"hash[0]": payload}
+        if "sign" not in payload:
+            info = self.offline_info()
+            payload["sign"] = info["sign"]
+            payload["time"] = info["time"]
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def offline_list(
         self, 
         payload: int | dict = 1, 
         /, 
         async_: bool = False, 
@@ -4303,14 +4327,22 @@
     def __itruediv__(self, id_or_path: IDOrPathType, /) -> Self:
         self.chdir(id_or_path)
         return self
 
     def __len__(self, /) -> int:
         return len(tuple(self.iterdir()))
 
+    def __repr__(self, /) -> str:
+        cls = type(self)
+        module = cls.__module__
+        name = cls.__qualname__
+        if module != "__main__":
+            name = module + "." + name
+        return f"<{name}(client={self.client!r}, cid={self.cid!r}, path={self.path!r}) at {hex(id(self))}>"
+
     @abstractmethod
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> M:
@@ -5201,22 +5233,14 @@
 
     def __delitem__(self, id_or_path: IDOrPathType, /):
         self.rmtree(id_or_path)
 
     def __len__(self, /) -> int:
         return self.get_directory_capacity(self.cid)
 
-    def __repr__(self, /) -> str:
-        cls = type(self)
-        module = cls.__module__
-        name = cls.__qualname__
-        if module != "__main__":
-            name = module + "." + name
-        return f"<{name}(client={self.client!r}, cid={self.cid!r}, path={self.path!r}) at {hex(id(self))}>"
-
     def __setattr__(self, attr, val, /) -> Never:
         raise TypeError("can't set attribute")
 
     def __setitem__(
         self, 
         id_or_path: IDOrPathType, 
         file: None | str | bytes | bytearray | memoryview | PathLike = None, 
@@ -7035,14 +7059,35 @@
 
     def __iter__(self, /) -> Iterator[dict]:
         return self.iter()
 
     def __len__(self, /) -> int:
         return check_response(self.client.offline_list())["count"]
 
+    def __repr__(self, /) -> str:
+        cls = type(self)
+        module = cls.__module__
+        name = cls.__qualname__
+        if module != "__main__":
+            name = module + "." + name
+        return f"<{name}(client={self.client!r}) at {hex(id(self))}>"
+
+    @property
+    def sign_time(self, /):
+        ns = self.__dict__
+        try:
+            sign_time = ns["sign_time"]
+            if time() - sign_time["time"] < 30 * 60:
+                return sign_time
+        except KeyError:
+            pass
+        info = check_response(self.client.offline_info())
+        sign_time = ns["sign_time"] = {"sign": info["sign"], "time": info["time"]}
+        return sign_time
+
     def add(
         self, 
         urls: str | Iterable[str], 
         /, 
         pid: Optional[int] = None, 
         savepath: Optional[str] = None, 
     ) -> dict:
@@ -7051,14 +7096,15 @@
             payload = {"url": urls}
             method = self.client.offline_add_url
         else:
             payload = {f"url[{i}]": url for i, url in enumerate(urls)}
             if not payload:
                 raise ValueError("no `url` specified")
             method = self.client.offline_add_urls
+        payload.update(self.sign_time)
         if pid is not None:
             payload["wp_path_id"] = pid
         if savepath:
             payload["savepath"] = savepath
         return check_response(method(payload))
 
     def add_torrent(
@@ -7085,14 +7131,15 @@
         payload = {
             "info_hash": resp["info_hash"], 
             "wanted": wanted, 
             "savepath": resp["torrent_name"] if savepath is None else savepath, 
         }
         if pid is not None:
             payload["wp_path_id"] = pid
+        payload.update(self.sign_time)
         return check_response(self.client.offline_add_torrent(payload))
 
     def clear(self, /, flag: int = 1) -> dict:
         """清空离线任务列表
 
         :param flag: 操作目标
             - 0: 已完成
@@ -7143,14 +7190,15 @@
             payload = {"hash[0]": hashes}
         else:
             payload = {f"hash[{i}]": h for i, h in enumerate(hashes)}
             if not payload:
                 raise ValueError("no `hash` specified")
         if remove_files:
             payload["flag"] = "1"
+        payload.update(self.sign_time)
         return check_response(self.client.offline_remove(payload))
 
     def torrent_info(self, torrent_or_magnet_or_sha1_or_fid: int | bytes | str, /) -> dict:
         torrent = None
         if isinstance(torrent_or_magnet_or_sha1_or_fid, int):
             fid = torrent_or_magnet_or_sha1_or_fid
             resp = check_response(self.client.fs_file(fid))
@@ -7204,14 +7252,22 @@
 
     def __iter__(self, /) -> Iterator[dict]:
         return self.iter()
 
     def __len__(self, /) -> int:
         return int(check_response(self.client.recyclebin_list({"limit": 1}))["count"])
 
+    def __repr__(self, /) -> str:
+        cls = type(self)
+        module = cls.__module__
+        name = cls.__qualname__
+        if module != "__main__":
+            name = module + "." + name
+        return f"<{name}(client={self.client!r}) at {hex(id(self))}>"
+
     @check_response
     def clear(self, /, password: None | int | str = None) -> dict:
         if password is None:
             password = self.password
         return self.client.recyclebin_clean({"password": password})
 
     def get(self, id: int | str, /, default=None):
@@ -7298,14 +7354,22 @@
 
     def __iter__(self, /) -> Iterator[dict]:
         return self.iter()
 
     def __len__(self, /) -> int:
         return check_response(self.client.share_list({"limit": 1}))["count"]
 
+    def __repr__(self, /) -> str:
+        cls = type(self)
+        module = cls.__module__
+        name = cls.__qualname__
+        if module != "__main__":
+            name = module + "." + name
+        return f"<{name}(client={self.client!r}) at {hex(id(self))}>"
+
     @check_response
     def add(
         self, 
         file_ids: int | str | Iterable[int | str], 
         /, 
         is_asc: Literal[0, 1] = 1, 
         order: str = "file_name",
```

### Comparing `python_115-0.0.5.3/p115/util/_init_mimetypes.py` & `python_115-0.0.5.4/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/cipher.py` & `python_115-0.0.5.4/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/concurrent.py` & `python_115-0.0.5.4/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/download.py` & `python_115-0.0.5.4/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/file.py` & `python_115-0.0.5.4/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/hash.py` & `python_115-0.0.5.4/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/ignore.py` & `python_115-0.0.5.4/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/iter.py` & `python_115-0.0.5.4/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/path.py` & `python_115-0.0.5.4/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/property.py` & `python_115-0.0.5.4/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/response.py` & `python_115-0.0.5.4/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/retry.py` & `python_115-0.0.5.4/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/text.py` & `python_115-0.0.5.4/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/p115/util/urlopen.py` & `python_115-0.0.5.4/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/pyproject.toml` & `python_115-0.0.5.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.5.3"
+version = "0.0.5.4"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.5.3/readme.md` & `python_115-0.0.5.4/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.3/PKG-INFO` & `python_115-0.0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.5.3
+Version: 0.0.5.4
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

