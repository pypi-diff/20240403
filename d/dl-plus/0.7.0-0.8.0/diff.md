# Comparing `tmp/dl-plus-0.7.0.tar.gz` & `tmp/dl-plus-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl-plus-0.7.0.tar", last modified: Wed Jan 24 09:53:44 2024, max compression
+gzip compressed data, was "dl-plus-0.8.0.tar", last modified: Wed Apr  3 13:38:23 2024, max compression
```

## Comparing `dl-plus-0.7.0.tar` & `dl-plus-0.8.0.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.414878 dl-plus-0.7.0/
--rw-rw-r--   0 def       (1000) def       (1000)     1090 2024-01-24 09:52:12.000000 dl-plus-0.7.0/LICENSE
--rw-r--r--   0 def       (1000) def       (1000)     3903 2024-01-24 09:53:44.414878 dl-plus-0.7.0/PKG-INFO
--rw-rw-r--   0 def       (1000) def       (1000)     2994 2023-07-27 10:36:26.000000 dl-plus-0.7.0/README.md
--rw-rw-r--   0 def       (1000) def       (1000)     2331 2024-01-24 09:48:35.000000 dl-plus-0.7.0/pyproject.toml
--rw-rw-r--   0 def       (1000) def       (1000)       38 2024-01-24 09:53:44.414878 dl-plus-0.7.0/setup.cfg
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.410878 dl-plus-0.7.0/src/
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.410878 dl-plus-0.7.0/src/dl_plus/
--rw-rw-r--   0 def       (1000) def       (1000)       38 2022-04-23 13:15:25.000000 dl-plus-0.7.0/src/dl_plus/__main__.py
--rw-rw-r--   0 def       (1000) def       (1000)     3705 2024-01-14 10:58:28.000000 dl-plus-0.7.0/src/dl_plus/backend.py
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.414878 dl-plus-0.7.0/src/dl_plus/cli/
--rw-rw-r--   0 def       (1000) def       (1000)       43 2022-04-23 13:15:25.000000 dl-plus-0.7.0/src/dl_plus/cli/__init__.py
--rw-rw-r--   0 def       (1000) def       (1000)     1931 2023-07-03 14:42:02.000000 dl-plus-0.7.0/src/dl_plus/cli/args.py
--rw-rw-r--   0 def       (1000) def       (1000)     4021 2023-07-28 12:39:45.000000 dl-plus-0.7.0/src/dl_plus/cli/cli.py
--rw-rw-r--   0 def       (1000) def       (1000)     2773 2023-07-25 09:51:10.000000 dl-plus-0.7.0/src/dl_plus/cli/command.py
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.414878 dl-plus-0.7.0/src/dl_plus/cli/commands/
--rw-rw-r--   0 def       (1000) def       (1000)      372 2023-07-03 13:49:40.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/__init__.py
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.414878 dl-plus-0.7.0/src/dl_plus/cli/commands/backend/
--rw-rw-r--   0 def       (1000) def       (1000)      384 2023-07-03 14:49:37.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/backend/__init__.py
--rw-rw-r--   0 def       (1000) def       (1000)      437 2023-07-03 14:56:11.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/backend/base.py
--rw-rw-r--   0 def       (1000) def       (1000)      852 2023-07-03 15:07:49.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/backend/info.py
--rw-rw-r--   0 def       (1000) def       (1000)     1019 2023-07-03 15:24:37.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/backend/install.py
--rw-rw-r--   0 def       (1000) def       (1000)     1090 2023-07-03 15:26:11.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/backend/update.py
--rw-rw-r--   0 def       (1000) def       (1000)     8248 2023-07-27 16:43:19.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/base.py
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.414878 dl-plus-0.7.0/src/dl_plus/cli/commands/extractor/
--rw-rw-r--   0 def       (1000) def       (1000)      332 2023-07-01 13:45:38.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/extractor/__init__.py
--rw-rw-r--   0 def       (1000) def       (1000)     1059 2023-07-03 15:12:18.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/extractor/base.py
--rw-rw-r--   0 def       (1000) def       (1000)      987 2023-07-03 12:11:53.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/extractor/install.py
--rw-rw-r--   0 def       (1000) def       (1000)      524 2023-07-03 12:11:48.000000 dl-plus-0.7.0/src/dl_plus/cli/commands/extractor/update.py
--rw-rw-r--   0 def       (1000) def       (1000)     8294 2024-01-14 11:20:11.000000 dl-plus-0.7.0/src/dl_plus/config.py
--rw-rw-r--   0 def       (1000) def       (1000)       65 2024-01-24 09:52:44.000000 dl-plus-0.7.0/src/dl_plus/const.py
--rw-rw-r--   0 def       (1000) def       (1000)     2039 2024-01-14 10:58:48.000000 dl-plus-0.7.0/src/dl_plus/core.py
--rw-rw-r--   0 def       (1000) def       (1000)      765 2023-10-31 16:03:37.000000 dl-plus-0.7.0/src/dl_plus/deprecated.py
--rw-rw-r--   0 def       (1000) def       (1000)      564 2022-04-23 13:15:25.000000 dl-plus-0.7.0/src/dl_plus/exceptions.py
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.414878 dl-plus-0.7.0/src/dl_plus/extractor/
--rw-rw-r--   0 def       (1000) def       (1000)      413 2023-07-25 09:52:48.000000 dl-plus-0.7.0/src/dl_plus/extractor/__init__.py
--rw-rw-r--   0 def       (1000) def       (1000)     1532 2023-07-24 13:29:10.000000 dl-plus-0.7.0/src/dl_plus/extractor/extractor.py
--rw-rw-r--   0 def       (1000) def       (1000)     2116 2022-04-23 13:15:25.000000 dl-plus-0.7.0/src/dl_plus/extractor/machinery.py
--rw-rw-r--   0 def       (1000) def       (1000)     3134 2022-04-23 13:15:25.000000 dl-plus-0.7.0/src/dl_plus/extractor/peqn.py
--rw-rw-r--   0 def       (1000) def       (1000)     5817 2022-04-23 13:15:25.000000 dl-plus-0.7.0/src/dl_plus/extractor/plugin.py
--rw-rw-r--   0 def       (1000) def       (1000)     3819 2023-07-01 13:45:38.000000 dl-plus-0.7.0/src/dl_plus/pypi.py
--rw-rw-r--   0 def       (1000) def       (1000)      276 2022-04-23 13:15:25.000000 dl-plus-0.7.0/src/dl_plus/utils.py
--rw-rw-r--   0 def       (1000) def       (1000)     6114 2023-07-02 11:13:30.000000 dl-plus-0.7.0/src/dl_plus/ytdl.py
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.414878 dl-plus-0.7.0/src/dl_plus.egg-info/
--rw-r--r--   0 def       (1000) def       (1000)     3903 2024-01-24 09:53:44.000000 dl-plus-0.7.0/src/dl_plus.egg-info/PKG-INFO
--rw-rw-r--   0 def       (1000) def       (1000)     1217 2024-01-24 09:53:44.000000 dl-plus-0.7.0/src/dl_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 def       (1000) def       (1000)        1 2024-01-24 09:53:44.000000 dl-plus-0.7.0/src/dl_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 def       (1000) def       (1000)       45 2024-01-24 09:53:44.000000 dl-plus-0.7.0/src/dl_plus.egg-info/entry_points.txt
--rw-rw-r--   0 def       (1000) def       (1000)        1 2024-01-24 09:53:44.000000 dl-plus-0.7.0/src/dl_plus.egg-info/not-zip-safe
--rw-rw-r--   0 def       (1000) def       (1000)        8 2024-01-24 09:53:44.000000 dl-plus-0.7.0/src/dl_plus.egg-info/top_level.txt
-drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-01-24 09:53:44.414878 dl-plus-0.7.0/tests/
--rw-rw-r--   0 def       (1000) def       (1000)      402 2023-07-01 14:25:07.000000 dl-plus-0.7.0/tests/testlib.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.567470 dl-plus-0.8.0/
+-rw-rw-r--   0 def       (1000) def       (1000)     1090 2024-01-24 09:52:12.000000 dl-plus-0.8.0/LICENSE
+-rw-r--r--   0 def       (1000) def       (1000)     3903 2024-04-03 13:38:23.567470 dl-plus-0.8.0/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)     2994 2023-07-27 10:36:26.000000 dl-plus-0.8.0/README.md
+-rw-rw-r--   0 def       (1000) def       (1000)     2331 2024-01-24 09:48:35.000000 dl-plus-0.8.0/pyproject.toml
+-rw-rw-r--   0 def       (1000) def       (1000)       38 2024-04-03 13:38:23.567470 dl-plus-0.8.0/setup.cfg
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.563470 dl-plus-0.8.0/src/
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.563470 dl-plus-0.8.0/src/dl_plus/
+-rw-rw-r--   0 def       (1000) def       (1000)       38 2022-04-23 13:15:25.000000 dl-plus-0.8.0/src/dl_plus/__main__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     5286 2024-02-01 16:48:45.000000 dl-plus-0.8.0/src/dl_plus/backend.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.563470 dl-plus-0.8.0/src/dl_plus/cli/
+-rw-rw-r--   0 def       (1000) def       (1000)       43 2022-04-23 13:15:25.000000 dl-plus-0.8.0/src/dl_plus/cli/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1931 2023-07-03 14:42:02.000000 dl-plus-0.8.0/src/dl_plus/cli/args.py
+-rw-rw-r--   0 def       (1000) def       (1000)     4066 2024-02-01 08:26:53.000000 dl-plus-0.8.0/src/dl_plus/cli/cli.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3037 2024-02-01 15:59:49.000000 dl-plus-0.8.0/src/dl_plus/cli/command.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.563470 dl-plus-0.8.0/src/dl_plus/cli/commands/
+-rw-rw-r--   0 def       (1000) def       (1000)      439 2024-02-01 16:52:51.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/__init__.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.563470 dl-plus-0.8.0/src/dl_plus/cli/commands/backend/
+-rw-rw-r--   0 def       (1000) def       (1000)      384 2023-07-03 14:49:37.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/backend/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)      755 2024-02-12 16:18:29.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/backend/base.py
+-rw-rw-r--   0 def       (1000) def       (1000)      912 2024-02-12 16:19:50.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/backend/info.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1019 2023-07-03 15:24:37.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/backend/install.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1090 2023-07-03 15:26:11.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/backend/update.py
+-rw-rw-r--   0 def       (1000) def       (1000)     8193 2024-02-04 10:33:50.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/base.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.563470 dl-plus-0.8.0/src/dl_plus/cli/commands/config/
+-rw-rw-r--   0 def       (1000) def       (1000)      233 2024-02-01 16:01:22.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/config/__init__.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.563470 dl-plus-0.8.0/src/dl_plus/cli/commands/config/show/
+-rw-rw-r--   0 def       (1000) def       (1000)      631 2024-02-01 16:54:16.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/config/show/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1782 2024-02-01 16:52:27.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/config/show/backends.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1403 2024-02-01 16:39:44.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/config/show/main.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.567470 dl-plus-0.8.0/src/dl_plus/cli/commands/extractor/
+-rw-rw-r--   0 def       (1000) def       (1000)      332 2023-07-01 13:45:38.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/extractor/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1059 2023-07-03 15:12:18.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/extractor/base.py
+-rw-rw-r--   0 def       (1000) def       (1000)      987 2023-07-03 12:11:53.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/extractor/install.py
+-rw-rw-r--   0 def       (1000) def       (1000)      524 2023-07-03 12:11:48.000000 dl-plus-0.8.0/src/dl_plus/cli/commands/extractor/update.py
+-rw-rw-r--   0 def       (1000) def       (1000)     8294 2024-01-14 11:20:11.000000 dl-plus-0.8.0/src/dl_plus/config.py
+-rw-rw-r--   0 def       (1000) def       (1000)       65 2024-04-03 13:22:27.000000 dl-plus-0.8.0/src/dl_plus/const.py
+-rw-rw-r--   0 def       (1000) def       (1000)     2039 2024-01-14 10:58:48.000000 dl-plus-0.8.0/src/dl_plus/core.py
+-rw-rw-r--   0 def       (1000) def       (1000)      765 2023-10-31 16:03:37.000000 dl-plus-0.8.0/src/dl_plus/deprecated.py
+-rw-rw-r--   0 def       (1000) def       (1000)      564 2022-04-23 13:15:25.000000 dl-plus-0.8.0/src/dl_plus/exceptions.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.567470 dl-plus-0.8.0/src/dl_plus/extractor/
+-rw-rw-r--   0 def       (1000) def       (1000)      413 2023-07-25 09:52:48.000000 dl-plus-0.8.0/src/dl_plus/extractor/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1899 2024-02-09 10:05:36.000000 dl-plus-0.8.0/src/dl_plus/extractor/extractor.py
+-rw-rw-r--   0 def       (1000) def       (1000)     2116 2022-04-23 13:15:25.000000 dl-plus-0.8.0/src/dl_plus/extractor/machinery.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3134 2022-04-23 13:15:25.000000 dl-plus-0.8.0/src/dl_plus/extractor/peqn.py
+-rw-rw-r--   0 def       (1000) def       (1000)     5817 2022-04-23 13:15:25.000000 dl-plus-0.8.0/src/dl_plus/extractor/plugin.py
+-rw-rw-r--   0 def       (1000) def       (1000)     5922 2024-02-08 14:03:49.000000 dl-plus-0.8.0/src/dl_plus/pypi.py
+-rw-rw-r--   0 def       (1000) def       (1000)      276 2022-04-23 13:15:25.000000 dl-plus-0.8.0/src/dl_plus/utils.py
+-rw-rw-r--   0 def       (1000) def       (1000)     6309 2024-02-09 09:36:43.000000 dl-plus-0.8.0/src/dl_plus/ytdl.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.567470 dl-plus-0.8.0/src/dl_plus.egg-info/
+-rw-r--r--   0 def       (1000) def       (1000)     3903 2024-04-03 13:38:23.000000 dl-plus-0.8.0/src/dl_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)     1404 2024-04-03 13:38:23.000000 dl-plus-0.8.0/src/dl_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2024-04-03 13:38:23.000000 dl-plus-0.8.0/src/dl_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 def       (1000) def       (1000)       45 2024-04-03 13:38:23.000000 dl-plus-0.8.0/src/dl_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2024-04-03 13:38:23.000000 dl-plus-0.8.0/src/dl_plus.egg-info/not-zip-safe
+-rw-rw-r--   0 def       (1000) def       (1000)        8 2024-04-03 13:38:23.000000 dl-plus-0.8.0/src/dl_plus.egg-info/top_level.txt
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-04-03 13:38:23.567470 dl-plus-0.8.0/tests/
+-rw-rw-r--   0 def       (1000) def       (1000)      402 2023-07-01 14:25:07.000000 dl-plus-0.8.0/tests/testlib.py
```

### Comparing `dl-plus-0.7.0/LICENSE` & `dl-plus-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/PKG-INFO` & `dl-plus-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-plus
-Version: 0.7.0
+Version: 0.8.0
 Summary: A youtube-dl extension with pluggable extractors
 Author-email: Dmitry Meyer <me@undef.im>
 License: MIT
 Project-URL: Homepage, https://github.com/un-def/dl-plus
 Project-URL: Repository, https://github.com/un-def/dl-plus.git
 Project-URL: Changelog, https://github.com/un-def/dl-plus/blob/master/CHANGELOG.md
 Project-URL: Issues, https://github.com/un-def/dl-plus/issues
