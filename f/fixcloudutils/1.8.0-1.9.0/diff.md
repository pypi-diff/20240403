# Comparing `tmp/fixcloudutils-1.8.0.tar.gz` & `tmp/fixcloudutils-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixcloudutils-1.8.0.tar", last modified: Mon Oct 30 12:02:19 2023, max compression
+gzip compressed data, was "fixcloudutils-1.9.0.tar", last modified: Fri Nov  3 11:47:07 2023, max compression
```

## Comparing `fixcloudutils-1.8.0.tar` & `fixcloudutils-1.9.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:02:19.653307 fixcloudutils-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34477 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40885 2023-10-30 12:02:19.653307 fixcloudutils-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:02:19.649306 fixcloudutils-1.8.0/fixcloudutils/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:02:19.649306 fixcloudutils-1.8.0/fixcloudutils/arangodb/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/arangodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/arangodb/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21682 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/arangodb/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/arangodb/entitydb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:02:19.653307 fixcloudutils-1.8.0/fixcloudutils/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/asyncio/async_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/asyncio/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/asyncio/timed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:02:19.653307 fixcloudutils-1.8.0/fixcloudutils/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/logging/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/logging/prometheus_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:02:19.653307 fixcloudutils-1.8.0/fixcloudutils/redis/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/redis/event_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/redis/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/redis/pub_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/fixcloudutils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:02:19.649306 fixcloudutils-1.8.0/fixcloudutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40885 2023-10-30 12:02:19.000000 fixcloudutils-1.8.0/fixcloudutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-30 12:02:19.000000 fixcloudutils-1.8.0/fixcloudutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 12:02:19.000000 fixcloudutils-1.8.0/fixcloudutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 12:00:32.000000 fixcloudutils-1.8.0/fixcloudutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-10-30 12:02:19.000000 fixcloudutils-1.8.0/fixcloudutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-30 12:02:19.000000 fixcloudutils-1.8.0/fixcloudutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-10-30 12:00:24.000000 fixcloudutils-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-30 12:02:19.653307 fixcloudutils-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:47:07.442534 fixcloudutils-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34477 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40885 2023-11-03 11:47:07.442534 fixcloudutils-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:47:07.434534 fixcloudutils-1.9.0/fixcloudutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:47:07.438534 fixcloudutils-1.9.0/fixcloudutils/arangodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/arangodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/arangodb/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21682 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/arangodb/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/arangodb/entitydb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:47:07.438534 fixcloudutils-1.9.0/fixcloudutils/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/asyncio/async_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/asyncio/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/asyncio/timed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:47:07.438534 fixcloudutils-1.9.0/fixcloudutils/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/logging/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/logging/prometheus_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:47:07.438534 fixcloudutils-1.9.0/fixcloudutils/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/redis/event_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/redis/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/redis/pub_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/fixcloudutils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:47:07.434534 fixcloudutils-1.9.0/fixcloudutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40885 2023-11-03 11:47:07.000000 fixcloudutils-1.9.0/fixcloudutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-11-03 11:47:07.000000 fixcloudutils-1.9.0/fixcloudutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 11:47:07.000000 fixcloudutils-1.9.0/fixcloudutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 11:45:00.000000 fixcloudutils-1.9.0/fixcloudutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-11-03 11:47:07.000000 fixcloudutils-1.9.0/fixcloudutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-03 11:47:07.000000 fixcloudutils-1.9.0/fixcloudutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-11-03 11:44:51.000000 fixcloudutils-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-11-03 11:47:07.442534 fixcloudutils-1.9.0/setup.cfg
```

### Comparing `fixcloudutils-1.8.0/LICENSE` & `fixcloudutils-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/PKG-INFO` & `fixcloudutils-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixcloudutils
-Version: 1.8.0
+Version: 1.9.0
 Summary: Utilities for fixcloud.
 Author: Some Engineering Inc.
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fixcloudutils-1.8.0/fixcloudutils/__init__.py` & `fixcloudutils-1.9.0/fixcloudutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/arangodb/__init__.py` & `fixcloudutils-1.9.0/fixcloudutils/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/arangodb/arangodb_extensions.py` & `fixcloudutils-1.9.0/fixcloudutils/arangodb/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/arangodb/async_arangodb.py` & `fixcloudutils-1.9.0/fixcloudutils/arangodb/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/arangodb/entitydb.py` & `fixcloudutils-1.9.0/fixcloudutils/arangodb/entitydb.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/asyncio/__init__.py` & `fixcloudutils-1.9.0/fixcloudutils/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/asyncio/async_extensions.py` & `fixcloudutils-1.9.0/fixcloudutils/asyncio/async_extensions.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/asyncio/periodic.py` & `fixcloudutils-1.9.0/fixcloudutils/asyncio/periodic.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/asyncio/timed.py` & `fixcloudutils-1.9.0/fixcloudutils/asyncio/timed.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/logging/__init__.py` & `fixcloudutils-1.9.0/fixcloudutils/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/logging/json_logger.py` & `fixcloudutils-1.9.0/fixcloudutils/logging/json_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,32 +17,34 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Affero General Public License for more details.
 #
 #  You should have received a copy of the GNU Affero General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import json
 from logging import Formatter, LogRecord
