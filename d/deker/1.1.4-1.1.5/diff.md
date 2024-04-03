# Comparing `tmp/deker-1.1.4.tar.gz` & `tmp/deker-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deker-1.1.4.tar", max compression
+gzip compressed data, was "deker-1.1.5.tar", max compression
```

## Comparing `deker-1.1.4.tar` & `deker-1.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35149 2024-03-05 13:45:07.275511 deker-1.1.4/LICENSE
--rw-r--r--   0        0        0     4264 2024-03-05 13:45:07.275511 deker-1.1.4/README.md
--rw-r--r--   0        0        0     1141 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/__init__.py
--rw-r--r--   0        0        0    17166 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_adapters.py
--rw-r--r--   0        0        0    21663 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_array.py
--rw-r--r--   0        0        0     1595 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_collection.py
--rw-r--r--   0        0        0     2254 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_dimension.py
--rw-r--r--   0        0        0     2900 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_factory.py
--rw-r--r--   0        0        0     2471 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_integrity.py
--rw-r--r--   0        0        0     5216 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_locks.py
--rw-r--r--   0        0        0     3266 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_managers.py
--rw-r--r--   0        0        0     6487 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_schemas.py
--rw-r--r--   0        0        0    12459 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ABC/base_subset.py
--rw-r--r--   0        0        0     1746 2024-03-05 13:45:07.275511 deker-1.1.4/deker/__init__.py
--rw-r--r--   0        0        0    12506 2024-03-05 13:45:07.275511 deker-1.1.4/deker/arrays.py
--rw-r--r--   0        0        0    25520 2024-03-05 13:45:07.275511 deker-1.1.4/deker/client.py
--rw-r--r--   0        0        0    13687 2024-03-05 13:45:07.275511 deker-1.1.4/deker/collection.py
--rw-r--r--   0        0        0     2134 2024-03-05 13:45:07.275511 deker-1.1.4/deker/config.py
--rw-r--r--   0        0        0     1527 2024-03-05 13:45:07.275511 deker-1.1.4/deker/ctx.py
--rw-r--r--   0        0        0    13257 2024-03-05 13:45:07.275511 deker-1.1.4/deker/dimensions.py
--rw-r--r--   0        0        0     2868 2024-03-05 13:45:07.275511 deker-1.1.4/deker/errors.py
--rw-r--r--   0        0        0     3054 2024-03-05 13:45:07.275511 deker-1.1.4/deker/flock.py
--rw-r--r--   0        0        0    11575 2024-03-05 13:45:07.275511 deker-1.1.4/deker/integrity.py
--rw-r--r--   0        0        0    19394 2024-03-05 13:45:07.279511 deker-1.1.4/deker/locks.py
--rw-r--r--   0        0        0     1853 2024-03-05 13:45:07.279511 deker-1.1.4/deker/log.py
--rw-r--r--   0        0        0     8640 2024-03-05 13:45:07.279511 deker-1.1.4/deker/managers.py
--rw-r--r--   0        0        0    18705 2024-03-05 13:45:07.279511 deker-1.1.4/deker/schemas.py
--rw-r--r--   0        0        0    26932 2024-03-05 13:45:07.279511 deker-1.1.4/deker/subset.py
--rw-r--r--   0        0        0     1193 2024-03-05 13:45:07.279511 deker-1.1.4/deker/tools/__init__.py
--rw-r--r--   0        0        0     4241 2024-03-05 13:45:07.279511 deker-1.1.4/deker/tools/array.py
--rw-r--r--   0        0        0     2063 2024-03-05 13:45:07.279511 deker-1.1.4/deker/tools/decorators.py
--rw-r--r--   0        0        0     5351 2024-03-05 13:45:07.279511 deker-1.1.4/deker/tools/path.py
--rw-r--r--   0        0        0     5157 2024-03-05 13:45:07.279511 deker-1.1.4/deker/tools/schema.py
--rw-r--r--   0        0        0     2013 2024-03-05 13:45:07.279511 deker-1.1.4/deker/tools/time.py
--rw-r--r--   0        0        0      902 2024-03-05 13:45:07.279511 deker-1.1.4/deker/types/__init__.py
--rw-r--r--   0        0        0      720 2024-03-05 13:45:07.279511 deker-1.1.4/deker/types/private/__init__.py
--rw-r--r--   0        0        0     3281 2024-03-05 13:45:07.279511 deker-1.1.4/deker/types/private/classes.py
--rw-r--r--   0        0        0     2923 2024-03-05 13:45:07.279511 deker-1.1.4/deker/types/private/enums.py
--rw-r--r--   0        0        0     1339 2024-03-05 13:45:07.279511 deker-1.1.4/deker/types/private/shell.py
--rw-r--r--   0        0        0     3388 2024-03-05 13:45:07.279511 deker-1.1.4/deker/types/private/typings.py
--rw-r--r--   0        0        0        0 2024-03-05 13:45:07.279511 deker-1.1.4/deker/types/public/__init__.py
--rw-r--r--   0        0        0     5274 2024-03-05 13:45:07.279511 deker-1.1.4/deker/types/public/classes.py
--rw-r--r--   0        0        0     6339 2024-03-05 13:45:07.279511 deker-1.1.4/deker/uri.py
--rw-r--r--   0        0        0     7766 2024-03-05 13:45:07.279511 deker-1.1.4/deker/validators.py
--rw-r--r--   0        0        0      787 2024-03-05 13:45:07.279511 deker-1.1.4/deker/warnings.py
--rw-r--r--   0        0        0     9525 2024-03-05 13:45:15.463508 deker-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     6008 1970-01-01 00:00:00.000000 deker-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-03 11:51:51.083068 deker-1.1.5/LICENSE
+-rw-r--r--   0        0        0     4264 2024-04-03 11:51:51.083068 deker-1.1.5/README.md
+-rw-r--r--   0        0        0     1141 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/__init__.py
+-rw-r--r--   0        0        0    17166 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_adapters.py
+-rw-r--r--   0        0        0    21663 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_array.py
+-rw-r--r--   0        0        0     1595 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_collection.py
+-rw-r--r--   0        0        0     2254 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_dimension.py
+-rw-r--r--   0        0        0     2900 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_factory.py
+-rw-r--r--   0        0        0     2471 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_integrity.py
+-rw-r--r--   0        0        0     5216 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_locks.py
+-rw-r--r--   0        0        0     3266 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_managers.py
+-rw-r--r--   0        0        0     6487 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_schemas.py
+-rw-r--r--   0        0        0    12459 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_subset.py
+-rw-r--r--   0        0        0     1746 2024-04-03 11:51:51.083068 deker-1.1.5/deker/__init__.py
+-rw-r--r--   0        0        0    12506 2024-04-03 11:51:51.083068 deker-1.1.5/deker/arrays.py
+-rw-r--r--   0        0        0    25520 2024-04-03 11:51:51.083068 deker-1.1.5/deker/client.py
+-rw-r--r--   0        0        0    13687 2024-04-03 11:51:51.083068 deker-1.1.5/deker/collection.py
+-rw-r--r--   0        0        0     2134 2024-04-03 11:51:51.083068 deker-1.1.5/deker/config.py
+-rw-r--r--   0        0        0     1527 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ctx.py
+-rw-r--r--   0        0        0    13257 2024-04-03 11:51:51.083068 deker-1.1.5/deker/dimensions.py
+-rw-r--r--   0        0        0     2868 2024-04-03 11:51:51.083068 deker-1.1.5/deker/errors.py
+-rw-r--r--   0        0        0     3054 2024-04-03 11:51:51.083068 deker-1.1.5/deker/flock.py
+-rw-r--r--   0        0        0    11575 2024-04-03 11:51:51.083068 deker-1.1.5/deker/integrity.py
+-rw-r--r--   0        0        0    19347 2024-04-03 11:51:51.083068 deker-1.1.5/deker/locks.py
+-rw-r--r--   0        0        0     1848 2024-04-03 11:51:51.083068 deker-1.1.5/deker/log.py
+-rw-r--r--   0        0        0     8640 2024-04-03 11:51:51.083068 deker-1.1.5/deker/managers.py
+-rw-r--r--   0        0        0    18705 2024-04-03 11:51:51.083068 deker-1.1.5/deker/schemas.py
+-rw-r--r--   0        0        0    26932 2024-04-03 11:51:51.083068 deker-1.1.5/deker/subset.py
+-rw-r--r--   0        0        0     1193 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/__init__.py
+-rw-r--r--   0        0        0     4241 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/array.py
+-rw-r--r--   0        0        0     2063 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/decorators.py
+-rw-r--r--   0        0        0     5351 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/path.py
+-rw-r--r--   0        0        0     5157 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/schema.py
+-rw-r--r--   0        0        0     2013 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/time.py
+-rw-r--r--   0        0        0      902 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/__init__.py
+-rw-r--r--   0        0        0     3281 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/classes.py
+-rw-r--r--   0        0        0     2923 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/enums.py
+-rw-r--r--   0        0        0     1339 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/shell.py
+-rw-r--r--   0        0        0     3388 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/typings.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/public/__init__.py
+-rw-r--r--   0        0        0     5274 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/public/classes.py
+-rw-r--r--   0        0        0     6339 2024-04-03 11:51:51.083068 deker-1.1.5/deker/uri.py
+-rw-r--r--   0        0        0     7766 2024-04-03 11:51:51.087068 deker-1.1.5/deker/validators.py
+-rw-r--r--   0        0        0      787 2024-04-03 11:51:51.087068 deker-1.1.5/deker/warnings.py
+-rw-r--r--   0        0        0     9525 2024-04-03 11:51:59.215157 deker-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6008 1970-01-01 00:00:00.000000 deker-1.1.5/PKG-INFO
```

### Comparing `deker-1.1.4/LICENSE` & `deker-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/README.md` & `deker-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/__init__.py` & `deker-1.1.5/deker/ABC/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_adapters.py` & `deker-1.1.5/deker/ABC/base_adapters.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_array.py` & `deker-1.1.5/deker/ABC/base_array.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_collection.py` & `deker-1.1.5/deker/ABC/base_collection.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_dimension.py` & `deker-1.1.5/deker/ABC/base_dimension.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_factory.py` & `deker-1.1.5/deker/ABC/base_factory.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_integrity.py` & `deker-1.1.5/deker/ABC/base_integrity.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_locks.py` & `deker-1.1.5/deker/ABC/base_locks.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_managers.py` & `deker-1.1.5/deker/ABC/base_managers.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_schemas.py` & `deker-1.1.5/deker/ABC/base_schemas.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ABC/base_subset.py` & `deker-1.1.5/deker/ABC/base_subset.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/__init__.py` & `deker-1.1.5/deker/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/arrays.py` & `deker-1.1.5/deker/arrays.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/client.py` & `deker-1.1.5/deker/client.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/collection.py` & `deker-1.1.5/deker/collection.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/config.py` & `deker-1.1.5/deker/config.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/ctx.py` & `deker-1.1.5/deker/ctx.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/dimensions.py` & `deker-1.1.5/deker/dimensions.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/errors.py` & `deker-1.1.5/deker/errors.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/flock.py` & `deker-1.1.5/deker/flock.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/integrity.py` & `deker-1.1.5/deker/integrity.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/locks.py` & `deker-1.1.5/deker/locks.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         # Clear links to locks
         self.locks = []
         # Locks that have been acquired by third party process
 
         # Iterate over Arrays in VArray and try to lock them. If locking fails - wait.
         # If it fails again - release all locks.
         currently_locked = self.check_arrays_locks(arrays_positions, adapter, varray)
