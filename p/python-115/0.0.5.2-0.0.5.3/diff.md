# Comparing `tmp/python_115-0.0.5.2.tar.gz` & `tmp/python_115-0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.5.2.tar", max compression
+gzip compressed data, was "python_115-0.0.5.3.tar", max compression
```

## Comparing `python_115-0.0.5.2.tar` & `python_115-0.0.5.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.2/LICENSE
--rw-r--r--   0        0        0   253746 2024-04-03 04:45:26.887593 python_115-0.0.5.2/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.2/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.2/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.2/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.2/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.2/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.2/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.2/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.2/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.2/p115/util/download.py
--rw-r--r--   0        0        0    14936 2024-04-02 07:02:17.355689 python_115-0.0.5.2/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.2/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.2/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.2/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.2/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.2/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.2/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.2/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.2/p115/util/text.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.2/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-03 04:47:11.974962 python_115-0.0.5.2/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.2/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.3/LICENSE
+-rw-r--r--   0        0        0   253816 2024-04-03 05:37:00.295957 python_115-0.0.5.3/p115/__init__.py
+-rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.3/p115/__main__.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.3/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.3/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.3/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.3/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.3/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.3/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.3/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.3/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.3/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.3/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.3/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.3/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.3/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.3/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.3/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.3/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.3/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.3/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.3/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-03 05:34:30.162787 python_115-0.0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.3/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.3/PKG-INFO
```

### Comparing `python_115-0.0.5.2/LICENSE` & `python_115-0.0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/__init__.py` & `python_115-0.0.5.3/p115/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3956,16 +3956,19 @@
             no_root=no_root, 
             write_mode=write_mode, 
         )
 
     def exists(self, /) -> bool:
         return self.fs.exists(self)
 