```

### Comparing `dl-plus-0.7.0/README.md` & `dl-plus-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/pyproject.toml` & `dl-plus-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/backend.py` & `dl-plus-0.8.0/src/dl_plus/backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,94 @@
 from __future__ import annotations
 
-import enum
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, NamedTuple, Optional
 
 from dl_plus import ytdl
-from dl_plus.config import ConfigValue, get_data_home
+from dl_plus.config import ConfigValue, _Config, get_config_home, get_data_home
 from dl_plus.exceptions import DLPlusException
 from dl_plus.pypi import load_metadata
 
 
 if TYPE_CHECKING:
     from .pypi import Metadata
 
 
+def _normalize(string: str) -> str:
+    return string.replace('-', '_')
+
+
 class Backend(NamedTuple):
     # a name of the project ("distribution" in PyPA terms)
     # *.dist-info/METADATA->Name
     project_name: str
     # a name of the root package directory
     # *.dist-info/top_level.txt
     import_name: str
     # a name of the the executable script
     # *.dist-info/entry_points.txt->console_scripts).
     executable_name: str
 
 
-class KnownBackend(Backend, enum.Enum):
-    # NB: the order of members does matter: _autodetect_backend()
-    # builds a list of candidates from this enumeration.
-    YT_DLP = ('yt-dlp', 'yt_dlp', 'yt-dlp')
-    YOUTUBE_DL = ('youtube-dl', 'youtube_dl', 'youtube-dl')
-    YOUTUBE_DLC = ('youtube-dlc', 'youtube_dlc', 'youtube-dlc')
+DEFAULT_BACKENDS_CONFIG = """
+[yt-dlp]
+project-name = yt-dlp
+import-name = yt_dlp
+executable-name = yt-dlp
+
+[youtube-dl-nightly]
+project-name = youtube-dl-nightly
+import-name = youtube_dl
+executable-name = youtube-dl
+
+[youtube-dl]
+project-name = youtube_dl
+import-name = youtube_dl
+executable-name = youtube-dl
+
+[youtube-dlc]
+project-name = youtube-dlc
+import-name = youtube_dlc
+executable-name = youtube-dlc
+"""
+
+
+def parse_backends_config(content: str) -> dict[str, Backend]:
+    config = _Config()
+    config.read_string(content)
+    backends = {}
+    for alias in config.sections():
+        backends[_normalize(alias)] = Backend(**{
+            _normalize(field): value
+            for field, value in config[alias].items()
+        })
+    return backends
+
+
+_known_backends: dict[str, Backend] | None = None
+
+
+def get_backends_config_path() -> Optional[Path]:
+    path = get_config_home() / 'backends.ini'
+    if not path.is_file():
+        return None
+    return path
+
+
+def get_known_backends() -> dict[str, Backend]:
+    global _known_backends
+    if _known_backends is not None:
+        return _known_backends
+    _known_backends = parse_backends_config(DEFAULT_BACKENDS_CONFIG)
+    config_path = get_backends_config_path()
+    if config_path:
+        with open(config_path) as fobj:
+            _known_backends.update(parse_backends_config(fobj.read()))
+    return _known_backends
 
 
 class BackendInfo(NamedTuple):
     import_name: str
     version: str
     path: Path
     is_managed: bool