-        if not currently_locked and (len(self.locks) == len(arrays_positions)):
+        if not currently_locked:
             # Release array locks
             return
 
         # Wait till there are no more read locks
         start_time = time.monotonic()
         while (time.monotonic() - start_time) <= adapter.ctx.config.write_lock_timeout:
             if not self.check_arrays_locks(arrays_positions, adapter, varray):
```

### Comparing `deker-1.1.4/deker/log.py` & `deker-1.1.5/deker/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,39 +9,38 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 import logging
-import os
 
-from logging import Logger
+from typing import Optional
+
 
 _ROOT_DEKER_LOGGER_NAME = "Deker"
-_level = os.getenv("DEKER_LOGLEVEL", "WARNING")
 
 format_string = "%(levelname)s | %(asctime)s | %(name)s | %(message)s"
 fmter = logging.Formatter(fmt=format_string)
 
 _logger = logging.getLogger(_ROOT_DEKER_LOGGER_NAME)
+_logger.propagate = False
 _handler = logging.StreamHandler()
 _handler.setFormatter(fmter)
 _logger.addHandler(_handler)
 
 
 class SelfLoggerMixin(object):
     """Mixin with a logger object with a possibility to log its actions."""
 
-    __logger: Logger = None
+    __logger: Optional[logging.Logger] = None
 
     @property
