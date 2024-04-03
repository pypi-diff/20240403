# Comparing `tmp/PaifuLogger-0.3.9.tar.gz` & `tmp/PaifuLogger-0.3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaifuLogger-0.3.9.tar", last modified: Fri Mar 22 17:22:58 2024, max compression
+gzip compressed data, was "PaifuLogger-0.3.9.1.tar", last modified: Wed Apr  3 05:20:26 2024, max compression
```

## Comparing `PaifuLogger-0.3.9.tar` & `PaifuLogger-0.3.9.1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:22:58.136402 PaifuLogger-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-03-22 17:22:58.136402 PaifuLogger-0.3.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:22:58.136402 PaifuLogger-0.3.9/PaifuLogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-03-22 17:22:58.000000 PaifuLogger-0.3.9/PaifuLogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-22 17:22:58.000000 PaifuLogger-0.3.9/PaifuLogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:22:58.000000 PaifuLogger-0.3.9/PaifuLogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-22 17:22:58.000000 PaifuLogger-0.3.9/PaifuLogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 17:22:58.000000 PaifuLogger-0.3.9/PaifuLogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-22 17:22:58.000000 PaifuLogger-0.3.9/PaifuLogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:22:58.132403 PaifuLogger-0.3.9/paifulogger/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:22:58.136402 PaifuLogger-0.3.9/paifulogger/localizations/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/localizations/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/localizations/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/localizations/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/localizations/zh_tw.json
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/paifu_dl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:22:58.136402 PaifuLogger-0.3.9/paifulogger/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/Paifu.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/get_paifu.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/get_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/log_into_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/log_into_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/log_into_xlsx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:22:58.136402 PaifuLogger-0.3.9/paifulogger/src/mjlog2mjai/
--rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-03-22 17:22:50.000000 PaifuLogger-0.3.9/paifulogger/src/mjlog2mjai/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-22 17:22:50.000000 PaifuLogger-0.3.9/paifulogger/src/mjlog2mjai/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/url_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/paifulogger/src/url_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 17:22:58.136402 PaifuLogger-0.3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:22:58.136402 PaifuLogger-0.3.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-22 17:22:49.000000 PaifuLogger-0.3.9/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.085144 PaifuLogger-0.3.9.1/paifulogger/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/paifulogger/localizations/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/localizations/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/localizations/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/localizations/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/localizations/zh_tw.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/paifu_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/paifulogger/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/Paifu.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/get_paifu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/log_into_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/log_into_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/log_into_xlsx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/
+-rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/url_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/test/test.py
```

### Comparing `PaifuLogger-0.3.9/LICENSE` & `PaifuLogger-0.3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9/PKG-INFO` & `PaifuLogger-0.3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaifuLogger
-Version: 0.3.9
+Version: 0.3.9.1
 Summary: Logging tenhou paifu into excel or html file with some key information.
 Author-email: Jim137 <jim@mail.jim137.eu.org>
 License: MIT License
         
         Copyright (c) 2023 Jim137
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `PaifuLogger-0.3.9/PaifuLogger.egg-info/PKG-INFO` & `PaifuLogger-0.3.9.1/PaifuLogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaifuLogger
-Version: 0.3.9
+Version: 0.3.9.1
 Summary: Logging tenhou paifu into excel or html file with some key information.
 Author-email: Jim137 <jim@mail.jim137.eu.org>
 License: MIT License
         
         Copyright (c) 2023 Jim137
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `PaifuLogger-0.3.9/PaifuLogger.egg-info/SOURCES.txt` & `PaifuLogger-0.3.9.1/PaifuLogger.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 paifulogger/localizations/en.json
 paifulogger/localizations/ja.json
 paifulogger/localizations/zh.json
 paifulogger/localizations/zh_tw.json
 paifulogger/src/Paifu.py
 paifulogger/src/__init__.py
 paifulogger/src/get_paifu.py
-paifulogger/src/get_place.py
 paifulogger/src/i18n.py
 paifulogger/src/log_into_csv.py
 paifulogger/src/log_into_html.py
 paifulogger/src/log_into_xlsx.py
 paifulogger/src/url_log.py
-paifulogger/src/url_request_handler.py
 paifulogger/src/mjlog2mjai/parse.py
 paifulogger/src/mjlog2mjai/test.py
+test/__init__.py
 test/test.py