@@ -62,51 +114,57 @@
     try:
         location.relative_to(get_backends_dir())
         return True
     except ValueError:
         return False
 
 
-def _normalize(string: str) -> str:
-    return string.replace('-', '_')
-
-
 def get_backends_dir() -> Path:
     return get_data_home() / 'backends'
 
 
 def get_backend_dir(backend: str) -> Path:
     return get_backends_dir() / _normalize(backend)
 
 
 def parse_backend_string(backend_string: str) -> tuple[Path | None, str]:
+    # backend_string is one of:
+    #   * alias ([section-name] in the backends.ini, e.g., 'yt-dlp');
+    #   * 'import_name', e.g., 'youtube_dl';
+    #   * 'project-name/import_name', e.g., 'youtube-dl-nightly/youtube_dl'.
     if '/' in backend_string:
-        backend, _, package_name = backend_string.partition('/')
-        backend_dir = get_backend_dir(backend)
+        project_name, _, import_name = backend_string.partition('/')
+        backend_dir = get_backend_dir(project_name)
         if not backend_dir.is_dir():
             raise BackendError(
                 f'{backend_dir} does not exist or is not a directory')
+    elif backend := get_known_backends().get(_normalize(backend_string)):
+        import_name = backend.import_name
+        backend_dir = get_backend_dir(backend.project_name)
+        if not backend_dir.is_dir():
+            # in case of backends not managed by dl-plus
+            backend_dir = None
     else:
