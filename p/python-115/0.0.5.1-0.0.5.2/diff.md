# Comparing `tmp/python_115-0.0.5.1.tar.gz` & `tmp/python_115-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.5.1.tar", max compression
+gzip compressed data, was "python_115-0.0.5.2.tar", max compression
```

## Comparing `python_115-0.0.5.1.tar` & `python_115-0.0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.1/LICENSE
--rw-r--r--   0        0        0   252566 2024-04-02 11:34:36.820422 python_115-0.0.5.1/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.1/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.1/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.1/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.1/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.1/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.1/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.1/p115/util/cipher.py
--rw-r--r--   0        0        0     5670 2024-04-02 11:03:33.575384 python_115-0.0.5.1/p115/util/concurrent.py
--rw-r--r--   0        0        0    12108 2024-04-02 11:33:11.042124 python_115-0.0.5.1/p115/util/download.py
--rw-r--r--   0        0        0    14936 2024-04-02 07:02:17.355689 python_115-0.0.5.1/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.1/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.1/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.1/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.1/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.1/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.1/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.1/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.1/p115/util/text.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.1/p115/util/urlopen.py
--rw-r--r--   0        0        0     1251 2024-04-02 11:34:52.132047 python_115-0.0.5.1/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.1/readme.md
--rw-r--r--   0        0        0    35866 1970-01-01 00:00:00.000000 python_115-0.0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.2/LICENSE
+-rw-r--r--   0        0        0   253746 2024-04-03 04:45:26.887593 python_115-0.0.5.2/p115/__init__.py
+-rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.2/p115/__main__.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.2/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.2/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.2/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.2/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.2/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.2/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.2/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.2/p115/util/download.py
+-rw-r--r--   0        0        0    14936 2024-04-02 07:02:17.355689 python_115-0.0.5.2/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.2/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.2/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.2/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.2/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.2/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.2/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.2/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.2/p115/util/text.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.2/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-03 04:47:11.974962 python_115-0.0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.2/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.2/PKG-INFO
```

### Comparing `python_115-0.0.5.1/LICENSE` & `python_115-0.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/__init__.py` & `python_115-0.0.5.2/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from xml.etree.ElementTree import fromstring
 
 from aiohttp import ClientSession
 from requests.cookies import create_cookie
 from requests.exceptions import Timeout
 from requests.models import Response
 from requests.sessions import Session
+from magnet2torrent import Magnet2Torrent # type: ignore
 from yarl import URL
 
 # NOTE: OR use `pyqrcode` instead
 import qrcode # type: ignore
 
 from .exception import AuthenticationError, LoginError
 from .util.args import argcount
@@ -309,14 +310,24 @@
                 raise LoginError("[status=-1] qrcode: expired")
             elif status == -2:
                 raise LoginError("[status=-2] qrcode: canceled")
             else:
                 raise LoginError(f"qrcode: aborted with {resp!r}")
         return self.login_qrcode_result({"account": qrcode_token["uid"], "app": app}, **request_kwargs)
 
+    def login(
+        self, 
+        /, 
+        app: str = "web", 
+        **request_kwargs, 
+    ):
+        if not self.is_login(**request_kwargs):
+            cookie = self.login_with_qrcode(app, **request_kwargs)["data"]["cookie"]
+            self.set_cookie(cookie)
+
     def _request(
         self, 
         /, 
         url: str, 
         method: str = "GET", 
         parse: None | bool | Callable = False, 
         **request_kwargs, 
@@ -4409,15 +4420,15 @@
         /, 
         local_dir: bytes | str | PathLike = "", 
         pid: Optional[int] = None, 
         write_mode: Literal["i", "x", "w", "a"] = "a", 
         submit = None, 
         no_root: bool = False, 
         predicate: Optional[Callable[[P115PathType], bool]] = None, 
-        onerror: Optional[Callable[[BaseException], Any]] = None, 
+        onerror: None | bool | Callable[[BaseException], Any] = None, 
     ) -> Iterator[DownloadTask]:
         local_dir = fsdecode(local_dir)
         if local_dir:
             makedirs(local_dir, exist_ok=True)
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             if not no_root:
@@ -4442,20 +4453,24 @@
                 try:
                     task = self.download(
                         subpath["id"], 
                         ospath.join(local_dir, subpath["name"]), 
                         write_mode=write_mode, 
                         submit=submit, 
                     )
-                    if task is not None:
-                        yield task
                 except KeyboardInterrupt:
                     raise
                 except BaseException as exc:
-                    onerror and onerror(exc)
+                    if onerror is None or onerror is True:
+                        raise
+                    elif callable(onerror):
+                        onerror(exc)
+                else:
+                    if task is not None:
+                        yield task
 
     def exists(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
@@ -5396,72 +5411,81 @@
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         refresh: bool = False, 
     ) -> Iterator[dict]:
+        path_to_id = self.path_to_id
         id_to_children = self.id_to_children
         get_version = self.get_version
+        version = None
         if id_to_children is None and isinstance(id_or_path, int):
             id = id_or_path
-            version = None
         else:
             attr = self.attr(id_or_path, pid)
             if not attr["is_directory"]:
                 raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
             id = attr["id"]
-            version = get_version and get_version(attr)
+            if get_version is not None:
+                version = get_version(attr)
         if id_to_children is None:
             pid_attrs = None
         else:
             pid_attrs = id_to_children.get(id)
         if (
             refresh or 
             pid_attrs is None or 
             "version" not in pid_attrs or
             version != pid_attrs["version"]
         ):
             pagesize = 1 << 10
+            def normalize_attr(attr, dirname, /, **extra):
+                attr = normalize_info(attr, **extra)
+                path = joinpath(dirname, escape(attr["name"]))
+                if path_to_id is not None:
+                    path_to_id[path] = attr["id"]
+                if id_to_children is not None:
+                    try:
+                        id_attrs = id_to_children[attr["id"]]
+                    except LookupError:
+                        id_to_children[attr["id"]] = {"attr": attr}
+                    else:
+                        try:
+                            old_attr = id_attrs["attr"]
+                        except LookupError:
+                            id_attrs["attr"] = attr
+                        else:
+                            if path != old_attr["path"] and path_to_id is not None:
+                                try:
+                                    del path_to_id[old_attr["path"]]
+                                except LookupError:
+                                    pass
+                            old_attr.update(attr)
+                return attr
             def iterdir():
                 get_files = self._files
-                path_to_id = self.path_to_id
                 resp = get_files(id, limit=pagesize)
                 dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
                 if path_to_id is not None:
                     path_to_id[dirname] = id
                 lastest_update = datetime.now()
                 count = resp["count"]
                 for attr in resp["data"]:
-                    attr = normalize_info(attr, lastest_update=lastest_update)
-                    path = attr["path"] = joinpath(dirname, escape(attr["name"]))
-                    if path_to_id is not None:
-                        path_to_id[path] = attr["id"]
-                    if id_to_children is not None:
-                        try:
-                            id_to_children[attr["id"]].update(attr)
-                        except KeyError:
-                            id_to_children[attr["id"]] = {"attr": attr}
-                    yield attr
+                    yield normalize_attr(attr, dirname, lastest_update=lastest_update)
                 for offset in range(pagesize, count, 1 << 10):
                     resp = get_files(id, limit=pagesize, offset=offset)
                     lastest_update = datetime.now()
                     if resp["count"] != count:
                         raise RuntimeError(f"{id} detected count changes during iteration")
                     for attr in resp["data"]:
-                        attr = normalize_info(attr, lastest_update=lastest_update)
-                        path = attr["path"] = joinpath(dirname, escape(attr["name"]))
-                        if path_to_id is not None:
-                            path_to_id[path] = attr["id"]
-                        yield attr
+                        yield normalize_attr(attr, dirname, lastest_update=lastest_update)
             children = {a["id"]: a for a in iterdir()}
             if id_to_children is not None:
-                attrs = id_to_children[id] = {"attr": attr, "children": children}
-                if get_version is not None:
-                    attrs["version"] = version
+                attrs = id_to_children[id] = {"version": version, "attr": attr, "children": children}
         else:
             children = pid_attrs["children"]
         return iter(children.values())
 
     def _attr(self, id: int, /) -> dict:
         if id == 0:
             lastest_update = datetime.now()
@@ -5486,39 +5510,55 @@
         if attrs and "attr" in attrs and get_version is None:
             return attrs["attr"]
         try:
             data = self._info(id)["data"][0]
         except OSError as e:
             raise FileNotFoundError(errno.ENOENT, f"no such id: {id!r}") from e
         attr = normalize_info(data, lastest_update=datetime.now())
+        pid = attr["parent_id"]
+        attr_old = None
         if id_to_children is not None:
             if get_version is None:
                 version = None
             else:
                 version = get_version(attr)
-            if not attrs or "attr" not in attrs or version != attrs.get("version"):
-                pid = attr["parent_id"]
-                if pid:
-                    path = joins((*(a["name"] for a in self._dir_get_ancestors(pid)), attr["name"]))
-                else:
-                    path = "/" + escape(attr["name"])
-                path_to_id = self.path_to_id
-                if path_to_id is not None:
-                    path_to_id[path] = id
-                attr["path"] = path
+            if attrs is None or "attr" not in attrs:
                 if attrs is None:
                     id_to_children[id] = {"attr": attr}