-from typing import Mapping, Optional, Dict
+from typing import Mapping, Optional, Dict, Callable
 
 
 class JsonFormatter(Formatter):
     """
     Simple json log formatter.
     """
 
     def __init__(
         self,
         fmt_dict: Mapping[str, str],
         time_format: str = "%Y-%m-%dT%H:%M:%S",
         static_values: Optional[Dict[str, str]] = None,
+        get_logging_context: Optional[Callable[[], Dict[str, str]]] = None,
     ) -> None:
         super().__init__()
         self.fmt_dict = fmt_dict
         self.time_format = time_format
         self.static_values = static_values or {}
+        self.get_logging_context = get_logging_context
         self.__uses_time = "asctime" in self.fmt_dict.values()
 
     def usesTime(self) -> bool:  # noqa: N802
         return self.__uses_time
 
     def format(self, record: LogRecord) -> str:
         def prop(name: str) -> str:
@@ -51,14 +53,16 @@
             elif name == "message":
                 return record.getMessage()
             else:
                 return getattr(record, name, "n/a")
 
         message_dict = {fmt_key: prop(fmt_val) for fmt_key, fmt_val in self.fmt_dict.items()}
         message_dict.update(self.static_values)
+        if get_context := self.get_logging_context:
+            message_dict.update(get_context())
         if record.exc_info:
             if not record.exc_text:
                 record.exc_text = self.formatException(record.exc_info)
         if record.exc_text:
             message_dict["exception"] = record.exc_text
         if record.stack_info:
             message_dict["stack_info"] = self.formatStack(record.stack_info)
```

### Comparing `fixcloudutils-1.8.0/fixcloudutils/logging/prometheus_counter.py` & `fixcloudutils-1.9.0/fixcloudutils/logging/prometheus_counter.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/redis/__init__.py` & `fixcloudutils-1.9.0/fixcloudutils/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/redis/event_stream.py` & `fixcloudutils-1.9.0/fixcloudutils/redis/event_stream.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/redis/lock.py` & `fixcloudutils-1.9.0/fixcloudutils/redis/lock.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/redis/pub_sub.py` & `fixcloudutils-1.9.0/fixcloudutils/redis/pub_sub.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/service.py` & `fixcloudutils-1.9.0/fixcloudutils/service.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/types.py` & `fixcloudutils-1.9.0/fixcloudutils/types.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils/util.py` & `fixcloudutils-1.9.0/fixcloudutils/util.py`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/fixcloudutils.egg-info/PKG-INFO` & `fixcloudutils-1.9.0/fixcloudutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixcloudutils
-Version: 1.8.0
+Version: 1.9.0
 Summary: Utilities for fixcloud.
 Author: Some Engineering Inc.
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fixcloudutils-1.8.0/fixcloudutils.egg-info/SOURCES.txt` & `fixcloudutils-1.9.0/fixcloudutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixcloudutils-1.8.0/pyproject.toml` & `fixcloudutils-1.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixcloudutils"
-version = "1.8.0"
+version = "1.9.0"
 authors = [{ name = "Some Engineering Inc." }]
 description = "Utilities for fixcloud."
 license = { file = "LICENSE" }
 urls = { "Homepage" = "https://fix.tt" }
 requires-python = ">=3.9"
 classifiers = ["Programming Language :: Python :: 3"]
 readme = { file = "README.md", content-type = "text/markdown" }
```

