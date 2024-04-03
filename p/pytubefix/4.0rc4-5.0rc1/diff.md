# Comparing `tmp/pytubefix-4.0rc4.tar.gz` & `tmp/pytubefix-5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-4.0rc4.tar", last modified: Mon Apr  1 12:29:01 2024, max compression
+gzip compressed data, was "pytubefix-5.0rc1.tar", last modified: Wed Apr  3 02:57:19 2024, max compression
```

## Comparing `pytubefix-4.0rc4.tar` & `pytubefix-5.0rc1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 12:29:01.173731 pytubefix-4.0rc4/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1101 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/LICENSE
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       18 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/MANIFEST.in
--rw-r--r--   0 estoque   (1000) estoque   (1000)     4506 2024-04-01 12:29:01.173731 pytubefix-4.0rc4/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3174 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/README.md
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1524 2024-04-01 12:28:16.000000 pytubefix-4.0rc4/pyproject.toml
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 12:29:01.165731 pytubefix-4.0rc4/pytubefix/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      614 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    17933 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6595 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/captions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1121 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/chapters.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    22543 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/cipher.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    17032 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      786 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/colors.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 12:29:01.165731 pytubefix-4.0rc4/pytubefix/contrib/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        0 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/contrib/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    19995 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/contrib/channel.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    14600 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/contrib/playlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    11048 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/contrib/search.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     4115 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18093 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/extract.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     9944 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/helpers.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16837 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/innertube.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     4311 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/itags.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1483 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/metadata.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      478 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/monostate.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     5960 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/parser.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    14289 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/query.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     8817 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/request.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    14818 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/pytubefix/streams.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-01 12:28:05.000000 pytubefix-4.0rc4/pytubefix/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 12:29:01.173731 pytubefix-4.0rc4/pytubefix.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     4506 2024-04-01 12:29:01.000000 pytubefix-4.0rc4/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1007 2024-04-01 12:29:01.000000 pytubefix-4.0rc4/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-01 12:29:01.000000 pytubefix-4.0rc4/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       49 2024-04-01 12:29:01.000000 pytubefix-4.0rc4/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       10 2024-04-01 12:29:01.000000 pytubefix-4.0rc4/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-01 12:29:01.173731 pytubefix-4.0rc4/setup.cfg
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 12:29:01.169731 pytubefix-4.0rc4/tests/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6579 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_captions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2742 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_cipher.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18009 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3626 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2963 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_extract.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     5060 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_helpers.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      279 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_itags.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1939 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_main.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      501 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_metadata.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1412 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_parser.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6172 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_query.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1882 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_request.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    13661 2024-04-01 11:17:12.000000 pytubefix-4.0rc4/tests/test_streams.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-03 02:57:19.024347 pytubefix-5.0rc1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/LICENSE
+-rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/MANIFEST.in
+-rw-r--r--   0 juan      (1000) juan      (1000)     4506 2024-04-03 02:57:19.024347 pytubefix-5.0rc1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3174 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-04-03 02:54:31.000000 pytubefix-5.0rc1/pyproject.toml
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-03 02:57:19.020346 pytubefix-5.0rc1/pytubefix/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    20098 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6595 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1121 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/chapters.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17032 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      786 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/colors.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-03 02:57:19.020346 pytubefix-5.0rc1/pytubefix/contrib/
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/contrib/channel.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    11048 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/contrib/search.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4115 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18319 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     9944 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17414 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/innertube.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4311 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/jsinterp.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/monostate.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5960 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14289 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     8817 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14818 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/pytubefix/streams.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-04-03 02:53:43.000000 pytubefix-5.0rc1/pytubefix/version.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-03 02:57:19.024347 pytubefix-5.0rc1/pytubefix.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     4506 2024-04-03 02:57:19.000000 pytubefix-5.0rc1/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-04-03 02:57:19.000000 pytubefix-5.0rc1/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-03 02:57:19.000000 pytubefix-5.0rc1/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-04-03 02:57:19.000000 pytubefix-5.0rc1/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-04-03 02:57:19.000000 pytubefix-5.0rc1/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-03 02:57:19.024347 pytubefix-5.0rc1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-03 02:57:19.024347 pytubefix-5.0rc1/tests/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-04-03 02:52:51.000000 pytubefix-5.0rc1/tests/test_streams.py
```

### Comparing `pytubefix-4.0rc4/LICENSE` & `pytubefix-5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/PKG-INFO` & `pytubefix-5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 4.0rc4
+Version: 5.0rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 4.0rc4 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.0rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-4.0rc4/README.md` & `pytubefix-5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pyproject.toml` & `pytubefix-5.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "4.0-rc4"
+version = "5.0-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-4.0rc4/pytubefix/__init__.py` & `pytubefix-5.0rc1/pytubefix/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/__main__.py` & `pytubefix-5.0rc1/pytubefix/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 The problem domain of the :class:`YouTube <YouTube> class focuses almost
 exclusively on the developer interface. Pytubefix offloads the heavy lifting to
 smaller peripheral modules and functions.
 
 """
 
-
 import logging
 from typing import Any, Callable, Dict, List, Optional
 
 import pytubefix
 import pytubefix.exceptions as exceptions
 from pytubefix import extract, request
 from pytubefix import Stream, StreamQuery
@@ -46,26 +45,34 @@
 logger = logging.getLogger(__name__)
 
 
 class YouTube:
     """Core developer interface for pytubefix."""
 
     def __init__(
-        self,
-        url: str,
-        on_progress_callback: Optional[Callable[[Any, bytes, int], None]] = None,
-        on_complete_callback: Optional[Callable[[Any, Optional[str]], None]] = None,
-        proxies: Dict[str, str] = None,
-        use_oauth: bool = False,
-        allow_oauth_cache: bool = True
+            self,
+            url: str,
+            client: str = 'ANDROID',
+            on_progress_callback: Optional[Callable[[Any, bytes, int], None]] = None,
+            on_complete_callback: Optional[Callable[[Any, Optional[str]], None]] = None,
+            proxies: Dict[str, str] = None,
+            use_oauth: bool = False,
+            allow_oauth_cache: bool = True
     ):
         """Construct a :class:`YouTube <YouTube>`.
 
         :param str url:
             A valid YouTube watch URL.
