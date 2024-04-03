# Comparing `tmp/shellserver-0.1.0.tar.gz` & `tmp/shellserver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellserver-0.1.0.tar", last modified: Sun Oct  8 06:16:46 2023, max compression
+gzip compressed data, was "shellserver-0.1.1.tar", last modified: Wed Apr  3 03:30:45 2024, max compression
```

## Comparing `shellserver-0.1.0.tar` & `shellserver-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-10-08 06:16:46.341529 shellserver-0.1.0/
--rw-rw-rw-   0        0        0      942 2023-10-08 06:16:46.341529 shellserver-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1313 2023-10-08 06:06:20.000000 shellserver-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-08 06:16:46.341529 shellserver-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-08 06:16:46.262971 shellserver-0.1.0/shellserver/
--rw-rw-rw-   0        0        0      250 2023-04-07 07:52:16.000000 shellserver-0.1.0/shellserver/__init__.py
--rw-rw-rw-   0        0        0      558 2023-08-30 07:10:45.000000 shellserver-0.1.0/shellserver/__main__.py
--rw-rw-rw-   0        0        0     1926 2023-09-22 07:46:45.000000 shellserver-0.1.0/shellserver/cli.py
-drwxrwxrwx   0        0        0        0 2023-10-08 06:16:46.341529 shellserver-0.1.0/shellserver/gitstatus/
--rw-rw-rw-   0        0        0        0 2023-04-03 05:05:55.000000 shellserver-0.1.0/shellserver/gitstatus/__init__.py
--rw-rw-rw-   0        0        0    16715 2023-10-08 03:44:41.000000 shellserver-0.1.0/shellserver/gitstatus/base.py
--rw-rw-rw-   0        0        0    26386 2023-10-08 03:51:08.000000 shellserver-0.1.0/shellserver/gitstatus/high.py
--rw-rw-rw-   0        0        0     4772 2023-10-08 06:03:09.000000 shellserver-0.1.0/shellserver/gitstatus/interface.py
--rw-rw-rw-   0        0        0     4659 2023-10-08 03:44:41.000000 shellserver-0.1.0/shellserver/gitstatus/packs.py
--rw-rw-rw-   0        0        0     1279 2023-10-08 03:52:20.000000 shellserver-0.1.0/shellserver/gitstatus/plugins.py
--rw-rw-rw-   0        0        0     2595 2023-09-17 02:16:58.000000 shellserver-0.1.0/shellserver/gitstatus/utils.py
--rw-rw-rw-   0        0        0    15102 2023-10-08 05:46:46.000000 shellserver-0.1.0/shellserver/server.py
--rw-rw-rw-   0        0        0     9081 2023-09-22 06:07:22.000000 shellserver-0.1.0/shellserver/style.py
--rw-rw-rw-   0        0        0    14437 2023-10-08 03:44:41.000000 shellserver-0.1.0/shellserver/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-08 06:16:46.310282 shellserver-0.1.0/shellserver.egg-info/
--rw-rw-rw-   0        0        0      942 2023-10-08 06:16:46.000000 shellserver-0.1.0/shellserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-10-08 06:16:46.000000 shellserver-0.1.0/shellserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-08 06:16:46.000000 shellserver-0.1.0/shellserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-10-08 06:16:46.000000 shellserver-0.1.0/shellserver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-10-08 06:16:46.000000 shellserver-0.1.0/shellserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-08 06:16:46.000000 shellserver-0.1.0/shellserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 03:30:45.791712 shellserver-0.1.1/
+-rw-rw-rw-   0        0        0      942 2024-04-03 03:30:45.791712 shellserver-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1379 2024-04-03 02:12:47.000000 shellserver-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 03:30:45.791712 shellserver-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 03:30:45.737304 shellserver-0.1.1/shellserver/
+-rw-rw-rw-   0        0        0      250 2023-04-07 07:52:16.000000 shellserver-0.1.1/shellserver/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-08-30 07:10:45.000000 shellserver-0.1.1/shellserver/__main__.py
+-rw-rw-rw-   0        0        0     1936 2023-10-08 06:35:42.000000 shellserver-0.1.1/shellserver/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:30:45.791712 shellserver-0.1.1/shellserver/gitstatus/
+-rw-rw-rw-   0        0        0        0 2023-04-03 05:05:55.000000 shellserver-0.1.1/shellserver/gitstatus/__init__.py
+-rw-rw-rw-   0        0        0    16797 2023-12-29 04:44:51.000000 shellserver-0.1.1/shellserver/gitstatus/base.py
+-rw-rw-rw-   0        0        0    26383 2023-12-15 02:54:59.000000 shellserver-0.1.1/shellserver/gitstatus/high.py
+-rw-rw-rw-   0        0        0     4772 2023-10-08 06:03:09.000000 shellserver-0.1.1/shellserver/gitstatus/interface.py
+-rw-rw-rw-   0        0        0     4667 2023-12-15 02:41:57.000000 shellserver-0.1.1/shellserver/gitstatus/packs.py
+-rw-rw-rw-   0        0        0     1296 2023-12-15 01:26:14.000000 shellserver-0.1.1/shellserver/gitstatus/plugins.py
+-rw-rw-rw-   0        0        0     2595 2023-12-15 01:19:25.000000 shellserver-0.1.1/shellserver/gitstatus/utils.py
+-rw-rw-rw-   0        0        0    15160 2024-04-02 04:05:59.000000 shellserver-0.1.1/shellserver/server.py
+-rw-rw-rw-   0        0        0     9081 2023-09-22 06:07:22.000000 shellserver-0.1.1/shellserver/style.py
+-rw-rw-rw-   0        0        0    14554 2024-04-02 23:27:28.000000 shellserver-0.1.1/shellserver/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:30:45.791712 shellserver-0.1.1/shellserver.egg-info/
+-rw-rw-rw-   0        0        0      942 2024-04-03 03:30:45.000000 shellserver-0.1.1/shellserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2024-04-03 03:30:45.000000 shellserver-0.1.1/shellserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 03:30:45.000000 shellserver-0.1.1/shellserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-04-03 03:30:45.000000 shellserver-0.1.1/shellserver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 03:30:45.000000 shellserver-0.1.1/shellserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 03:30:45.000000 shellserver-0.1.1/shellserver.egg-info/top_level.txt
```

### Comparing `shellserver-0.1.0/PKG-INFO` & `shellserver-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Server to aid shell navigation.
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
 License: MIT
 Project-URL: Home-page, https://github.com/HenriquedoVal/shellserver
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `shellserver-0.1.0/pyproject.toml` & `shellserver-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'shellserver'
-version = '0.1.0'
+version = '0.1.1'
 authors = [
   {name = 'Henrique do Val'},
   {email = 'henrique.val@hotmail.com'}
 ]
 
 description = 'Server to aid shell navigation.'
 readme = {file = "README.md", content-type = 'text/markdown'}
@@ -35,15 +35,18 @@
 
 [project.urls]
 Home-page = "https://github.com/HenriquedoVal/shellserver"
 
 [project.scripts]
 shellserver = 'shellserver.cli:main'
 
-[project.optional-dependencies]
+[project.gui-scripts]
+shellserverw = 'shellserver.cli:main'
+
+# [project.optional-dependencies]
 # all = [
 #   "whatchdog>=3.2.1",
 #   "ssd_checker>=1.0.3",
 #   "pygit2>=1.11.1"
 # ]
 
 [tool.setuptools.packages.find]
```

