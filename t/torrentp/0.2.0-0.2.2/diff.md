# Comparing `tmp/torrentp-0.2.0.tar.gz` & `tmp/torrentp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrentp-0.2.0.tar", last modified: Mon Apr  1 12:25:38 2024, max compression
+gzip compressed data, was "torrentp-0.2.2.tar", last modified: Wed Apr  3 08:30:19 2024, max compression
```

## Comparing `torrentp-0.2.0.tar` & `torrentp-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:25:38.857336 torrentp-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    12179 2024-04-01 12:25:35.000000 torrentp-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-01 12:25:38.857336 torrentp-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-01 12:25:35.000000 torrentp-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 12:25:38.857336 torrentp-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-01 12:25:35.000000 torrentp-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:25:38.857336 torrentp-0.2.0/torrentp/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-01 12:25:35.000000 torrentp-0.2.0/torrentp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-01 12:25:35.000000 torrentp-0.2.0/torrentp/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-01 12:25:35.000000 torrentp-0.2.0/torrentp/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-01 12:25:35.000000 torrentp-0.2.0/torrentp/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-01 12:25:35.000000 torrentp-0.2.0/torrentp/torrent_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-01 12:25:35.000000 torrentp-0.2.0/torrentp/torrent_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:25:38.857336 torrentp-0.2.0/torrentp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-01 12:25:38.000000 torrentp-0.2.0/torrentp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-01 12:25:38.000000 torrentp-0.2.0/torrentp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:25:38.000000 torrentp-0.2.0/torrentp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 12:25:38.000000 torrentp-0.2.0/torrentp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 12:25:38.000000 torrentp-0.2.0/torrentp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 12:25:38.000000 torrentp-0.2.0/torrentp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:30:19.390355 torrentp-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12179 2024-04-03 08:30:15.000000 torrentp-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-03 08:30:19.390355 torrentp-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-03 08:30:15.000000 torrentp-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:30:19.390355 torrentp-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-03 08:30:15.000000 torrentp-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:30:19.390355 torrentp-0.2.2/torrentp/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 08:30:15.000000 torrentp-0.2.2/torrentp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-03 08:30:15.000000 torrentp-0.2.2/torrentp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-03 08:30:15.000000 torrentp-0.2.2/torrentp/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-03 08:30:15.000000 torrentp-0.2.2/torrentp/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-03 08:30:15.000000 torrentp-0.2.2/torrentp/torrent_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-03 08:30:15.000000 torrentp-0.2.2/torrentp/torrent_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:30:19.390355 torrentp-0.2.2/torrentp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-03 08:30:19.000000 torrentp-0.2.2/torrentp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 08:30:19.000000 torrentp-0.2.2/torrentp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:30:19.000000 torrentp-0.2.2/torrentp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 08:30:19.000000 torrentp-0.2.2/torrentp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:30:19.000000 torrentp-0.2.2/torrentp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 08:30:19.000000 torrentp-0.2.2/torrentp.egg-info/top_level.txt
```

### Comparing `torrentp-0.2.0/LICENSE` & `torrentp-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torrentp-0.2.0/PKG-INFO` & `torrentp-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrentp
-Version: 0.2.0
+Version: 0.2.2
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `torrentp-0.2.0/README.md` & `torrentp-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `torrentp-0.2.0/setup.py` & `torrentp-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `torrentp-0.2.0/torrentp/__init__.py` & `torrentp-0.2.2/torrentp/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 A great wrapped library for downloading from torrent.
 """
 from .torrent_downloader import TorrentDownloader
 from .torrent_info import TorrentInfo
 from .downloader import Downloader
 from .session import Session
 
-__version__ = "0.2.0"
+__version__ = "0.2.2"
 __author__ = 'Nima Akbarzade'
 __author_email__ = "iw4p@protonmail.com"
 __license__ = "BSD 2-clause"
 __url__ = "https://github.com/iw4p/torrentp"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/torrentp"
```

### Comparing `torrentp-0.2.0/torrentp/cli.py` & `torrentp-0.2.2/torrentp/cli.py`

 * *Files identical despite different names*

### Comparing `torrentp-0.2.0/torrentp/downloader.py` & `torrentp-0.2.2/torrentp/downloader.py`

 * *Files identical despite different names*

### Comparing `torrentp-0.2.0/torrentp/session.py` & `torrentp-0.2.2/torrentp/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class Session:
-    def __init__(self, libtorrent):
+    def __init__(self, libtorrent, port='6881'):
         self._user_agent = 'python client v0.1'
         self._listen_interfaces = '0.0.0.0'
-        self._port = '6881'
+        self._port = port
         self._download_rate_limit = 0
         self._upload_rate_limit = 0
         self._lt = libtorrent
         self._session = None
 
     def create_session(self):
         self._session = self._lt.session({'listen_interfaces':f'{self._listen_interfaces}:{self._port}'})
```

### Comparing `torrentp-0.2.0/torrentp/torrent_downloader.py` & `torrentp-0.2.2/torrentp/torrent_downloader.py`

 * *Files identical despite different names*

### Comparing `torrentp-0.2.0/torrentp.egg-info/PKG-INFO` & `torrentp-0.2.2/torrentp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrentp
-Version: 0.2.0
+Version: 0.2.2
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