+        :param str client:
+            (Optional) A YouTube client,
+            Available:
+                WEB, WEB_EMBED, WEB_MUSIC, WEB_CREATOR,
+                ANDROID, ANDROID_EMBED, ANDROID_MUSIC, ANDROID_CREATOR,
+                IOS, IOS_EMBED, IOS_MUSIC, IOS_CREATOR,
+                MWEB, TV_EMBED.
         :param func on_progress_callback:
             (Optional) User defined callback function for stream download
             progress events.
         :param func on_complete_callback:
             (Optional) User defined callback function for stream download
             complete events.
         :param dict proxies:
@@ -94,14 +101,18 @@
 
         # video_id part of /watch?v=<video_id>
         self.video_id = extract.video_id(url)
 
         self.watch_url = f"https://youtube.com/watch?v={self.video_id}"
         self.embed_url = f"https://www.youtube.com/embed/{self.video_id}"
 
+        self.client = client
+
+        self._signature_timestamp: dict = {}
+
         # Shared between all instances of `Stream` (Borg pattern).
         self.stream_monostate = Monostate(
             on_progress=on_progress_callback, on_complete=on_complete_callback
         )
 
         if proxies:
             install_proxy(proxies)
@@ -176,17 +187,36 @@
         self._initial_data = extract.initial_data(self.watch_html)
         return self._initial_data
 
     @property
     def streaming_data(self):
         """Return streamingData from video info."""
         if 'streamingData' in self.vid_info:
+
+            invalid_id_list = ['aQvGIIdgFDM']  # List of YouTube error video IDs
+            video_id = self.vid_info['videoDetails']['videoId']
+
+            if video_id in invalid_id_list:
+                logger.warning(
+                    f'The {self.client} client did not get a valid response, trying to use the WEB client.'
+                )
+                logger.warning(
+                    f'Video ID: {video_id}'
+                )
+                logger.warning(
+                    'Please open an issue at '
+                    'https://github.com/JuanBindez/pytubefix/issues '
+                    'and provide this log output.'
+                )
+
+                self.try_another_client()
+
             return self.vid_info['streamingData']
         else:
-            self.bypass_age_gate()
+            self.try_another_client()
             return self.vid_info['streamingData']
 
     @property
     def fmt_streams(self):
         """Returns a list of streams if they have been initialized.
 
         If the streams have not been initialized, finds all relevant
@@ -233,64 +263,94 @@
         otherwise does nothing.
         """
         status, messages = extract.playability_status(self.watch_html)
 
         for reason in messages:
             if status == 'UNPLAYABLE':
                 if reason == (
-                    'Join this channel to get access to members-only content '
-                    'like this video, and other exclusive perks.'
+                        'Join this channel to get access to members-only content '
+                        'like this video, and other exclusive perks.'
                 ):
                     raise exceptions.MembersOnly(video_id=self.video_id)
                 elif reason == 'This live stream recording is not available.':
                     raise exceptions.RecordingUnavailable(video_id=self.video_id)
                 else:
                     raise exceptions.VideoUnavailable(video_id=self.video_id)
             elif status == 'LOGIN_REQUIRED':
                 if reason == (
-                    'This is a private video. '
-                    'Please sign in to verify that you may see it.'
+                        'This is a private video. '
+                        'Please sign in to verify that you may see it.'
                 ):
                     raise exceptions.VideoPrivate(video_id=self.video_id)
             elif status == 'ERROR':
                 if reason == 'Video unavailable':
                     raise exceptions.VideoUnavailable(video_id=self.video_id)
             elif status == 'LIVE_STREAM':
                 raise exceptions.LiveStreamError(video_id=self.video_id)
 
     @property
+    def signature_timestamp(self) -> dict:
+        """WEB clients need to be signed with a signature timestamp.
+
+        The signature is found inside the player's base.js.
+
+        :rtype: Dict
+        """
+        if not self._signature_timestamp:
+            self._signature_timestamp = {
+                'playbackContext': {
+                    'contentPlaybackContext': {
+                        'signatureTimestamp': extract.signature_timestamp(self.js)
+                    }
+                }
+            }
+        return self._signature_timestamp
+
+    @property
     def vid_info(self):
         """Parse the raw vid info and return the parsed result.
 
         :rtype: Dict[Any, Any]
         """
         if self._vid_info:
             return self._vid_info
 
-        innertube = InnerTube(use_oauth=self.use_oauth, allow_cache=self.allow_oauth_cache)
+        innertube = InnerTube(client=self.client, use_oauth=self.use_oauth, allow_cache=self.allow_oauth_cache)
+        if innertube.require_js_player:
+            innertube.innertube_context.update(self.signature_timestamp)
 
         innertube_response = innertube.player(self.video_id)
         self._vid_info = innertube_response
         return self._vid_info
 
-    def bypass_age_gate(self):
-        """Attempt to update the vid_info by bypassing the age gate."""
+    def try_another_client(self):
+        """If the default client does not have streamData, try using another client.
+
+        We use the WEB client, as it is the most stable so far.
+
+        Previously, this function was used to bypass age gate by trying to use EMBED clients,
+        but it is no longer effective.
+
+        """
         innertube = InnerTube(
-            client='ANDROID_EMBED',
+            client='WEB',
             use_oauth=self.use_oauth,
             allow_cache=self.allow_oauth_cache
         )
+
+        if innertube.require_js_player:
+            innertube.innertube_context.update(self.signature_timestamp)
+
         innertube_response = innertube.player(self.video_id)
 
         playability_status = innertube_response['playabilityStatus'].get('status', None)
 
         # If we still can't access the video, raise an exception
-        # (tier 3 age restriction)
         if playability_status == 'UNPLAYABLE':
-            raise exceptions.AgeRestrictedError(self.video_id)
+            raise exceptions.VideoUnavailable(self.video_id)
 
         self._vid_info = innertube_response
 
     @property
     def caption_tracks(self) -> List[pytubefix.Caption]:
         """Get a list of :class:`Caption <Caption>`.
 
@@ -390,15 +450,14 @@
 
         :rtype: str
         """
         self._author = self.vid_info.get("videoDetails", {}).get(
             "author", "unknown"
         )
 