-    def logger(self) -> Logger:
+    def logger(self) -> logging.Logger:
         """Lazy deker logger property."""
         if not self.__logger:
             self.__logger = _logger.getChild(self.__class__.__name__)
         return self.__logger
 
 
 def set_logging_level(level: str) -> None:
```

### Comparing `deker-1.1.4/deker/managers.py` & `deker-1.1.5/deker/managers.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/schemas.py` & `deker-1.1.5/deker/schemas.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/subset.py` & `deker-1.1.5/deker/subset.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/tools/__init__.py` & `deker-1.1.5/deker/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/tools/array.py` & `deker-1.1.5/deker/tools/array.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/tools/decorators.py` & `deker-1.1.5/deker/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/tools/path.py` & `deker-1.1.5/deker/tools/path.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/tools/schema.py` & `deker-1.1.5/deker/tools/schema.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/tools/time.py` & `deker-1.1.5/deker/tools/time.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/types/__init__.py` & `deker-1.1.5/deker/types/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/types/private/__init__.py` & `deker-1.1.5/deker/types/private/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/types/private/classes.py` & `deker-1.1.5/deker/types/private/classes.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/types/private/enums.py` & `deker-1.1.5/deker/types/private/enums.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/types/private/shell.py` & `deker-1.1.5/deker/types/private/shell.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/types/private/typings.py` & `deker-1.1.5/deker/types/private/typings.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/types/public/classes.py` & `deker-1.1.5/deker/types/public/classes.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/uri.py` & `deker-1.1.5/deker/uri.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/validators.py` & `deker-1.1.5/deker/validators.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/deker/warnings.py` & `deker-1.1.5/deker/warnings.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.4/pyproject.toml` & `deker-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
                                 ###############
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
-version = "1.1.4"  # a placeholder for poetry CI dynamic versionning plugin
+version = "1.1.5"  # a placeholder for poetry CI dynamic versionning plugin
 name = "deker"
 packages = [{ include = "deker" }]
 description = "Multidimensional arrays storage engine"
 authors = ["OpenWeather <info@openweathermap.org>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 documentation = 'https://docs.deker.io/'
```

### Comparing `deker-1.1.4/PKG-INFO` & `deker-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker
-Version: 1.1.4
+Version: 1.1.5
 Summary: Multidimensional arrays storage engine
 Home-page: https://deker.io/
 License: GPL-3.0-only
 Author: OpenWeather
 Author-email: info@openweathermap.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