```

### Comparing `PaifuLogger-0.3.9/README.md` & `PaifuLogger-0.3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9/paifulogger/localizations/en.json` & `PaifuLogger-0.3.9.1/paifulogger/localizations/en.json`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9/paifulogger/localizations/ja.json` & `PaifuLogger-0.3.9.1/paifulogger/localizations/ja.json`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9/paifulogger/localizations/zh.json` & `PaifuLogger-0.3.9.1/paifulogger/localizations/zh.json`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9/paifulogger/localizations/zh_tw.json` & `PaifuLogger-0.3.9.1/paifulogger/localizations/zh_tw.json`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9/paifulogger/log.py` & `PaifuLogger-0.3.9.1/paifulogger/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import argparse
 import json
-from typing import Callable
 import urllib.request
 import re
 import os
 import sys
 import warnings
+from typing import Callable
 
 from pandas import HDFStore, DataFrame
 from platformdirs import user_data_dir
 
 from .src.get_paifu import get_paifu
-from .src.i18n import localized_str, local_str
+from .src.i18n import localized_str, LocalStr
 from .src.log_into_csv import log_into_csv
 from .src.log_into_xlsx import log_into_xlsx
 from .src.log_into_html import log_into_html
 from .src.url_log import url_log, check_duplicate
 
 
 url_reg = r"https?://tenhou\.net/\d/\?log=\d{10}gm-\w{4}-\w{4}-\w{8}&tw=\d"
@@ -49,15 +49,15 @@
     for format in formats:
         if os.path.exists(f"{output}/{paifu_str}.{format}"):
             os.remove(f"{output}/{paifu_str}.{format}")
             print(f"{paifu_str}.{format} has been removed.")
     return None
 
 
-def _get_lang(lang: str | None = None) -> local_str:
+def _get_lang(lang: str | None = None) -> LocalStr:
     """
     Get the localized string.
 
     If not given, use English.
     """
 
     if lang:
@@ -81,15 +81,17 @@
     else:
         _output = os.path.abspath("./")
     return _output
 
 
 def _get_urls(
     url: list[str] | None = None,
-    local_lang: local_str = local_str("en", os.path.dirname(os.path.abspath(__file__))),
+    local_lang: LocalStr = localized_str(
+        "en", os.path.dirname(os.path.abspath(__file__))
+    ),
     output: str = os.path.abspath("./"),
     remake: bool = False,
 ) -> list[str]:
     """
     Get urls from input or url.
 
     If remake, get urls from url_log.h5
@@ -142,15 +144,15 @@
         formats = format
     else:
         formats = ["csv"]
     return formats
 
 
 def _remake_log(
-    local_lang: local_str, output: str, formats: list[str], all_formats: bool = False
+    local_lang: LocalStr, output: str, formats: list[str], all_formats: bool = False
 ) -> None:
     """
     Remake the log file from url_log.h5 (past logging log), and remove old paifu files.
     """
 
     paifu_str3 = local_lang.paifu + "/" + local_lang.sanma + local_lang.paifu
     paifu_str4 = local_lang.paifu + "/" + local_lang.yonma + local_lang.paifu
@@ -191,44 +193,44 @@
             log_formats.append(log_into_csv)
     return log_formats
 
 
 def log_paifu(
     *urls: list[str] | str,
     log_formats: list[Callable] = [log_into_csv],
-    local_lang: local_str = local_str("en", os.path.dirname(os.path.abspath(__file__))),
+    local_lang: LocalStr = LocalStr("en", os.path.dirname(os.path.abspath(__file__))),
     output: str = os.path.abspath("./"),
     remake: bool = False,
     ignore_duplicated: bool = False,
     mjai: bool = False,
 ) -> int:
     """
     Log paifu files.
 
     Args:
         urls: list[str]
             The urls of the paifu files.
         log_formats: list
             The list of log functions.