-                    if pid not in id_to_children:
-                        id_to_children[pid] = {}
-                    id_to_children.setdefault(pid, {})[id] = attr
                 else:
+                    attrs["attr"] = attr
+                try:
+                    pid_attrs = id_to_children[pid]
+                except LookupError:
+                    pid_attrs = id_to_children[pid] = {}
+                try:
+                    children = pid_attrs["children"]
+                except LookupError:
+                    children = pid_attrs["children"] = {}
+                children[id] = attr
+            else:
+                attr_old = attrs["attr"]
+                if version != attrs.get("version"):
                     attrs.pop("version", None)
-                    attrs["attr"].update(attr)
+                attr_old.update(attr)
+                attr = attr_old
+        if "path" not in attr:
+            if pid:
+                path = attr["path"] = joins(
+                    (*(a["name"] for a in self._dir_get_ancestors(pid)), attr["name"]))
             else:
-                attrs["attr"].update(attr)
+                path = attr["path"] = "/" + escape(attr["name"])
+            path_to_id = self.path_to_id
+            if path_to_id is not None:
+                path_to_id[path] = id
+                if attr_old and path != attr_old["path"]:
+                    try:
+                        del path_to_id[attr_old["path"]]
+                    except LookupError:
+                        pass
         return attr
 
     def _attr_path(
         self, 
         path: str | PathLike[str] | Sequence[str], 
         /, 
         pid: Optional[int] = None, 
@@ -7102,32 +7142,30 @@
         if isinstance(torrent_or_magnet_or_sha1_or_fid, int):
             fid = torrent_or_magnet_or_sha1_or_fid
             resp = check_response(self.client.fs_file(fid))
             sha = resp["data"][0]["sha1"]
         elif isinstance(torrent_or_magnet_or_sha1_or_fid, bytes):
             torrent = torrent_or_magnet_or_sha1_or_fid
         elif torrent_or_magnet_or_sha1_or_fid.startswith("magnet:?xt=urn:btih:"):
-            info_hash = torrent_or_magnet_or_sha1_or_fid[20:60]
-            url = f"https://itorrents.org/torrent/{info_hash}.torrent"
-            with Session() as session:
-                with session.get(url, headers={"User-Agent": "Mozilla/5.0"}) as response:
-                    response.raise_for_status()
-                    torrent = response.content
+            m2t = Magnet2Torrent(torrent_or_magnet_or_sha1_or_fid)
+            torrent = run(m2t.retrieve_torrent())[1]
         else:
             sha = torrent_or_magnet_or_sha1_or_fid
         if torrent is None:
-            return check_response(self.client.offline_torrent_info(sha))
+            resp = check_response(self.client.offline_torrent_info(sha))
         else:
             sha = sha1(torrent).hexdigest()
             try:
-                return check_response(self.client.offline_torrent_info(sha))
+                resp = check_response(self.client.offline_torrent_info(sha))
             except:
-                name = f"{uuid4()}.torrent"
+                name = f"{sha}.torrent"
                 check_response(self.client.upload_file_sample(torrent, name, 0))
-                return check_response(self.client.offline_torrent_info(sha))
+                resp = check_response(self.client.offline_torrent_info(sha))
+        resp["sha1"] = sha
+        return resp
 
 
 class P115Recyclebin:
     __slots__ = ("client", "password")
 
     def __init__(
         self,
```

### Comparing `python_115-0.0.5.1/p115/util/_init_mimetypes.py` & `python_115-0.0.5.2/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/cipher.py` & `python_115-0.0.5.2/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/concurrent.py` & `python_115-0.0.5.2/p115/util/concurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__all__ = ["thread_batch", "thread_pool_batch", "async_batch", "as_thread", "run_thread"]
+__all__ = ["thread_batch", "thread_pool_batch", "async_batch", "threaded", "run_as_thread"]
 
 from asyncio import CancelledError, Semaphore as AsyncSemaphore, TaskGroup
 from collections.abc import Callable, Coroutine, Iterable
 from concurrent.futures import Future, ThreadPoolExecutor
 from functools import partial, update_wrapper
 from inspect import isawaitable
 from queue import Queue
@@ -138,22 +138,22 @@
         return create_task(works(task))
     async with TaskGroup() as tg:
         create_task = tg.create_task
         for task in tasks:
             submit(task)
 
 
-def as_thread(
+def threaded(
     func: Optional[Callable] = None, 
     /, 
     lock = None, 
     **thread_init_kwds, 
 ):
     if func is None:
-        return partial(as_thread, **thread_init_kwds)
+        return partial(threaded, **thread_init_kwds)
     if isinstance(lock, int):
         lock = Semaphore(lock)
     def wrapper(*args, **kwds) -> Future[V]:
         if lock is None:
             def asfuture():
                 try: 
                     fu.set_result(func(*args, **kwds))
@@ -169,18 +169,18 @@
         fu: Future[V] = Future()
         thread = fu.thread = Thread(target=asfuture, **thread_init_kwds) # type: ignore
         thread.start()
         return fu
     return update_wrapper(wrapper, func)
 
 
-def run_thread(
+def run_as_thread(
     func: Optional[Callable] = None, 
     /, 
     *args, 
     **kwargs, 
 ):
     if func is None:
-        f = as_thread(None, *args, **kwargs)
+        f = threaded(None, *args, **kwargs)
         return lambda func, *args, **kwargs: f(func)(*args, **kwargs)
-    return as_thread(func)(*args, **kwargs)
+    return threaded(func)(*args, **kwargs)
```

### Comparing `python_115-0.0.5.1/p115/util/download.py` & `python_115-0.0.5.2/p115/util/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 from typing import cast, Any, NamedTuple, Never, Optional, Self
 
 from requests import Response, Session
 
 if __name__ == "__main__":
     from sys import path
     path.insert(0, dirname(dirname(__file__)))
-    from util.concurrent import run_thread # type: ignore
+    from util.concurrent import run_as_thread # type: ignore
     from util.file import bio_skip_iter, SupportsRead, SupportsWrite # type: ignore
     from util.iter import cut_iter # type: ignore
     from util.response import get_filename, get_length, is_chunked, is_range_request # type: ignore
     from util.text import headers_str_to_dict # type: ignore
     from util.urlopen import urlopen # type: ignore
     del path[0]
 else:
-    from .concurrent import run_thread
+    from .concurrent import run_as_thread
     from .file import bio_skip_iter, SupportsRead, SupportsWrite
     from .iter import cut_iter
     from .response import get_filename, get_length, is_chunked, is_range_request
     from .text import headers_str_to_dict
     from .urlopen import urlopen
 
 
@@ -84,15 +84,15 @@
     @property
     def task_done(self, /) -> bool:
         return self.completed >= self.total
 
 
 class DownloadTask:
 
-    def __init__(self, /, gen, submit=run_thread):
+    def __init__(self, /, gen, submit=run_as_thread):
         if not callable(submit):
             submit = submit.submit
         self._submit = submit
         self._state = "PENDING"
         self._gen = gen
         self._done_event = Event()
 
@@ -100,15 +100,15 @@
         return f"<{type(self).__qualname__} :: state={self.state!r} progress={self.progress!r}>"
 
     @classmethod
     def create_task(
         cls, 
         /, 
         *args, 
-        submit=run_thread, 
+        submit=run_as_thread, 
         **kwargs, 
     ) -> Self:
         return cls(download_iter(*args, **kwargs), submit=submit)
 
     @property
     def closed(self, /) -> bool:
         return self._state in ("CANCELED", "FAILED", "FINISHED")
```

### Comparing `python_115-0.0.5.1/p115/util/file.py` & `python_115-0.0.5.2/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/hash.py` & `python_115-0.0.5.2/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/ignore.py` & `python_115-0.0.5.2/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/iter.py` & `python_115-0.0.5.2/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/path.py` & `python_115-0.0.5.2/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/property.py` & `python_115-0.0.5.2/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/response.py` & `python_115-0.0.5.2/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/retry.py` & `python_115-0.0.5.2/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/text.py` & `python_115-0.0.5.2/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/p115/util/urlopen.py` & `python_115-0.0.5.2/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/pyproject.toml` & `python_115-0.0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.5.1"
+version = "0.0.5.2"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
@@ -30,14 +30,15 @@
 aiohttp = "*"
 cachetools = "*"
 ecdsa = "*"
 lz4 = "*"
 pycryptodome = "*"
 qrcode = "*"
 requests = "*"
+magnet2torrent = "*"
 yarl = "*"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_115-0.0.5.1/readme.md` & `python_115-0.0.5.2/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.1/PKG-INFO` & `python_115-0.0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -20,14 +20,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp
 Requires-Dist: cachetools
 Requires-Dist: ecdsa
 Requires-Dist: lz4
+Requires-Dist: magnet2torrent
 Requires-Dist: pycryptodome
 Requires-Dist: qrcode
 Requires-Dist: requests
 Requires-Dist: yarl
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 Description-Content-Type: text/markdown
```