-        package_name = backend_string
+        import_name = backend_string
         backend_dir = get_backend_dir(backend_string)
         if not backend_dir.is_dir():
             backend_dir = None
-    return backend_dir, _normalize(package_name)
+    return backend_dir, _normalize(import_name)
 
 
 def _init_backend(backend_string: str) -> Path | None:
     backend_dir, package_name = parse_backend_string(backend_string)
     if backend_dir:
         sys.path.insert(0, str(backend_dir))
     ytdl.init(package_name)
     return backend_dir
 
 
 def _autodetect_backend() -> Path | None:
-    candidates = [backend.import_name for backend in KnownBackend]
+    candidates = tuple(get_known_backends())
     for candidate in candidates:
         try:
             return _init_backend(candidate)
         except DLPlusException:
             pass
     raise AutodetectFailed(candidates)
```

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/args.py` & `dl-plus-0.8.0/src/dl_plus/cli/args.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/cli.py` & `dl-plus-0.8.0/src/dl_plus/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import pathlib
 import sys
 from textwrap import dedent
 from typing import Union
 
 from dl_plus import core, ytdl
-from dl_plus.backend import KnownBackend, init_backend
+from dl_plus.backend import get_known_backends, init_backend
 from dl_plus.config import Config
 from dl_plus.const import DL_PLUS_VERSION
 from dl_plus.exceptions import DLPlusException
 
 from . import args as cli_args
 
 
@@ -25,15 +25,18 @@
 
 def _detect_compat_mode(program_name: str) -> bool:
     path = pathlib.Path(program_name)
     if path.suffix == '.exe':
         name = path.stem
     else:
         name = path.name
-    return name in (backend.executable_name for backend in KnownBackend)
+    return name in (
+        backend.executable_name for backend
+        in get_known_backends().values()
+    )
 
 
 class _MainArgParser(argparse.ArgumentParser):
 
     def format_help(self):
         return super().format_help() + ytdl.get_help()
```

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/command.py` & `dl-plus-0.8.0/src/dl_plus/cli/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,26 +23,35 @@
         super().__init__(**kwargs)
         self.__dict__[_COMMAND_DEST] = []
 
     def _get_command(self):
         return self.__dict__[_COMMAND_DEST]
 
     def _set_command(self, value):