### Comparing `shellserver-0.1.0/shellserver/__main__.py` & `shellserver-0.1.1/shellserver/__main__.py`

 * *Files identical despite different names*

### Comparing `shellserver-0.1.0/shellserver/cli.py` & `shellserver-0.1.1/shellserver/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 commands:
 
     run       Run the server.
     kill      Kill the server.
     sync      Clear useless entries and write cache to disk.
     clear     Delete the server cache.
-    dump      Dump the server cache.
+    dump      Dump the server cache to stdout.
 
 options:
   -h, --help  show this help message and exit'''
 )
 
 
 def run():
```

### Comparing `shellserver-0.1.0/shellserver/gitstatus/base.py` & `shellserver-0.1.1/shellserver/gitstatus/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hashlib
 import os
 import subprocess
 import zlib
 
 from . import packs
 from . import plugins
+from .plugins import HAS_SSD_CHECKER, DRIVE_SSD_MAP
 
 
 class IndexTooBigError(Exception):
     pass
 
 
 class Base(packs.Packs):
@@ -56,20 +57,20 @@
         """
         Sets `index_tracked` attribute.
         Modified and simpler version of gin.
         https://github.com/sbp/gin
         return: None.
         """
         max_entries = 1000
-        if plugins.HAS_SSD_CHECKER:
-            for drive in plugins.DRIVE_SSD_MAP:
+        if HAS_SSD_CHECKER:
+            for drive in DRIVE_SSD_MAP:
                 if self.git_dir.startswith(drive):
                     # if SSD: 2500 if HDD: 1000
                     max_entries = (
-                        2500 if plugins.DRIVE_SSD_MAP[drive] else 1000
+                        2500 if DRIVE_SSD_MAP[drive] else 1000
                     )
                     break
 
         index_path = os.path.join(self.git_dir, '.git/index')
         if not os.path.exists(index_path):
             self.index_tracked = {}
             return
@@ -85,28 +86,33 @@
 
                     ret.append(b)
 
             constant = f.read(4)
             version = int.from_bytes(f.read(4), 'big')
             if constant != b'DIRC' or version not in (2, 3):
                 self.index_tracked = {}
+                return
 
             entries = int.from_bytes(f.read(4), 'big')
+
+            if self.fallback and entries > max_entries:
+                raise IndexTooBigError
+
             res = {}
 
             for entry in range(entries):
                 f.read(8)
                 # converted to float to keep type consistence
                 mtime = float(int.from_bytes(f.read(4), 'big'))
                 mtime += int.from_bytes(f.read(4), 'big') / 1000000000
                 f.read(44)
 
                 flags = int.from_bytes(f.read(2), 'big')
                 namelen = flags & 0xfff
-                extended = flags & (0b0100_0000 << 8)
+                extended = flags & 16384  # 0b0100_0000 << 8
 
                 entrylen = 62
 
                 if extended:
                     f.read(2)
                     entrylen += 2
 
@@ -115,17 +121,14 @@
                     entrylen += namelen
                 else:
                     name = read_str_until(b'\x00')
                     entrylen += 1
 
                 res[name] = mtime
 
-                if self.fallback and len(res) > max_entries:
-                    raise IndexTooBigError
-
                 padlen = (8 - (entrylen % 8)) or 8
                 f.read(padlen)
 
         self.index_tracked = res
 
     def get_split_ignored(
         self, raw_ignored: list[str], prepend: None | str = None
@@ -182,17 +185,18 @@
         Gets the last commit's hash of a git repo by a packed perspective.
         return: str | None: String of the last commit hash, None if there's no
                             last commit packed.
         """
         info_refs = self.get_info_refs_content()
         last_commt_hash = None
 
+        target = f'refs/heads/{self.branch}'
         for line in info_refs:
             a, b = line.strip().split()
-            if b == f'refs/heads/{self.branch}':
+            if b == target:
                 last_commt_hash = a
                 break
 
         return last_commt_hash
 
     def get_last_commit_hash(self) -> str | None:
         """
@@ -390,16 +394,16 @@
 
         content = self.prev_read
 
         if not use_cr:
             content = content.replace(b'\r\n', b'\n', -1)
 
         size = len(content)
-        string = f"blob {size}\x00"
-        hash_ = hashlib.sha1(string.encode() + content).hexdigest()
+        preamble = f"blob {size}\x00"
+        hash_ = hashlib.sha1(preamble.encode() + content).hexdigest()
 
         return hash_
 
     def get_content_by_hash_loose(self, hash_: str) -> bytes | None:
         """
         Get the content of a loose file by its hash.
         param `hash`: The hash gotten from `get_hash_of_file` for files in repo
```

### Comparing `shellserver-0.1.0/shellserver/gitstatus/high.py` & `shellserver-0.1.1/shellserver/gitstatus/high.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Module for functions with high level of abstraction
 and/or complexity.
 """
 
 import ctypes
-import fnmatch
+from fnmatch import fnmatch
 import io
 import multiprocessing as mp
 import os
 import pickle
 import time
 
 from collections import deque
 from mmap import mmap
 from multiprocessing.shared_memory import SharedMemory
 from typing import Any
 
 from . import base
 from . import plugins
-from . import utils
+from .utils import (
+    PathMatchSpecW, DirEntryWrapper, DiscardOutput,
+    OVERLAPPED,
+    read_async
+)
 
 OS_CPU_COUNT = os.cpu_count() or 1
 n = '\n\n'
 
 
 class FallbackError(Exception):
     pass
@@ -53,30 +57,30 @@
             *,
             multiproc: bool = False,
             workers: int = OS_CPU_COUNT - 1,
             linear: bool = False,
             read_async: bool = True,
             fallback: bool = True,
             watchdog: bool = True,
-            output: io.TextIOWrapper | utils.DiscardOutput | None = None,
+            output: io.TextIOWrapper | DiscardOutput | None = None,
             _is_worker: bool = False,
             **kwargs,
     ) -> None:
 
         # config
         self.linear = linear
         self.read_async = read_async
         self.fallback = fallback
         self.watchdog = watchdog
 
-        self.output: io.TextIOWrapper | io.StringIO | utils.DiscardOutput
+        self.output: io.TextIOWrapper | io.StringIO | DiscardOutput
         if not isinstance(
             output, (io.TextIOWrapper, io.StringIO)
         ) or output is None:
-            self.output = utils.DiscardOutput()
+            self.output = DiscardOutput()
         else:
             self.output = output
 
         self.untracked = 0
         self.staged = 0
         self.modified = 0
         self.deleted = 0
@@ -86,15 +90,15 @@
 
         self.event_handlers: dict[str, EventHandler] = {}
         self.final_result_cache: dict[
             str, tuple[float | None, str | None]] = {}
         self.dirs_mtimes: dict[str, float] = {}
 
         self.files_readden: deque[
-            tuple[ctypes.Array[Any], utils.OVERLAPPED, float, str]
+            tuple[ctypes.Array[Any], OVERLAPPED, float, str]
         ] = deque()
 
         self.mp_main = multiproc
         self.multiproc = (multiproc and workers) or _is_worker
         self.raised_exception = False
 
         if not self.multiproc:
@@ -201,17 +205,17 @@
         self.staged = 0
         self.modified = 0
         self.deleted = 0
 
         if not self.multiproc:
             self.output.write(
                 'Entries classified: '
-                f'{utils.DirEntryWrapper.counter}\n'
+                f'{DirEntryWrapper.counter}\n'
             )
-        utils.DirEntryWrapper.counter = 0
+        DirEntryWrapper.counter = 0
 
         return status_string
 
     def load_balancer(
         self,
         dir_path: str,
         tree_hash: str,
@@ -289,15 +293,15 @@
             return
 
         for dir_entry in directory:
 
             if self.raised_exception:
                 break
 
-            file = utils.DirEntryWrapper(dir_entry, self.git_dir)
+            file = DirEntryWrapper(dir_entry, self.git_dir)
 
             # 100755(exe) is file
             if file.is_file():
                 if file.relpath in self.index_tracked:
                     self.handle_tracked_file(
                         file, tree_items_list, file.relpath
                     )
@@ -310,15 +314,15 @@
                 self.handle_dir(
                     file, fixed, relative, clean_fixed,
                     tracked_directories, tree_items_list
                 )
 
     def handle_dir(
         self,
-        file: utils.DirEntryWrapper,
+        file: DirEntryWrapper,
         fixed: list[str],
         relative: list[str],
         clean_fixed: list[str],
         tracked_directories: dict[str, str],
         tree_items_list: list[tuple[str, str, str]]
     ) -> None:
 
@@ -351,15 +355,15 @@
 
             if file_present:
                 self.output.write(f'Untracked: {file.relpath}\n')
                 self.untracked += 1
 
     def handle_tracked_file(
         self,
-        file: utils.DirEntryWrapper,
+        file: DirEntryWrapper,
         tree_items_list: list[tuple[str, str, str]],
         relpath: str
     ) -> None:
         # get the item or it's staged
         for item in tree_items_list:
             if item[2] == file.name:
                 break
@@ -378,15 +382,15 @@
         if st_mtime != mtime:
             self.output.write(f'Modified: {relpath}\n')
             self.modified += 1
             return
 
         file_hash_in_tree = item[1]
         if not self.linear and self.read_async:
-            buffer, overl = utils.read_async(file.path, st_size)
+            buffer, overl = read_async(file.path, st_size)
             self.files_readden.append(
                 (buffer, overl, st_size, file_hash_in_tree)
             )
             return
 
         # use_cr: interchangeably switch the use of crlf
         file_hash = self.get_hash_of_file(file.path, self.use_cr)
@@ -428,19 +432,19 @@
             return 0, False
 
         sub_dir = []
         for file in directory:
             if file.name == '.git':
                 directory.close()
                 return 0, False
-            sub_dir.append(utils.DirEntryWrapper(file, self.git_dir))
+            sub_dir.append(DirEntryWrapper(file, self.git_dir))
 
         file_present = False
         staged_flag = 0
-        marked_dirs_to_classify: list[utils.DirEntryWrapper] = []
+        marked_dirs_to_classify: list[DirEntryWrapper] = []
         for sub_file in sub_dir:
 
             if sub_file.relpath in self.index_tracked:
                 self.output.write(f'Staged: {sub_file.relpath}\n')
                 self.staged += 1
                 staged_flag += 1
                 file_present = True
@@ -558,50 +562,50 @@
 
         self.objects_cache[tree_hash] = tree_items_list
 
         return tree_items_list
 
     def is_ignored(
         self,
-        file: utils.DirEntryWrapper,
+        file: DirEntryWrapper,
         fixed: list[str],
         relative: list[str]
     ) -> bool:
         is_dir = file.is_dir()
 
         for pattern in relative:
 
             if pattern[-1] == '/' and not is_dir:
                 continue
 
             name = file.name + '/' if pattern[-1] == '/' else file.name
 
             # `PathMatchSpecW` doesn't deal with '[a-z]' but will be used if
             # pattern doesn't have this because it is way faster
-            if '[' in pattern and fnmatch.fnmatch(name, pattern):
+            if '[' in pattern and fnmatch(name, pattern):
                 return True
 
-            elif utils.PathMatchSpecW(name, pattern):
+            elif PathMatchSpecW(name, pattern):
                 return True
 
         for pattern in fixed:
 
             if pattern[-1] == '/' and not is_dir:
                 continue
 
             relpath = (
                 file.relpath + '/'
                 if pattern[-1] == '/'
                 else file.relpath
             )
 
-            if '[' in pattern and fnmatch.fnmatch(relpath, pattern):
+            if '[' in pattern and fnmatch(relpath, pattern):
                 return True
 
-            if utils.PathMatchSpecW(relpath, pattern):
+            if PathMatchSpecW(relpath, pattern):
                 return True
 
         return False
 
     def get_cached_result(self) -> int | str | None:
         cache = self.final_result_cache.get(self.git_dir)
         mtime = self.dirs_mtimes.get(self.git_dir)
```

### Comparing `shellserver-0.1.0/shellserver/gitstatus/interface.py` & `shellserver-0.1.1/shellserver/gitstatus/interface.py`

 * *Files identical despite different names*

### Comparing `shellserver-0.1.0/shellserver/gitstatus/packs.py` & `shellserver-0.1.1/shellserver/gitstatus/packs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Low level operations on packfiles.
 """
 
 import os
 import zlib
-import io
+from io import BytesIO, BufferedReader
 from collections import deque
 
 
 class Packs:
     # {'path': (mtime, buffer)}
-    bytes_io_cache: dict[str, tuple[float, io.BytesIO]] = {}
+    bytes_io_cache: dict[str, tuple[float, BytesIO]] = {}
     # [(mtime, path, stream)]
     streams_to_transform_in_bytes_io: deque[
-        tuple[float, str, io.BufferedReader]
+        tuple[float, str, BufferedReader]
     ] = deque()
 
     __slots__ = ()
 
     def search_idx(
             self,
             idx_path: str,
@@ -115,15 +115,15 @@
 
     def get_idx_of_pack(self, pack: str) -> str:
         """
         return pack.removesuffix('pack') + 'idx'
         """
         return pack.removesuffix('pack') + 'idx'
 
-    def _get_buffer(self, path: str) -> io.BytesIO | io.BufferedReader:
+    def _get_buffer(self, path: str) -> BytesIO | BufferedReader:
         mtime = os.stat(path, follow_symlinks=False).st_mtime
         cache = self.bytes_io_cache.get(path)
         if cache and cache[0] == mtime:
             c = cache[1]
             c.seek(0)
             return c
 
@@ -131,21 +131,21 @@
         self.streams_to_transform_in_bytes_io.append((mtime, path, raw))
         return raw
 
     def _write_buffer(self) -> None:
         while self.streams_to_transform_in_bytes_io:
             mtime, path, raw = self.streams_to_transform_in_bytes_io.pop()
             raw.seek(0)
-            c = io.BytesIO(raw.read())
+            c = BytesIO(raw.read())
             raw.close()
 
             self.bytes_io_cache[path] = mtime, c
 
     def get_offset(
-        self, file: io.BytesIO | io.BufferedReader,
+        self, file: BytesIO | BufferedReader,
         total_files: int,
         target: int
     ) -> int:
         file.seek(
             1032
             + 20 * total_files  # jump layer2
             + 4 * total_files  # jump layer3
```

### Comparing `shellserver-0.1.0/shellserver/gitstatus/plugins.py` & `shellserver-0.1.1/shellserver/gitstatus/plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-__all__ = [
+__all__ = (
     'HAS_PYGIT2',
     'HAS_SSD_CHECKER',
     'DRIVE_SSD_MAP',
     'pygit2',
     'FileSystemEvent'
-]
+)
 
 try:
     import pygit2
     HAS_PYGIT2 = True
 except ImportError:
     HAS_PYGIT2 = False
 
     class pygit2:  # dummy
         Repository = None
 
 try:
+    DRIVE_SSD_MAP: dict[str, bool] = {}
+
     from ssd_checker import is_ssd  # fail fast
 
     # pywin32 is dep of ssd_checker
     from pythoncom import CoInitialize
 
     from ctypes import windll
-    import string
-    import threading as th
-
-    DRIVE_SSD_MAP: dict[str, bool] = {}
+    from string import ascii_uppercase
+    from threading import Thread
 
     def populate(letter: str) -> None:
         CoInitialize()
         DRIVE_SSD_MAP[letter] = is_ssd(letter)
 
     bitmask = windll.kernel32.GetLogicalDrives()
-    for letter in string.ascii_uppercase:
+    for letter in ascii_uppercase:
         if bitmask & 1:
             letter = letter + ':'
-            th.Thread(
+            Thread(
                 target=populate, args=(letter,), daemon=True
             ).start()
         bitmask >>= 1
 
     HAS_SSD_CHECKER = True
 
 except ImportError:
```

### Comparing `shellserver-0.1.0/shellserver/gitstatus/utils.py` & `shellserver-0.1.1/shellserver/gitstatus/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import ctypes
 import ctypes.wintypes
 from typing import Any
 
-__all__ = ['DiscardOutput', 'DirEntryWrapper', 'read_async']
+__all__ = ('DiscardOutput', 'DirEntryWrapper', 'read_async')
 
 FILE_FLAG_OVERLAPPED = 0x40000000
 GENERIC_READ = 0x80000000
 OPEN_EXISTING = 3
 
 
 class DiscardOutput:
@@ -15,21 +15,21 @@
         return
 
     def flush(self) -> None:
         return
 
 
 class OVERLAPPED(ctypes.Structure):
-    _fields_ = [
+    _fields_ = (
         ('Internal', ctypes.c_ulong),
         ('InternalHigh', ctypes.c_ulong),
         ('Offset', ctypes.c_ulong),
         ('OffsetHigh', ctypes.c_ulong),
         ('hEvent', ctypes.c_void_p),
-    ]
+    )
 
 
 class DirEntryWrapper:
     counter = 0
     # os.DirEntry is a final class, can't be subclassed
     __slots__ = 'entry', 'name', 'path', 'relpath'
```

### Comparing `shellserver-0.1.0/shellserver/server.py` & `shellserver-0.1.1/shellserver/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.exes_with_version = {}
         self.exes_without_version = []
         self.exes_to_search = [
             'node', 'g++', 'gcc', 'lua', 'pwsh', 'java', 'rustc', 'dotnet'
         ]
 
         # can't get all executables versions through the api
-        self.exes_to_search_with_winapi = ('pwsh', 'node', 'java')
+        self.exes_to_search_with_winapi = ('pwsh', 'node', 'java', 'dotnet')
 
         self.map_suffix = {
             'node': '.js',
             'g++': '.cpp',
             'gcc': '.c',
             'lua': '.lua',
             'pwsh': ('.ps1', '.psd1', '.psm1'),
@@ -154,17 +154,18 @@
                 if conf[0] == '_':
                     continue
                 res.write(f'{conf};{val}\n')
 
             self.dispatcher.send_through(self.sock, res.getvalue(), addr)
 
         elif entry == 'Sync':
-            self.cache._clear()
+            if self.cache.clear():
+                self.dispatcher.set_update()
             self.cache.sort()
-            self.cache._save()
+            self.cache.save()
 
         elif entry == 'Kill':
             self.cache.finish()
             return 1
 
     def get_abs_by_ref(self, entry: str, addr: tuple[Any]) -> None:
         result = self.cache.get(entry)
```

### Comparing `shellserver-0.1.0/shellserver/style.py` & `shellserver-0.1.1/shellserver/style.py`

 * *Files identical despite different names*

### Comparing `shellserver-0.1.0/shellserver/utils.py` & `shellserver-0.1.1/shellserver/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,16 +60,14 @@
         ("dwFileSubtype", wintypes.DWORD),
         ("dwFileDateMS", wintypes.DWORD),
         ("dwFileDateLS", wintypes.DWORD),
     ]
 
 
 def get_file_version(filename: str) -> str | None:
-
-    # Get the file version information
     dwHandle = wintypes.DWORD()
     dwLen = version_dll.GetFileVersionInfoSizeW(
         filename, ctypes.byref(dwHandle)
     )
     if not dwLen:
         return
 
@@ -96,37 +94,37 @@
         dwFileVersionLS >> 16,
         # dwFileVersionLS & 0xFFFF
     )
     return ".".join(map(str, dwFileVersion))
 
 
 class DirCache:
-    __slots__ = 'dirs', '_save_on_exit', 'completions', 'manual_functions'
+    __slots__ = 'dirs', 'completions', '_save_on_exit'
 
-    # dirs = list[list[precedence: int, abs_path: str, short_path: str]]
     def __init__(self):
-        self._save_on_exit = False  # New paths were added to cache?
+        self._save_on_exit = False
 
+        # dirs = list[list[precedence: int, abs_path: str, short_path: str]]
         if os.path.exists(CACHE_PATH):
             with open(CACHE_PATH, 'rb') as in_file:
                 self.dirs = pickle.load(in_file)
-            self._clear()
+            self.clear()
         else:
             self.dirs = []
 
             os.makedirs(APP_HOME, exist_ok=True)
 
             # Need to create file or cache will never save
             # if it doesn't exist.
             # Need to put something there or server might break
             # when pickle tries to read an empty file.
             with open(CACHE_PATH, 'wb') as in_file:
                 pickle.dump([], in_file)
 
-        self.completions = ';'.join(item[2] for item in self.dirs)
+        self._update_completions()
 
     def manual_manage(self, opt: str, arg: str) -> bool:
         """"""
         func = (self.add, self.delete)[int(opt in ('Del', 'DRf'))]
 
         args_to_func = [arg]
         if func == self.delete:
@@ -153,16 +151,15 @@
 
         if not items_to_delete:
             return False
 
         for i in items_to_delete:
             self.dirs.remove(i)
 
-        # will be slow with 1000 entries?
-        self.completions = ';'.join([item[2] for item in self.dirs])
+        self._update_completions()
         self.set_save_on_exit()
 
         return True
 
     def add(self, path: str) -> bool:
         "Return if the cache changed."
 
@@ -190,14 +187,31 @@
 
         self.dirs.append([0, path, path_ref])
 
         self.set_save_on_exit()
 
         return True
 
+    def clear(self) -> bool:
+        """Returns if there was any change to the cache."""
+        aux = [
+            item for item in self.dirs
+            if not os.path.exists(item[1])
+        ]
+
+        for item in aux:
+            self.dirs.remove(item)
+
+        if aux:
+            self.set_save_on_exit()
+            self._update_completions()
+            return True
+
+        return False
+
     def get(self, path_ref: str) -> str:
         for item in self.dirs:
             if item[2] == path_ref:
                 return item[1]
         return ''
 
     def update_by_full_path(self, full_path: str) -> None:
@@ -205,21 +219,21 @@
         for idx, item in enumerate(self.dirs):
             if item[1] == full_path:
                 break
         else:
             return
 
         # set every entry precedence with same last path name to zero
-        last_path_name = item[2]
-        idxs_with_same_last_path_name = [
-            other_idx for other_idx, i in enumerate(self.dirs)
-            if i[2] == last_path_name
+        path_ref = item[2]
+        idxs_with_same_path_ref = [
+            other_idx for other_idx, item in enumerate(self.dirs)
+            if item[2] == path_ref
         ]
 
-        for other_idx in idxs_with_same_last_path_name:
+        for other_idx in idxs_with_same_path_ref:
             self.dirs[other_idx][0] = 0
 
         # update only given full_path to one
         self.dirs[idx][0] = 1
 
         self.set_save_on_exit()
 
@@ -227,39 +241,32 @@
         # just want to set save_on_exit if it is false to start thread
         # that will capture WM_SAVE_YOURSELF
         if not self._save_on_exit:
             self._save_on_exit = True
             threading.Thread(target=self._signal_cap, daemon=True).start()
 
     def finish(self):
-        self._clear()
-        self._save()
+        self.clear()
+        self.save()
 
     def sort(self) -> None:
         self.dirs.sort(key=lambda x: x[0], reverse=True)
 
-    def _save(self) -> None:
+    def save(self) -> None:
         # if there were calls to clear the cache during this runtime
         if not os.path.exists(CACHE_PATH):
             return
         if self._save_on_exit:
             with open(CACHE_PATH, 'wb') as out:
                 pickle.dump(self.dirs, out, protocol=5)
 
-    def _clear(self) -> None:
-        aux = [
-            item for item in self.dirs
-            if not os.path.exists(item[1])
-        ]
-
-        if aux:
-            self.set_save_on_exit()
+    def _update_completions(self) -> None:
+        # will be slow with 1000 entries?
+        self.completions = ';'.join(item[2] for item in self.dirs)
 
-        for item in aux:
-            self.dirs.remove(item)
 
     def _signal_cap(self):
         import tkinter as tk
 
         def finish():
             self.finish()
             raise SystemExit
@@ -274,50 +281,51 @@
     """
     This class will hold the specifics convertions
     necessary to each shell, apply them and send
     data through socket.
     """
 
     __slots__ = (
-        'addr_shell', 'addr_update', 'shell_func', 'buf_size', 'update_counter'
+        'addr_shell', 'addr_update', 'shell_func', 'buf_size', '_update_counter'
     )
 
     def __init__(self, buf_size: int):
         # afaik, udp header might be 20 or 40 bytes but none of these work
         # must be missing something because no value around it works
         self.buf_size = buf_size - 2000
         self.addr_shell = {}
         self.addr_update = {}
         self.shell_func = {'pwsh': self._pwsh_func}
-        self.update_counter = 0
+        self._update_counter = 0
 
     def set_update(self) -> None:
-        self.update_counter += 1
+        self._update_counter += 1
 
     def register(self, addr: int, shell: str):
         self.addr_shell.update({addr: shell})
-        self.addr_update.update({addr: self.update_counter})
+        self.addr_update.update({addr: self._update_counter})
 
     def send_through(
         self, sock, data: str, addr: tuple[str, int],
         *, prepare=True, send_update=False
     ):
 
         shell = self.addr_shell.get(addr, 'pwsh')
         func = self.shell_func.get(shell)
 
         if send_update:
             addr_update_counter = self.addr_update.get(
-                addr, self.update_counter
+                addr, self._update_counter
             )
 
-            up = '1' if addr_update_counter < self.update_counter else '0'
-
-            if up == '1':
-                self.addr_update[addr] = self.update_counter
+            if addr_update_counter < self._update_counter:
+                up = '1'
+                self.addr_update[addr] = self._update_counter
+            else:
+                up = '0'
 
             data = up + data
 
         if prepare and func is not None:
             data = func(data)
 
         while len(data) > self.buf_size:
```

### Comparing `shellserver-0.1.0/shellserver.egg-info/PKG-INFO` & `shellserver-0.1.1/shellserver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Server to aid shell navigation.
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
 License: MIT
 Project-URL: Home-page, https://github.com/HenriquedoVal/shellserver
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `shellserver-0.1.0/shellserver.egg-info/SOURCES.txt` & `shellserver-0.1.1/shellserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