-
         if self._title:
             return self._title.replace('/', '\\')
 
         try:
             self._title = self.vid_info['videoDetails']['title']
         except KeyError:
             # Check_availability will raise the correct exception in most cases
@@ -406,17 +465,17 @@
             self.check_availability()
             raise exceptions.PytubeFixError(
                 (
                     f'Exception while accessing title of {self.watch_url}. '
                     'Please file a bug report at https://github.com/JuanBindez/pytubefix'
                 )
             )
-        #print(self.vid_info['videoDetails'])
+        # print(self.vid_info['videoDetails'])
         return self._title.replace('/', '\\')
-    
+
     @title.setter
     def title(self, value):
         """Sets the title value."""
         self._title = value
 
     @property
     def description(self) -> str:
```

### Comparing `pytubefix-4.0rc4/pytubefix/captions.py` & `pytubefix-5.0rc1/pytubefix/captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/chapters.py` & `pytubefix-5.0rc1/pytubefix/chapters.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/cli.py` & `pytubefix-5.0rc1/pytubefix/cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/colors.py` & `pytubefix-5.0rc1/pytubefix/colors.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/contrib/channel.py` & `pytubefix-5.0rc1/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/contrib/playlist.py` & `pytubefix-5.0rc1/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/contrib/search.py` & `pytubefix-5.0rc1/pytubefix/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/exceptions.py` & `pytubefix-5.0rc1/pytubefix/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/extract.py` & `pytubefix-5.0rc1/pytubefix/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from pytubefix.cipher import Cipher
 from pytubefix.exceptions import HTMLParseError, LiveStreamError, RegexMatchError
 from pytubefix.helpers import regex_search
 from pytubefix.metadata import YouTubeMetadata
 from pytubefix.parser import parse_for_object, parse_for_all_objects
 
-
 logger = logging.getLogger(__name__)
 
 
 def publish_date(watch_html: str):
     """Extract publish date and return it as a datetime object
     :param str watch_html:
         The html contents of the watch page.
@@ -31,14 +30,15 @@
             watch_html
         )
         if result:
             return datetime.fromisoformat(result.group(0))
     except AttributeError:
         return None
 
+
 def recording_available(watch_html):
     """Check if live stream recording is available.
 
     :param str watch_html:
         The html contents of the watch page.
     :rtype: bool
     :returns:
@@ -111,14 +111,18 @@
         if 'reason' in status_dict:
             return status_dict['status'], [status_dict['reason']]
         if 'messages' in status_dict:
             return status_dict['status'], status_dict['messages']
     return None, [None]
 
 