-        self.__dict__[_COMMAND_DEST].append(value)
+        if isinstance(value, list):
+            self.__dict__[_COMMAND_DEST].extend(value)
+        else:
+            assert isinstance(value, str), repr(str)
+            self.__dict__[_COMMAND_DEST].append(value)
 
     command = property(_get_command, _set_command)
 
 
 class CommandArgParser(argparse.ArgumentParser):
 
     def __init__(self, *args, **kwargs):
         kwargs.setdefault(
             'formatter_class', argparse.RawDescriptionHelpFormatter)
         super().__init__(*args, **kwargs)
 
+    def parse_known_args(self, args=None, namespace=None):
+        if namespace is None:
+            namespace = CommandNamespace()
+        return super().parse_known_args(args, namespace)
+
     def add_command_arguments(self, command: Type[Command]):
         for parent in command.get_parents():
             for arg in parent.arguments:
                 arg.add_to_parser(self)
         for arg in command.arguments:
             arg.add_to_parser(self)
 
@@ -63,21 +72,20 @@
                 command_parser.add_command_group(command_or_group)
             else:
                 command_parser.add_command_arguments(command_or_group)
 
     def add_command_group_subparsers(self, *args, **kwargs):
         kwargs.setdefault('dest', _COMMAND_DEST)
         kwargs.setdefault('metavar', 'COMMAND')