-        local_lang: local_str
+        local_lang: LocalStr
             The localized string.
         output: str
             The output directory.
         remake: bool
             Remake the log file from url_log.h5.
         ignore_duplicated: bool
             Ignore duplicated urls.
         mjai: bool
             Output MJAI format paifu.
 
     Returns:
         int
     """
 
-    retCode = [0]
+    retCode = 0
     _urls: list[str] = []
     for url in urls:
         if isinstance(url, list):
             _urls.extend(url)
         else:
             _urls.append(url)
     for url in _urls:
@@ -244,25 +246,24 @@
             paifu = get_paifu(url, local_lang, output, mjai)
             for log_into_format in log_formats:
                 log_into_format(paifu, local_lang, output)
             if remake:
                 pass
             else:
                 url_log(url, local_lang, output)
-            retCode.append(0)
         except urllib.error.URLError:
             print(local_lang.hint_url, url)
-            retCode.append(1)
+            retCode = 1
         except OSError:
             print(local_lang.hint_url, url)
-            retCode.append(1)
+            retCode = 1
         except ValueError:
             print(local_lang.hint_tw, url)
-            retCode.append(1)
-    return max(retCode)
+            retCode = 1
+    return retCode
 
 
 def log(args: argparse.Namespace) -> int:
     """
     Parse the arguments and log paifu files.
     """
```

### Comparing `PaifuLogger-0.3.9/paifulogger/src/i18n.py` & `PaifuLogger-0.3.9.1/paifulogger/src/i18n.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 
-class local_str:
+class LocalStr:
     def __init__(self, lang: str = "en", main_path: str = "./"):
         self.lang = lang
         self.main_path = main_path
         pass
 
     def load_data(self, data):
         for key in data:
@@ -18,16 +18,16 @@
         "If the attribute is not loaded, return the value in English."
 
         with open(f"{self.main_path}/localizations/en.json") as f:
             data = json.load(f)
         return data[name]
 
 
-def localized_str(lang: str, main_path: str) -> local_str:
-    localized = local_str(lang, main_path)
+def localized_str(lang: str, main_path: str) -> LocalStr:
+    localized = LocalStr(lang, main_path)
     try:
         with open(f"{main_path}/localizations/{lang}.json", encoding="utf-8") as f:
             data = json.load(f)
             localized.load_data(data)
     except FileNotFoundError:
         with open(f"{main_path}/localizations/en.json") as f:
             data = json.load(f)
```

### Comparing `PaifuLogger-0.3.9/paifulogger/src/log_into_csv.py` & `PaifuLogger-0.3.9.1/paifulogger/src/log_into_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import csv
-from datetime import datetime
 import re
 import os.path
+from datetime import datetime
 
 import pandas as pd
 
-from .get_place import get_place
-from .i18n import local_str
+from .i18n import LocalStr
 from .Paifu import Paifu
 
 
-def log_into_csv(paifu: Paifu, local_lang: local_str, output: str):
+def log_into_csv(paifu: Paifu, local_lang: LocalStr, output: str):
     if paifu.player_num == 3:
         paifu_str = local_lang.sanma + local_lang.paifu
     else:
         paifu_str = local_lang.yonma + local_lang.paifu
     path = f"{output}/{local_lang.paifu}/{paifu_str}.csv"
     if os.path.isfile(path):
         csvfile = open(path, "a+", encoding="utf-8")
@@ -35,15 +34,15 @@
         df = pd.read_csv(path, index_col=0, encoding="utf-8")
     except pd.errors.EmptyDataError:
         df = pd.DataFrame(columns=["id", "date", "plc", "paifu", "preR"])
     writer.writerow(
         [
             df.shape[0],
             datetime.strptime(re.findall(r"\d{10}", paifu.url)[0], "%Y%m%d%H"),
-            get_place(paifu, paifu.ban),
+            paifu.get_place(paifu.ban),
             paifu.url,
             float(paifu.r[paifu.ban]),
         ]
     )
     print(
         "csv: "
         + local_lang.hint_record1
```

### Comparing `PaifuLogger-0.3.9/paifulogger/src/log_into_html.py` & `PaifuLogger-0.3.9.1/paifulogger/src/log_into_html.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from datetime import datetime
 import io
 import re
+from datetime import datetime
 
 import pandas as pd
 
-from .get_place import get_place
-from .i18n import local_str
+from .i18n import LocalStr
 from .Paifu import Paifu
 
 
-def create_html(html_str, paifu_str, local_lang: local_str):
+def create_html(html_str, paifu_str, local_lang: LocalStr):
     html_str += f"""<!DOCTYPE html>
     <html lang={local_lang.lang}>
     <head>
         <meta charset="utf-8">
         <title>{paifu_str}</title>
         <style>
             table {{
@@ -42,29 +41,29 @@
                 </tr>
             </thead>
             <tbody>
     """
     return html_str
 
 
-def log_into_table(html_str, paifu: Paifu, local_lang: local_str):
+def log_into_table(html_str, paifu: Paifu, local_lang: LocalStr):
     time_str = datetime.strptime(re.findall(r"\d{10}", paifu.url)[0], "%Y%m%d%H")
     html_str += f"""
                 <tr>
                     <td>{time_str}</td>
-                    <td>{get_place(paifu, paifu.ban)}</td>
+                    <td>{paifu.get_place(paifu.ban)}</td>
                     <td><a href="{paifu.url}">{paifu.url}</a></td>
                     <td><textarea id="persisted-text"></textarea></td>
                     <td>{float(paifu.r[paifu.ban])}</td>
                 </tr>
     """
     return html_str
 
 
-def average_plc(html_str, local_lang: local_str):
+def average_plc(html_str, local_lang: LocalStr):
     html_p = (
         html_str
         + """
             </tbody>
         </table>
     </body>
     </html>
@@ -72,15 +71,15 @@
     )
     wrapper = io.StringIO(html_p)
     df = pd.read_html(wrapper)[0]
     avg_plc = df[f"{local_lang.plc}"].mean()
     return avg_plc
 
 
-def end_of_table(html_str, avg_plc, local_lang: local_str):
+def end_of_table(html_str, avg_plc, local_lang: LocalStr):
     html_str += (
         f"""
             </tbody>
         </table>
         <p>{local_lang.avg_plc} = {avg_plc}</p>
         """
         + """
@@ -103,15 +102,15 @@
 
 
 def clear_end(html_str):
     html_str = html_str.split("</table>")[0]
     return html_str
 
 
-def log_into_html(paifu: Paifu, local_lang: local_str, output: str):
+def log_into_html(paifu: Paifu, local_lang: LocalStr, output: str):
     if paifu.player_num == 3:
         paifu_str = local_lang.sanma + local_lang.paifu
     else:
         paifu_str = local_lang.yonma + local_lang.paifu
     path = f"{output}/{local_lang.paifu}/{paifu_str}.html"
     try:
         with open(path, "r", encoding="utf-8") as f:
```

### Comparing `PaifuLogger-0.3.9/paifulogger/src/log_into_xlsx.py` & `PaifuLogger-0.3.9.1/paifulogger/src/log_into_xlsx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
+import re
 from datetime import datetime
 from typing import cast
-import re
 
 import openpyxl as xl
 from openpyxl.worksheet.worksheet import Worksheet
 
-from .get_place import get_place
-from .i18n import local_str
+from .i18n import LocalStr
 from .Paifu import Paifu
 
 
-def log_into_xlsx(paifu: Paifu, local_lang: local_str, output: str):
+def log_into_xlsx(paifu: Paifu, local_lang: LocalStr, output: str):
     try:
         if paifu.player_num == 3:
             paifu_str = local_lang.sanma + local_lang.paifu
         else:
             paifu_str = local_lang.yonma + local_lang.paifu
         path = f"{output}/{local_lang.paifu}/{paifu_str}.xlsx"
         wb = xl.load_workbook(path)
@@ -34,15 +33,15 @@
         )
         sheet.column_dimensions["A"].width = 20
         sheet.column_dimensions["C"].width = 71
         sheet.column_dimensions["E"].width = local_lang.excelE
     sheet.append(
         [
             datetime.strptime(re.findall(r"\d{10}", paifu.url)[0], "%Y%m%d%H"),
-            get_place(paifu, paifu.ban),
+            paifu.get_place(paifu.ban),
             paifu.url,
             "",
             float(paifu.r[paifu.ban]),
         ]
     )
     sheet["C" + str(sheet.max_row)].style = "Hyperlink"
     sheet.append([local_lang.avg_plc, "=average(B2:B" + str(sheet.max_row) + ")"])
```

### Comparing `PaifuLogger-0.3.9/paifulogger/src/mjlog2mjai/parse.py` & `PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/parse.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9/paifulogger/src/mjlog2mjai/test.py` & `PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/test.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9/paifulogger/src/url_log.py` & `PaifuLogger-0.3.9.1/paifulogger/src/url_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 This module provides functionality to save URLs to a log file and check if a URL is duplicated in the log.
 
 Log File:
     The module uses an HDF5 file format (url_log.h5) to store URLs. The log file is created automatically when
     you log the first URL.
 
 Functions:
-    - url_log(url, local_lang: local_str, output: str) -> None:
+    - url_log(url, local_lang: LocalStr, output: str) -> None:
         Logs the given URL to the log file.
 
-    - check_duplicate(url, local_lang: local_str, output: str) -> bool:
+    - check_duplicate(url, local_lang: LocalStr, output: str) -> bool:
         Checks if the given URL already exists in the log file.
 
 """
 
 import os
 
 import pandas as pd
 
-from .i18n import local_str
+from .i18n import LocalStr
 
 
-def check_duplicate(url, local_lang: local_str, output: str) -> bool:
+def check_duplicate(url, local_lang: LocalStr, output: str) -> bool:
     path = f"{output}/{local_lang.paifu}"
     if not os.path.isdir(path):
         os.makedirs(path)
     store = pd.HDFStore(f"{path}/url_log.h5")
     if "url" not in store:
         store["url"] = pd.DataFrame(columns=["url"])
     duplicated = url.split("//")[1] in store["url"]["url"].values
     store.close()
     return duplicated
 
 
-def url_log(url, local_lang: local_str, output: str) -> None:
+def url_log(url, local_lang: LocalStr, output: str) -> None:
     path = f"{output}/{local_lang.paifu}"
     if not os.path.isdir(path):
         os.makedirs(path)
     store = pd.HDFStore(f"{path}/url_log.h5")
     if "url" not in store:
         store["url"] = pd.DataFrame(columns=["url"])
     if url.split("//")[1] in store["url"]["url"].values:
```

### Comparing `PaifuLogger-0.3.9/pyproject.toml` & `PaifuLogger-0.3.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PaifuLogger"
-version = "0.3.9"
+version = "0.3.9.1"
 description = "Logging tenhou paifu into excel or html file with some key information."
 readme = "README.md"
 authors = [{ name = "Jim137", email = "jim@mail.jim137.eu.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
```

### Comparing `PaifuLogger-0.3.9/test/test.py` & `PaifuLogger-0.3.9.1/test/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,26 +18,26 @@
     "version",
     "mjai",
     "ignore-duplicated",
 ]
 
 
 class Test(unittest.TestCase):
-    def test0(self):
+    def test_0(self):
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.version = True
 
-        self.assertRaises(Exception, log.log(args))
+        self.assertEqual(log.log(args), 0)
 
-    def test1(self):
+    def test_1(self):
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.url = [
@@ -49,17 +49,17 @@
             "https://tenhou.net/0/?log=2023050200gm-0099-0000-50c65fbf&tw=2",
             "http://tenhou.net/0/?log=2023050419gm-0099-0000-b3111c7e&tw=0",
         ]
         args.all_formats = True
         args.ignore_duplicated = True
         args.output = "./test/"
 
-        self.assertRaises(Exception, log.log(args))
+        self.assertEqual(log.log(args), 0)
 
-    def test2(self):
+    def test_2(self):
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.url = [
@@ -72,38 +72,38 @@
             "http://tenhou.net/0/?log=2023050419gm-0099-0000-b3111c7e&tw=0",
         ]
         args.all_formats = True
         args.ignore_duplicated = True
         args.output = "./test/"
         args.lang = "zh_tw"
 
-        self.assertRaises(Exception, log.log(args))
+        self.assertEqual(log.log(args), 0)
 
-    def test3(self):
+    def test_3(self):
         urls = [
             # yonma tests
             "https://tenhou.net/3/?log=2022052501gm-00c1-0000-f71e7910&tw=1",
             "https://tenhou.net/0/?log=2023051123gm-0001-0000-b3720f99&tw=2",
             "http://tenhou.net/0/?log=2023051216gm-0001-0000-5fd022cc&tw=1",
             # sanma tests
             "https://tenhou.net/0/?log=2023050200gm-0099-0000-50c65fbf&tw=2",
             "http://tenhou.net/0/?log=2023050419gm-0099-0000-b3111c7e&tw=0",
         ]
 
-        self.assertRaises(Exception, paifu_dl.paifu_dl(urls, output="./test/"))
+        self.assertEqual(paifu_dl.paifu_dl(urls, output="./test/"), 0)
 
-    def test4(self):
+    def test_4(self):
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.all_formats = True
         args.output = "./test/"
         args.remake = True
 
-        self.assertRaises(Exception, log.log(args))
+        self.assertEqual(log.log(args), 0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