+def signature_timestamp(js: str) -> str:
+    return regex_search(r"signatureTimestamp:(\d*)", js, group=1)
+
+
 def video_id(url: str) -> str:
     """Extract the ``video_id`` from a YouTube url.
 
     This function supports the following patterns:
 
     - :samp:`https://youtube.com/watch?v={video_id}`
     - :samp:`https://youtube.com/embed/{video_id}`
@@ -411,52 +415,56 @@
     cipher = Cipher(js=js)
 
     for i, stream in enumerate(stream_manifest):
         try:
             url: str = stream["url"]
         except KeyError:
             live_stream = (
-                vid_info.get("playabilityStatus", {},)
+                vid_info.get("playabilityStatus", {}, )
                 .get("liveStreamability")
             )
             if live_stream:
                 raise LiveStreamError("UNKNOWN")
+
+        parsed_url = urlparse(url)
+
+        # Convert query params off url to dict
+        query_params = parse_qs(urlparse(url).query)
+        query_params = {
+            k: v[0] for k, v in query_params.items()
+        }
+
         # 403 Forbidden fix.
         if "signature" in url or (
-            "s" not in stream and ("&sig=" in url or "&lsig=" in url)
+                "s" not in stream and ("&sig=" in url or "&lsig=" in url)
         ):
             # For certain videos, YouTube will just provide them pre-signed, in
             # which case there's no real magic to download them and we can skip
             # the whole signature descrambling entirely.
             logger.debug("signature found, skip decipher")
-            continue
 
-        signature = cipher.get_signature(ciphered_signature=stream["s"])
+        else:
+            signature = cipher.get_signature(ciphered_signature=stream["s"])
 
-        logger.debug(
-            "finished descrambling signature for itag=%s", stream["itag"]
-        )
-        parsed_url = urlparse(url)
+            logger.debug(
+                "finished descrambling signature for itag=%s", stream["itag"]
+            )
 
-        # Convert query params off url to dict
-        query_params = parse_qs(urlparse(url).query)
-        query_params = {
-            k: v[0] for k,v in query_params.items()
-        }
-        query_params['sig'] = signature
-        if 'ratebypass' not in query_params.keys():
-            # Cipher n to get the updated value
+            query_params['sig'] = signature
+
+        if 'n' in query_params.keys():
+            # For WEB-based clients, YouTube sends an "n" parameter that throttles download speed.
+            # To decipher the value of "n", we must interpret the player's JavaScript.
 
-            initial_n = list(query_params['n'])
-            new_n = cipher.calculate_n(initial_n)
+            initial_n = query_params['n']
+            new_n = cipher.get_throttling(initial_n)
             query_params['n'] = new_n
 
         url = f'{parsed_url.scheme}://{parsed_url.netloc}{parsed_url.path}?{urlencode(query_params)}'  # noqa:E501
 
-        # 403 forbidden fix
         stream_manifest[i]["url"] = url
 
 
 def apply_descrambler(stream_data: Dict) -> None:
     """Apply various in-place transforms to YouTube's media stream data.
 
     Creates a ``list`` of dictionaries by string splitting on commas, then
```

### Comparing `pytubefix-4.0rc4/pytubefix/helpers.py` & `pytubefix-5.0rc1/pytubefix/helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/innertube.py` & `pytubefix-5.0rc1/pytubefix/innertube.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,16 @@
                     'clientVersion': '2.20200720.00.02'
                 }
             }
         },
         'header': {
             'User-Agent': 'Mozilla/5.0'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': True
     },
     'ANDROID': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'ANDROID',
                     'clientVersion': '19.08.35',
@@ -53,30 +54,32 @@
                 }
             },
             "params": "CgIIAdgDAQ%3D%3D"
         },
         'header': {
             'User-Agent': 'com.google.android.youtube/',
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': False
     },
     'IOS': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'IOS',
                     'clientVersion': '19.08.35',
                     'deviceModel': 'iPhone14,3'
                 }
             }
         },
         'header': {
             'User-Agent': 'com.google.ios.youtube/'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': False
     },
 
     'WEB_EMBED': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'WEB_EMBEDDED_PLAYER',
@@ -84,15 +87,16 @@
                     'clientScreen': 'EMBED'
                 }
             }
         },
         'header': {
             'User-Agent': 'Mozilla/5.0'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': True
     },
     'ANDROID_EMBED': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'ANDROID_EMBEDDED_PLAYER',
                     'clientVersion': '19.08.35',