-        kwargs.setdefault('parser_class', self.__class__)
         kwargs.setdefault('required', True)
         subparsers = self.add_subparsers(*args, **kwargs)
         return subparsers
 
 
 def run_command(prog: str, cmd_arg: str, args: List[str]) -> None:
     parser = CommandArgParser(prog=f'{prog} {cmd_arg}')
     parser.add_argument(
         cmd_arg, action='store_true', required=True, help=argparse.SUPPRESS)
     parser.add_command_group(RootCommandGroup)
-    parsed_args = parser.parse_args(args, namespace=CommandNamespace())
+    parsed_args = parser.parse_args(args)
     command_cls = RootCommandGroup.get_command(parsed_args.command)
     command_cls(parsed_args).run()
```

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/commands/backend/info.py` & `dl-plus-0.8.0/src/dl_plus/cli/commands/backend/info.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dl_plus.backend import init_backend
 from dl_plus.cli.args import Arg
 from dl_plus.cli.commands.base import Command
 
+from .base import BackendCommandMixin
 
-class BackendInfoCommand(Command):
+
+class BackendInfoCommand(BackendCommandMixin, Command):
 
     short_description = 'Show backend information'
 
     arguments = (
         Arg(
             'name', nargs='?', metavar='NAME',
             help='Backend name.'
```

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/commands/backend/install.py` & `dl-plus-0.8.0/src/dl_plus/cli/commands/backend/install.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/commands/backend/update.py` & `dl-plus-0.8.0/src/dl_plus/cli/commands/backend/update.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/commands/base.py` & `dl-plus-0.8.0/src/dl_plus/cli/commands/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
-import os
-import shutil
-import zipfile
 from argparse import Namespace
+from functools import cached_property
 from pathlib import Path
 from textwrap import dedent
 from typing import (
     TYPE_CHECKING, ClassVar, Dict, List, Optional, Sequence, Tuple, Type,
     Union,
 )
 
-from dl_plus.config import Config
+from dl_plus.config import Config, ConfigError, get_config_path
 from dl_plus.exceptions import DLPlusException