-    def get_url(self, /, headers: Optional[Mapping] = None) -> str:
-        return self.fs.get_url(self, headers=headers)
+    @property
+    def file_extension(self, /) -> Optional[str]:
+        if not self.is_file():
+            return None
+        return splitext(basename(self.path))[1]
 
     def glob(
         self, 
         /, 
         pattern: str = "*", 
         ignore_case: bool = False, 
         allow_escaped_slash: bool = True, 
@@ -4482,31 +4485,40 @@
             return True
         except FileNotFoundError:
             return False
 
     def getcid(self, /) -> int:
         return self.cid
 
-    def getcwd(self, /) -> str:
+    def getcwd(self, /, fetch_attr: bool = False) -> str:
+        if fetch_attr:
+            return self.attr(self.cid)["path"]
         return self.path
 
     def get_id(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> int:
         if pid is None and (not id_or_path or id_or_path == "."):
             return self.cid
         elif isinstance(id_or_path, type(self).path_class):
             return id_or_path.id
         elif isinstance(id_or_path, int):
             return id_or_path
-        if self.get_path(id_or_path, pid) == "/":
+        if id_or_path == "/":
             return 0
+        try:
+            path_to_id = getattr(self, "path_to_id", None)
+            if path_to_id is not None:
+                path = self.get_path(id_or_path, pid)
+                return path_to_id[path]
+        except LookupError:
+            pass
         return self.attr(id_or_path, pid)["id"]
 
     def get_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
@@ -5437,15 +5449,15 @@
             pid_attrs is None or 
             "version" not in pid_attrs or
             version != pid_attrs["version"]
         ):
             pagesize = 1 << 10
             def normalize_attr(attr, dirname, /, **extra):
                 attr = normalize_info(attr, **extra)
-                path = joinpath(dirname, escape(attr["name"]))
+                path = attr["path"] = joinpath(dirname, escape(attr["name"]))
                 if path_to_id is not None:
                     path_to_id[path] = attr["id"]
                 if id_to_children is not None:
                     try:
                         id_attrs = id_to_children[attr["id"]]
                     except LookupError:
                         id_to_children[attr["id"]] = {"attr": attr}
@@ -6222,15 +6234,15 @@
         try:
             return self.attr(id_or_path, pid)
         except FileNotFoundError:
             if isinstance(id_or_path, int):
                 raise ValueError(f"no such id: {id_or_path!r}")
             return self.upload(BytesIO(), id_or_path, pid=pid)
 
-    # TODO: 增加功能，返回一个 Future 对象，可以获取上传进度，可随时取消
+    # TODO: 增加功能，返回一个 Task 对象，可以获取上传进度，可随时取消
     def upload(
         self, 
         /, 
         file: bytes | str | PathLike | SupportsRead[bytes], 
         path: IDOrPathType = "", 
         pid: Optional[int] = None, 
         overwrite_or_ignore: Optional[bool] = None, 
@@ -6274,17 +6286,16 @@
                     raise IsADirectoryError(errno.EISDIR, f"{path!r} (in {pid!r}) is a directory")
                 elif not overwrite_or_ignore:
                     return attr
                 self._delete(attr["id"])
         return self._upload(fio, name, pid)
 
     # TODO: 为了提升速度，之后会支持多线程上传，以及直接上传不做检查
-    # TODO: 增加功能，可以多线程上传或异步上传，返回 Future 对象，可以获取每个上传任务的进度，并且可以随时取消
-    # TODO: 增加断言，可以选择不上传某些文件
-    # TODO: 增加参数，as_task=False，将任务提交到上传队列，返回task对象，可以随时取消，也可以操作调度的 executor
+    # TODO: 返回上传任务的迭代器，包含进度相关信息，以及最终的响应信息
+    # TODO: 增加参数，onerror, predicate, submit 等
     def upload_tree(
         self, 
         /, 
         local_path: str | PathLike[str] = ".", 
         path: IDOrPathType = "", 
         pid: Optional[int] = None, 
         no_root: bool = False, 
@@ -6639,14 +6650,15 @@
             0 if is_dir else attr["size"], 
             attr.get("time", lastest_update).timestamp(), 
             attr.get("time", lastest_update).timestamp(), 
             attr.get("time", lastest_update).timestamp(), 
         ))
 
 
+# TODO: 兼容 pathlib.Path 和 zipfile.Path 的接口
 class P115ZipPath(P115PathBase):
     fs: P115ZipFileSystem
     path: str
 
 
 class ExportDirStatus(Future):
     _condition: Condition
@@ -6777,15 +6789,15 @@
                 except BaseException as e:
                     self.set_exception(e)
                     return
                 sleep(1)
         Thread(target=update_progress).start()
 
 
-# TODO: 参考zipfile的接口设计 namelist filelist
+# TODO: 参考 zipfile 模块的接口设计 namelist、filelist 等属性，以及其它的和 zipfile 兼容的接口
 # TODO: 当文件特别多时，可以用 zipfile 等模块来读取文件列表
 class P115ZipFileSystem(P115FileSystemBase[MappingProxyType, P115ZipPath]):
     file_id: Optional[int]
     pick_code: str
     path_to_id: MutableMapping[str, int]
     id_to_attr: MutableMapping[int, MappingProxyType]
     id_to_children: MutableMapping[int, tuple[MappingProxyType]]
@@ -7373,12 +7385,7 @@
 
 # TODO upload_tree 多线程和进度条，并且为每一个上传返回一个 task，可重试
 # TODO 能及时处理文件已不存在
 # TODO 为各个fs接口添加额外的请求参数
 # TODO 115中多个文件可以在同一目录下同名，如何处理
 # TODO 上传如果失败，因为名字问题，则尝试用uuid名字，上传成功后，再进行改名，如果成功，删除原来的文件，不成功，则删掉上传的文件（如果上传了的话）
 # TODO 如果压缩包尚未解压，则使用 zipfile 之类的模块，去模拟文件系统
-# TODO 支持传入作为缓存的 MutableMapping
-# TODO 调用 getcwd 时需要获取最新的名字
-# TODO 支持 pickle 序列化和反序列化
-# TODO 支持上传、下载的 Future，可以 cancel、pause、resume 等
-
```

### Comparing `python_115-0.0.5.2/p115/util/_init_mimetypes.py` & `python_115-0.0.5.3/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/cipher.py` & `python_115-0.0.5.3/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/concurrent.py` & `python_115-0.0.5.3/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/download.py` & `python_115-0.0.5.3/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/file.py` & `python_115-0.0.5.3/p115/util/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,16 @@
     else:
         return -1
     return total
 
 
 from .urlopen import urlopen
 
+# TODO: 再尝试设计实现一个 HTTPFileWriter
+# TODO: 如果是 Range 请求，返回的状态码是 206，这也是一个明显的特征，是否能加以利用
 class HTTPFileReader(RawIOBase, BinaryIO):
     url: str | Callable[[], str]
     response: Any
     length: int
     chunked: bool
     start: int
     urlopen: Callable
```

### Comparing `python_115-0.0.5.2/p115/util/hash.py` & `python_115-0.0.5.3/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/ignore.py` & `python_115-0.0.5.3/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/iter.py` & `python_115-0.0.5.3/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/path.py` & `python_115-0.0.5.3/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/property.py` & `python_115-0.0.5.3/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/response.py` & `python_115-0.0.5.3/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/retry.py` & `python_115-0.0.5.3/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/text.py` & `python_115-0.0.5.3/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/p115/util/urlopen.py` & `python_115-0.0.5.3/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/pyproject.toml` & `python_115-0.0.5.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.5.2"
+version = "0.0.5.3"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.5.2/readme.md` & `python_115-0.0.5.3/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.2/PKG-INFO` & `python_115-0.0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