@@ -100,150 +104,160 @@
                     'androidSdkVersion': 30,
                 }
             }
         },
         'header': {
             'User-Agent': 'com.google.android.youtube/'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': False
     },
     'IOS_EMBED': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'IOS_MESSAGES_EXTENSION',
                     'clientVersion': '19.08.35',
                     'deviceModel': 'iPhone14,3'
                 }
             }
         },
         'header': {
             'User-Agent': 'com.google.ios.youtube/'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': False
     },
 
     'WEB_MUSIC': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'WEB_REMIX',
                     'clientVersion': '1.20220727.01.00',
                 }
             }
         },
         'header': {
             'User-Agent': 'Mozilla/5.0'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': True
     },
     'ANDROID_MUSIC': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'ANDROID_MUSIC',
                     'clientVersion': '6.40.52',
                     'androidSdkVersion': 30
                 }
             }
         },
         'header': {
             'User-Agent': 'com.google.android.apps.youtube.music/'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': False
     },
     'IOS_MUSIC': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'IOS_MUSIC',
                     'clientVersion': '6.41',
                     'deviceModel': 'iPhone14,3'
                 }
             }
         },
         'header': {
             'User-Agent': 'com.google.ios.youtubemusic/'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': False
     },
 
     'WEB_CREATOR': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'WEB_CREATOR',
                     'clientVersion': '1.20220726.00.00',
                 }
             }
         },
         'header': {
             'User-Agent': 'Mozilla/5.0'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': True
     },
     'ANDROID_CREATOR': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'ANDROID_CREATOR',
                     'clientVersion': '22.30.100',
                     'androidSdkVersion': 30,
                 }
             }
         },
         'header': {
             'User-Agent': 'com.google.android.apps.youtube.creator/',
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': False
     },
     'IOS_CREATOR': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'IOS_CREATOR',
                     'clientVersion': '22.33.101',
                     'deviceModel': 'iPhone14,3',
                 }
             }
         },
         'header': {
             'User-Agent': 'com.google.ios.ytcreator/'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': False
     },
 
     'MWEB': {
         'inertube_context': {
             'context': {
                 'client': {
                     'clientName': 'MWEB',
                     'clientVersion': '2.20220801.00.00',
                 }
             }
         },
         'header': {
             'User-Agent': 'Mozilla/5.0'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': True
     },
 
     'TV_EMBED': {
         'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'TVHTML5_SIMPLY_EMBEDDED_PLAYER',
                     'clientVersion': '2.0',
                 }
             }
         },
         'header': {
             'User-Agent': 'Mozilla/5.0'
         },
-        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
+        'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
+        'require_js_player': True
     },
 }
 _token_timeout = 1800
 _cache_dir = pathlib.Path(__file__).parent.resolve() / '__cache__'
 _token_file = os.path.join(_cache_dir, 'tokens.json')
 
 
@@ -260,14 +274,15 @@
             Whether or not to authenticate to YouTube.
         :param bool allow_cache:
             Allows caching of oauth tokens on the machine.
         """
         self.innertube_context = _default_clients[client]['innertube_context']
         self.header = _default_clients[client]['header']
         self.api_key = _default_clients[client]['api_key']
+        self.require_js_player = _default_clients[client]['require_js_player']
         self.access_token = None
         self.refresh_token = None
         self.use_oauth = use_oauth
         self.allow_cache = allow_cache
 
         # Stored as epoch time
         self.expires = None
```

### Comparing `pytubefix-4.0rc4/pytubefix/itags.py` & `pytubefix-5.0rc1/pytubefix/itags.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/metadata.py` & `pytubefix-5.0rc1/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/parser.py` & `pytubefix-5.0rc1/pytubefix/parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/query.py` & `pytubefix-5.0rc1/pytubefix/query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/request.py` & `pytubefix-5.0rc1/pytubefix/request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix/streams.py` & `pytubefix-5.0rc1/pytubefix/streams.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/pytubefix.egg-info/PKG-INFO` & `pytubefix-5.0rc1/pytubefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 4.0rc4
+Version: 5.0rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 4.0rc4 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.0rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-4.0rc4/pytubefix.egg-info/SOURCES.txt` & `pytubefix-5.0rc1/pytubefix.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pytubefix/cli.py
 pytubefix/colors.py
 pytubefix/exceptions.py
 pytubefix/extract.py
 pytubefix/helpers.py
 pytubefix/innertube.py
 pytubefix/itags.py
+pytubefix/jsinterp.py
 pytubefix/metadata.py
 pytubefix/monostate.py
 pytubefix/parser.py
 pytubefix/query.py
 pytubefix/request.py
 pytubefix/streams.py
 pytubefix/version.py
```

### Comparing `pytubefix-4.0rc4/tests/test_captions.py` & `pytubefix-5.0rc1/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_cli.py` & `pytubefix-5.0rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_exceptions.py` & `pytubefix-5.0rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_extract.py` & `pytubefix-5.0rc1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_helpers.py` & `pytubefix-5.0rc1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_main.py` & `pytubefix-5.0rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_parser.py` & `pytubefix-5.0rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_query.py` & `pytubefix-5.0rc1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_request.py` & `pytubefix-5.0rc1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-4.0rc4/tests/test_streams.py` & `pytubefix-5.0rc1/tests/test_streams.py`

 * *Files identical despite different names*