-from dl_plus.pypi import PyPIClient, Wheel, load_metadata, save_metadata
+from dl_plus.pypi import PyPIClient, Wheel, WheelInstaller, load_metadata
 
 
 if TYPE_CHECKING:
     from dl_plus.cli.args import Arg, ArgGroup, ExclusiveArgGroup
     from dl_plus.pypi import Metadata
 
 
@@ -66,38 +64,41 @@
             path.append(self.name)
         return path
 
 
 class Command(_CommandBase):
     args: Namespace
 
-    _config: Optional[Config] = None
-
     def __init__(self, args: Namespace) -> None:
         self.args = args
         self.init()
 
     def init(self) -> None:
         pass
 
     def run(self) -> None:
         raise NotImplementedError
 
-    @property
+    @cached_property
+    def config_path(self) -> Optional[Path]:
+        try:
+            return get_config_path(getattr(self.args, 'dlp_config', None))
+        except ConfigError:
+            return None
+
+    @cached_property
     def config(self) -> Config:
-        if self._config is None:
-            config = Config()
-            config_file: Union[str, bool, None]
-            if getattr(self.args, 'no_dlp_config', False):
-                config_file = False
-            else:
-                config_file = getattr(self.args, 'dlp_config', None)
-            config.load(config_file)
-            self._config = config
-        return self._config
+        config = Config()
+        config_file: Union[Path, bool, None]
+        if getattr(self.args, 'no_dlp_config', False):
+            config_file = False
+        else:
+            config_file = self.config_path
+        config.load(config_file)
+        return config
 
     def die(self, message: str) -> None:
         raise CommandError(message)
 
     print = print
 
 
@@ -133,39 +134,32 @@
 class CommandError(DLPlusException):
 
     pass
 
 
 class BaseInstallUpdateCommand(Command):
     client: PyPIClient
+    wheel_installer: WheelInstaller
 
     def get_output_dir(self, wheel: Wheel) -> Path:
         raise NotImplementedError
 
     def get_short_name(self) -> str:
         """Return short name used for logging, command examples, etc."""
         raise NotImplementedError
 
     def init(self) -> None:
         self.client = PyPIClient()
+        self.wheel_installer = WheelInstaller()
 
     def load_installed_metadata(self, output_dir: Path) -> Optional[Metadata]:
         if not output_dir.exists():
             return None
         return load_metadata(output_dir)
 
-    def install_wheel(self, wheel: Wheel, output_dir: Path) -> None:
-        if output_dir.exists():
-            shutil.rmtree(output_dir)
-        os.makedirs(output_dir)
-        with self.client.download_file(wheel.url, wheel.sha256) as fobj:
-            with zipfile.ZipFile(fobj) as zfobj:
-                zfobj.extractall(output_dir)
-        save_metadata(output_dir, wheel.metadata)
-
 
 class BaseInstallCommand(BaseInstallUpdateCommand):
 
     def get_project_name_version_tuple(self) -> Tuple[str, Optional[str]]:
         raise NotImplementedError
 
     def get_force_flag(self) -> bool:
@@ -211,15 +205,16 @@
                 return
             self.print('Forcing installation')
 
         self.install(wheel, output_dir)
 
     def install(self, wheel: Wheel, output_dir: Path) -> None:
         self.print('Installing')
-        self.install_wheel(wheel, output_dir)
+        self.print(f'Using {self.wheel_installer.identifier} installer')
+        self.wheel_installer.install(wheel, output_dir)
         self.print('Installed')
 
 
 class BaseUpdateCommand(BaseInstallUpdateCommand):
 
     def get_project_name(self) -> str:
         raise NotImplementedError
@@ -249,9 +244,10 @@
             self.print('The latest version is already installed')
             return
 
         self.update(wheel, output_dir)
 
     def update(self, wheel: Wheel, output_dir: Path) -> None:
         self.print('Updating')
-        self.install_wheel(wheel, output_dir)
+        self.print(f'Using {self.wheel_installer.identifier} installer')
+        self.wheel_installer.install(wheel, output_dir)
         self.print('Updated')
```

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/commands/extractor/base.py` & `dl-plus-0.8.0/src/dl_plus/cli/commands/extractor/base.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/commands/extractor/install.py` & `dl-plus-0.8.0/src/dl_plus/cli/commands/extractor/install.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/cli/commands/extractor/update.py` & `dl-plus-0.8.0/src/dl_plus/cli/commands/extractor/update.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/config.py` & `dl-plus-0.8.0/src/dl_plus/config.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/core.py` & `dl-plus-0.8.0/src/dl_plus/core.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/deprecated.py` & `dl-plus-0.8.0/src/dl_plus/deprecated.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/exceptions.py` & `dl-plus-0.8.0/src/dl_plus/exceptions.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/extractor/extractor.py` & `dl-plus-0.8.0/src/dl_plus/extractor/extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,25 @@
                 raise ExtractorError(
                     f'_VALID_URL: string expected, got: {valid_url!r}')
             # a copy/paste from youtube-dl
             if '_VALID_URL_RE' not in cls.__dict__:
                 cls._VALID_URL_RE = re.compile(valid_url)
             return cls._VALID_URL_RE.match(url)
 
+    if (
+            ytdl.get_ytdl_module_name() == 'yt_dlp'
+            and ytdl.get_ytdl_module_version() >= '2023.01.02'
+    ):
+
+        # suppress some warnings
+        def _sort_formats(self, formats, field_preference=None):
+            if not formats or not field_preference:
+                return
+            super()._sort_formats(formats, field_preference)
+
     # dl-plus extra attributes/methods
 
     DLP_BASE_URL: Optional[str] = None
     DLP_REL_URL: Optional[str] = None
 
     @classmethod
     def dlp_match(cls, url: str) -> Optional[Match[str]]:
```

### Comparing `dl-plus-0.7.0/src/dl_plus/extractor/machinery.py` & `dl-plus-0.8.0/src/dl_plus/extractor/machinery.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/extractor/peqn.py` & `dl-plus-0.8.0/src/dl_plus/extractor/peqn.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/extractor/plugin.py` & `dl-plus-0.8.0/src/dl_plus/extractor/plugin.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.7.0/src/dl_plus/ytdl.py` & `dl-plus-0.8.0/src/dl_plus/ytdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,24 @@
 
 def get_ytdl_module():
     _check_initialized()
     global _ytdl_module
     return _ytdl_module
 
 
+def get_ytdl_module_name():
+    _check_initialized()
+    global _ytdl_module_name
+    return _ytdl_module_name
+
+
+def get_ytdl_module_version():
+    return import_from('version', '__version__')
+
+
 def get_help():
     _check_initialized()
     with StringIO() as buffer:
         stdout, stderr = sys.stdout, sys.stderr
         sys.stdout = sys.stderr = buffer
         try:
             _ytdl_module.main(['--help'])
```

### Comparing `dl-plus-0.7.0/src/dl_plus.egg-info/PKG-INFO` & `dl-plus-0.8.0/src/dl_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-plus
-Version: 0.7.0
+Version: 0.8.0
 Summary: A youtube-dl extension with pluggable extractors
 Author-email: Dmitry Meyer <me@undef.im>
 License: MIT
 Project-URL: Homepage, https://github.com/un-def/dl-plus
 Project-URL: Repository, https://github.com/un-def/dl-plus.git
 Project-URL: Changelog, https://github.com/un-def/dl-plus/blob/master/CHANGELOG.md
 Project-URL: Issues, https://github.com/un-def/dl-plus/issues
```

### Comparing `dl-plus-0.7.0/src/dl_plus.egg-info/SOURCES.txt` & `dl-plus-0.8.0/src/dl_plus.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 src/dl_plus/cli/commands/__init__.py
 src/dl_plus/cli/commands/base.py
 src/dl_plus/cli/commands/backend/__init__.py
 src/dl_plus/cli/commands/backend/base.py
 src/dl_plus/cli/commands/backend/info.py
 src/dl_plus/cli/commands/backend/install.py
 src/dl_plus/cli/commands/backend/update.py
+src/dl_plus/cli/commands/config/__init__.py
+src/dl_plus/cli/commands/config/show/__init__.py
+src/dl_plus/cli/commands/config/show/backends.py
+src/dl_plus/cli/commands/config/show/main.py
 src/dl_plus/cli/commands/extractor/__init__.py
 src/dl_plus/cli/commands/extractor/base.py
 src/dl_plus/cli/commands/extractor/install.py
 src/dl_plus/cli/commands/extractor/update.py
 src/dl_plus/extractor/__init__.py
 src/dl_plus/extractor/extractor.py
 src/dl_plus/extractor/machinery.py
```

