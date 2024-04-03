# Comparing `tmp/orbax_checkpoint-0.5.7.tar.gz` & `tmp/orbax_checkpoint-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax_checkpoint-0.5.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orbax_checkpoint-0.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax_checkpoint-0.5.7.tar` & `orbax_checkpoint-0.5.8.tar`

### file list

```diff
@@ -1,55 +1,59 @@
--rw-r--r--   0        0        0    11357 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/LICENSE
--rw-r--r--   0        0        0      556 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/README.md
--rw-r--r--   0        0        0     3607 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0    11844 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/abstract_checkpoint_manager.py
--rw-r--r--   0        0        0     2824 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2919 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     2589 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/args.py
--rw-r--r--   0        0        0     7011 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1377 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0    13034 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     5055 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_args.py
--rw-r--r--   0        0        0     4307 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_args_test.py
--rw-r--r--   0        0        0     2324 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    51613 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0    16384 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0    12282 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     7219 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0    21516 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/composite_checkpoint_handler.py
--rw-r--r--   0        0        0    13063 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/composite_checkpoint_handler_test.py
--rw-r--r--   0        0        0      740 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0      583 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/experimental/__init__.py
--rw-r--r--   0        0        0      583 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/experimental/emergency/__init__.py
--rw-r--r--   0        0        0     2114 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/experimental/emergency/checkpoint_manager.py
--rw-r--r--   0        0        0     1576 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     3196 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     2018 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     7672 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2024-03-21 21:42:35.278915 orbax_checkpoint-0.5.7/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0    45656 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0      583 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/path/__init__.py
--rw-r--r--   0        0        0     6257 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/path/step.py
--rw-r--r--   0        0        0     6781 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/path/step_test.py
--rw-r--r--   0        0        0      757 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/proto/__init__.py
--rw-r--r--   0        0        0      757 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/proto/testing/__init__.py
--rw-r--r--   0        0        0      136 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/proto/testing/foo.proto
--rw-r--r--   0        0        0     3758 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/proto_checkpoint_handler.py
--rw-r--r--   0        0        0    56631 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     1284 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/pytree_checkpointer.py
--rw-r--r--   0        0        0     9107 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/random_key_checkpoint_handler.py
--rw-r--r--   0        0        0     6883 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/random_key_checkpoint_handler_test.py
--rw-r--r--   0        0        0     8158 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/sharding_metadata.py
--rw-r--r--   0        0        0     5332 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/sharding_metadata_test.py
--rw-r--r--   0        0        0    10416 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/single_host_test.py
--rw-r--r--   0        0        0     7098 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/standard_checkpoint_handler.py
--rw-r--r--   0        0        0     9845 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/standard_checkpoint_handler_test_utils.py
--rw-r--r--   0        0        0     1213 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/standard_checkpointer.py
--rw-r--r--   0        0        0     9948 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0    12624 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    15251 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    66788 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    31383 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0    10277 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     2741 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/orbax/checkpoint/value_metadata.py
--rw-r--r--   0        0        0     1153 2024-03-21 21:42:35.282915 orbax_checkpoint-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 orbax_checkpoint-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/LICENSE
+-rw-r--r--   0        0        0      556 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/README.md
+-rw-r--r--   0        0        0     3433 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0    11844 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/abstract_checkpoint_manager.py
+-rw-r--r--   0        0        0     2824 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2919 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     2589 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/args.py
+-rw-r--r--   0        0        0     6886 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1377 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0    12580 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     5055 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_args.py
+-rw-r--r--   0        0        0     5447 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_args_test.py
+-rw-r--r--   0        0        0     2324 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    54299 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0    16384 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0    12282 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     7098 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0    21616 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/composite_checkpoint_handler.py
+-rw-r--r--   0        0        0    13128 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/composite_checkpoint_handler_test.py
+-rw-r--r--   0        0        0      740 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0      583 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/emergency/__init__.py
+-rw-r--r--   0        0        0    13071 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/emergency/checkpoint_manager.py
+-rw-r--r--   0        0        0     1576 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     3196 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     2018 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     7672 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0      977 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/multihost/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/multihost/utils.py
+-rw-r--r--   0        0        0    45658 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0      583 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/__init__.py
+-rw-r--r--   0        0        0     5194 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/deleter.py
+-rw-r--r--   0        0        0     2131 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/deleter_test.py
+-rw-r--r--   0        0        0     6257 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/step.py
+-rw-r--r--   0        0        0     6781 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/step_test.py
+-rw-r--r--   0        0        0      757 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/proto/__init__.py
+-rw-r--r--   0        0        0      757 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/proto/testing/__init__.py
+-rw-r--r--   0        0        0      136 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/proto/testing/foo.proto
+-rw-r--r--   0        0        0     3946 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/proto_checkpoint_handler.py
+-rw-r--r--   0        0        0    56506 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     1284 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/pytree_checkpointer.py
+-rw-r--r--   0        0        0     8907 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/random_key_checkpoint_handler.py
+-rw-r--r--   0        0        0     6883 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/random_key_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     8385 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/sharding_metadata.py
+-rw-r--r--   0        0        0     5542 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/sharding_metadata_test.py
+-rw-r--r--   0        0        0    10702 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/single_host_test.py
+-rw-r--r--   0        0        0     7098 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpoint_handler.py
+-rw-r--r--   0        0        0     9916 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpoint_handler_test_utils.py
+-rw-r--r--   0        0        0     1213 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpointer.py
+-rw-r--r--   0        0        0    10827 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0    12624 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    15251 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    65030 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    31488 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0    10277 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     2870 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/value_metadata.py
+-rw-r--r--   0        0        0     1153 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 orbax_checkpoint-0.5.8/PKG-INFO
```

### Comparing `orbax_checkpoint-0.5.7/LICENSE` & `orbax_checkpoint-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/README.md` & `orbax_checkpoint-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/__init__.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,35 +19,33 @@
 import functools
 
 import nest_asyncio
 from orbax.checkpoint import aggregate_handlers
 from orbax.checkpoint import args
 from orbax.checkpoint import checkpoint_utils
 from orbax.checkpoint import msgpack_utils
+from orbax.checkpoint import multihost
 from orbax.checkpoint import test_utils
 from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 from orbax.checkpoint import value_metadata
 from orbax.checkpoint.path import step
 
 # pylint: disable=g-importing-member, g-bad-import-order
 from orbax.checkpoint.abstract_checkpoint_manager import AbstractCheckpointManager
 from orbax.checkpoint.abstract_checkpointer import AbstractCheckpointer
 from orbax.checkpoint.array_checkpoint_handler import ArrayCheckpointHandler
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
-from orbax.checkpoint.async_checkpointer import async_checkpointer_context
 from orbax.checkpoint.async_checkpointer import AsyncCheckpointer
 from orbax.checkpoint.checkpoint_handler import CheckpointHandler
 from orbax.checkpoint.checkpoint_manager import AsyncOptions
-from orbax.checkpoint.checkpoint_manager import checkpoint_manager_context
 from orbax.checkpoint.checkpoint_manager import CheckpointManager
 from orbax.checkpoint.checkpoint_manager import CheckpointManagerOptions
 from orbax.checkpoint.checkpointer import Checkpointer
-from orbax.checkpoint.checkpointer import checkpointer_context
 from orbax.checkpoint.composite_checkpoint_handler import CompositeCheckpointHandler
 from orbax.checkpoint.future import Future
 from orbax.checkpoint.json_checkpoint_handler import JsonCheckpointHandler
 from orbax.checkpoint.proto_checkpoint_handler import ProtoCheckpointHandler
 from orbax.checkpoint.pytree_checkpoint_handler import ArrayRestoreArgs
 from orbax.checkpoint.pytree_checkpoint_handler import PyTreeCheckpointHandler
 from orbax.checkpoint.pytree_checkpoint_handler import RestoreArgs
@@ -68,8 +66,8 @@
   nest_asyncio.apply()
 except RuntimeError:
   pass
 
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
 # Also modify version and date in CHANGELOG.
-__version__ = '0.5.7'
+__version__ = '0.5.8'
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/abstract_checkpoint_manager.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/abstract_checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/abstract_checkpointer.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/aggregate_handlers.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/args.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/args.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/array_checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,14 @@
       commit_futures = await self.async_save(directory, *args, **kwargs)  # pytype: disable=bad-return-type
       # Futures are already running, so sequential waiting is equivalent to
       # concurrent waiting.
       for f in commit_futures:
         f.result()  # Block on result.
 
     asyncio.run(async_save())
-    utils.sync_global_devices('ArrayCheckpointHandler:save')
 
   def restore(
       self,
       directory: epath.Path,
       item: Optional[ArrayType] = None,
       restore_args: Optional[type_handlers.RestoreArgs] = None,
       args: Optional['ArrayRestoreArgs'] = None,
@@ -164,15 +163,14 @@
       if restore_type is None:
         restore_type = type_handlers.default_restore_type(restore_args)
       type_handler = type_handlers.get_type_handler(restore_type)
       result = asyncio.run(
           type_handler.deserialize([info], args=[restore_args])
       )[0]
 
-    utils.sync_global_devices('ArrayCheckpointHandler:restore')
     return result
 
   def finalize(self, directory: epath.Path):
     type_handlers.merge_ocdbt_per_process_files(directory)
 
   def close(self):
     """See superclass documentation."""
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/async_checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/async_checkpointer.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/async_checkpointer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """AsyncCheckpointer."""
 
 import asyncio
-import contextlib
 import itertools
 import threading
 import time
-from typing import Any, Callable, Optional, Protocol, Sequence
+from typing import Any, Callable, Optional, Protocol, Sequence, Set
 
 from absl import logging
 from etils import epath
 import jax
 from orbax.checkpoint import async_checkpoint_handler
 from orbax.checkpoint import checkpoint_args
 from orbax.checkpoint import checkpointer
@@ -242,30 +241,34 @@
   """
 
   # Options mirror checkpoint_manager.AsyncOptions.
   def __init__(
       self,
       handler: async_checkpoint_handler.AsyncCheckpointHandler,
       timeout_secs: int = 300,
-      primary_host: Optional[int] = 0,
       *,
+      primary_host: Optional[int] = 0,
+      # TODO(b/331426277): Support this option when async-compatible barrier
+      # is provided.
+      active_processes: Optional[Set[int]] = None,
       barrier_sync_fn: Optional[BarrierSyncFn] = None,
   ):
     jax.monitoring.record_event('/jax/orbax/async_checkpointer/init')
     if not checkpoint_args.has_registered_args(handler):
       logging.warning(
           'No registered CheckpointArgs found for handler type: %s',
           type(handler),
       )
       handler = checkpointer.get_legacy_handler_wrapper(handler)
       assert isinstance(
           handler, async_checkpoint_handler.AsyncCheckpointHandler
       )
     self._handler = handler
     self._primary_host = primary_host
+    self._active_processes = active_processes
 
     # TODO(dicentra): consider folding into AsyncCheckpointer directly.
     self._async_manager = _AsyncManager(
         timeout_secs=timeout_secs,
         primary_host=primary_host,
         barrier_sync_fn=barrier_sync_fn or _get_barrier_sync_fn(),
     )
@@ -349,34 +352,7 @@
     """Waits to finish any outstanding operations before closing."""
     self.wait_until_finished()
     super().close()
 
   @property
   def handler(self) -> async_checkpoint_handler.AsyncCheckpointHandler:
     return self._handler
-
-
-@contextlib.contextmanager
-def async_checkpointer_context(*args, **kwargs):
-  """Context manager for AsyncCheckpointer.
-
-  Initializes AsyncCheckpointer and closes the object when the context is
-  exited.
-
-  Usage::
-    with async_checkpointer_context(PyTreeCheckpointHandler()) as ckptr:
-      ckptr.save(...)
-      ckptr.wait_until_finished()
-      ckptr.restore(...)
-
-  Args:
-    *args: Arguments to initialize AsyncCheckpointer.
-    **kwargs: Keyword arguments to initialize AsyncCheckpointer.
-
-  Yields:
-    AsyncCheckpointer
-  """
-  ckptr = AsyncCheckpointer(*args, **kwargs)
-  try:
-    yield ckptr
-  finally:
-    ckptr.close()
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_args.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_args.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_args_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_args_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests CheckpointArg registration."""
+
 import dataclasses
 from absl.testing import absltest
 from orbax.checkpoint import checkpoint_args
 from orbax.checkpoint import checkpoint_handler
 from orbax.checkpoint import standard_checkpoint_handler
 
 StandardCheckpointHandler = (
@@ -133,10 +134,47 @@
     self.assertIs(restore_args, MyHandlerArgs)
     save_args, restore_args = checkpoint_args.get_registered_args_cls(
         MyCheckpointHandler()
     )
     self.assertIs(save_args, MyHandlerArgs)
     self.assertIs(restore_args, MyHandlerArgs)
 
+  def test_get_registered_args_cls_single_handler_multiple_args(self):
+    class MyCheckpointHandler(checkpoint_handler.CheckpointHandler):
+
+      def save(self, *args, **kwargs):
+        pass
+
+      def restore(self, *args, **kwargs):
+        pass
+
+    # Register first CheckpointArgs to MyCheckpointHandler.
+    @checkpoint_args.register_with_handler(
+        MyCheckpointHandler, for_save=True, for_restore=True
+    )
+    @dataclasses.dataclass
+    class Args1(checkpoint_args.CheckpointArgs):
+      pass
+
+    # Register second CheckpointArgs to MyCheckpointHandler.
+    @checkpoint_args.register_with_handler(
+        MyCheckpointHandler, for_save=True, for_restore=True
+    )
+    @dataclasses.dataclass
+    class Args2(checkpoint_args.CheckpointArgs):
+      pass
+
+    save_args, restore_args = checkpoint_args.get_registered_args_cls(
+        MyCheckpointHandler
+    )
+    self.assertIs(save_args, Args1)
+    self.assertIs(restore_args, Args1)
+
+    save_args, restore_args = checkpoint_args.get_registered_args_cls(
+        MyCheckpointHandler()
+    )
+    self.assertIsNot(save_args, Args2)
+    self.assertIsNot(restore_args, Args2)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_manager.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,38 +11,39 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A class providing functionalities for managing a series of checkpoints."""
 
 import concurrent.futures
-import contextlib
 import dataclasses
 import datetime
 import threading
 import time
 import typing
-from typing import Any, Callable, Container, List, Mapping, Optional, Sequence, Tuple, Type, Union
-
+from typing import Any, Callable, Container, Iterable, List, Mapping, Optional, Sequence, Set, Tuple, Type, Union
 from absl import logging
 from etils import epath
+from etils import epy
 import jax
 from jax.experimental.array_serialization import serialization
 from orbax.checkpoint import abstract_checkpoint_manager
 from orbax.checkpoint import abstract_checkpointer
 from orbax.checkpoint import args as args_lib
 from orbax.checkpoint import async_checkpointer
 from orbax.checkpoint import checkpoint_args
 from orbax.checkpoint import checkpoint_handler
 from orbax.checkpoint import checkpointer as checkpointer_lib
 from orbax.checkpoint import composite_checkpoint_handler
 from orbax.checkpoint import json_checkpoint_handler
 from orbax.checkpoint import proto_checkpoint_handler
 from orbax.checkpoint import utils
+from orbax.checkpoint.path import deleter
 from orbax.checkpoint.path import step as step_lib
+from typing_extensions import Self  # for Python version < 3.11
 
 
 PyTree = Any
 CheckpointDirs = Tuple[str, str]
 SaveParams = Mapping[str, Any]
 RestoreParams = SaveParams
 AbstractCheckpointer = abstract_checkpointer.AbstractCheckpointer
@@ -122,14 +123,33 @@
   See `AsyncCheckpointer` for details.
   """
 
   timeout_secs: int = 300
   barrier_sync_fn: Optional[async_checkpointer.BarrierSyncFn] = None
 
 
+@dataclasses.dataclass
+class MultiprocessingOptions:
+  """Options used to configure multiprocessing behavior.
+
+  primary_host: the host id of the primary host.  Default to 0.  If it's set
+    to None, then all hosts will be considered as primary.  It's useful in
+    the case that all hosts are only working with local storage.
+  active_processes: A set of process indices (corresponding to
+    `jax.process_index()`) over which `CheckpointManager` is expected to be
+    called. This makes it possible to have a `CheckpointManager` instance
+    that runs over a subset of processes, rather than all processes as it is
+    normally expected to do. If specified, `primary_host` must belong to
+    `active_processes`.
+  """
+
+  primary_host: Optional[int] = 0
+  active_processes: Optional[Set[int]] = None
+
+
 # TODO(b/309965339) Set todelete_subdir defaults if directory is on CNS.
 @dataclasses.dataclass
 class CheckpointManagerOptions:
   """Optional arguments for CheckpointManager.
 
   save_interval_steps:
     The interval at which checkpoints should be saved.
@@ -189,14 +209,18 @@
     every host. This can be helpful to reduce QPS to the filesystem if there
     are a large number of hosts.
   todelete_subdir: If set, checkpoints to be deleted will be only renamed into a
     subdirectory with the provided string. Otherwise, they will be directly
     deleted from the file system. Useful if checkpoint deletion is time
     consuming. By default, delete the checkpoint assets. Ignored if file system
     is Google Cloud Storage (directory is prefixed with gs://)
+  enable_background_delete: If True, old checkpoint deletions will be done in a
+    background thread, otherwise, it will be done at the end of each save.  When
+    it's enabled, make sure to call CheckpointManager.close() or use context to
+    make sure all old steps are deleted before exit.
   read_only: If True, then checkpoints save and delete are skipped. However,
     checkpoints restore works as usual.
   enable_async_checkpointing: If True, enables async checkpointing.
   async_options: Used to configure properties of async behavior. See above.
   """
 
   save_interval_steps: int = 1
@@ -210,17 +234,21 @@
   step_format_fixed_length: Optional[int] = None
   step_name_format: Optional[step_lib.NameFormat] = None
   create: bool = True
   cleanup_tmp_directories: bool = False
   save_on_steps: Optional[Container[int]] = None
   single_host_load_and_broadcast: bool = False
   todelete_subdir: Optional[str] = None
+  enable_background_delete: bool = False
   read_only: bool = False
   enable_async_checkpointing: bool = True
   async_options: Optional[AsyncOptions] = None
+  multiprocessing_options: MultiprocessingOptions = dataclasses.field(
+      default_factory=MultiprocessingOptions
+  )
 
   def __post_init__(self):
     if self.best_mode not in ('min', 'max'):
       msg = (
           "`CheckpointManagerOptions.best_mode` must be one of None, 'min' "
           "or 'max'. Got {self.dtype}."
       )
@@ -308,30 +336,29 @@
     )
   for key, handler in handler._known_handlers.items():  # pylint: disable=protected-access
     if key == item_name:
       return checkpoint_args.get_registered_args_cls(handler)
   raise ValueError(f'Unknown key "{item_name}" in CompositeCheckpointHandler.')
 
 
-class CheckpointManager(AbstractCheckpointManager):
+class CheckpointManager(AbstractCheckpointManager, epy.ContextManager):
   """A generic, synchronous AbstractCheckpointManager implementation."""
 
   def __init__(
       self,
       directory: epath.PathLike,
       checkpointers: Optional[
           Union[AbstractCheckpointer, CheckpointersDict]
       ] = None,
       options: Optional[CheckpointManagerOptions] = None,
       metadata: Optional[Mapping[str, Any]] = None,
       item_names: Optional[Sequence[str]] = None,
       item_handlers: Optional[
           Union[CheckpointHandler, CheckpointHandlersDict]
       ] = None,
-      primary_host: Optional[int] = 0,
   ):
     """CheckpointManager constructor.
 
     IMPORTANT: `CheckpointManager` has been refactored to provide a new API.
     Please ensure you have migrated all existing use cases to the newer style by
     May 1st, 2024. Please see
     https://orbax.readthedocs.io/en/latest/api_refactor.html
@@ -341,48 +368,55 @@
     which saving and restoring is delegated. Behind step management options,
     metrics-related logic, and other frills, saving and restoring with
     `CheckpointManager` is quite similar to using
     `Checkpointer(CompositeCheckpointHandler)`.
 
     Example::
 
-      mngr = CheckpointManager(
+      with CheckpointManager(
         'path/to/dir/',
         # Multiple items.
         item_names=('train_state', 'custom_metadata'),
         metadata={'version': 1.1, 'lang': 'en'},
-      )
-      mngr.save(0, args=args.Composite(
-          train_state=args.StandardSave(train_state),
-          custom_metadata=args.JsonSave(custom_metadata),
+      ) as mngr:
+        mngr.save(0, args=args.Composite(
+            train_state=args.StandardSave(train_state),
+            custom_metadata=args.JsonSave(custom_metadata),
+          )
         )
-      )
-      restored = mngr.restore(0)
-      print(restored.train_state)
-      print(restored.custom_metadata)
-      restored = mngr.restore(0, args=args.Composite(
-          train_state=args.StandardRestore(abstract_train_state),
+        restored = mngr.restore(0)
+        print(restored.train_state)
+        print(restored.custom_metadata)
+        restored = mngr.restore(0, args=args.Composite(
+            train_state=args.StandardRestore(abstract_train_state),
+          )
         )
-      )
-      print(restored.train_state)
-      print(restored.custom_metadata)  # Error, not restored
+        print(restored.train_state)
+        print(restored.custom_metadata)  # Error, not restored
 
       # Single item, no need to specify `item_names`.
-      mngr = CheckpointManager(
-        'path/to/dir/',
-        options = CheckpointManagerOptions(max_to_keep=5, ...),
-      )
-      mngr.save(0, args=StandardSave(train_state))
-      train_state = mngr.restore(0)
-      train_state = mngr.restore(0, args=StandardRestore(abstract_train_state))
+      with CheckpointManager(
+          'path/to/dir/',
+          options = CheckpointManagerOptions(max_to_keep=5, ...),
+        ) as mngr:
+        mngr.save(0, args=StandardSave(train_state))
+        train_state = mngr.restore(0)
+        train_state = mngr.restore(0,
+        args=StandardRestore(abstract_train_state))
 
     IMPORTANT: Don't forget to use the keyword `args=...` for save and restore!
     Otherwise you will get the legacy API. This will not be necessary forever,
     but only until the legacy API is removed.
 
+    IMPORTANT: The CheckpointManager is designed to be used as a context
+    manager. Use `with CheckpointManager` schematic for automatic cleanup. If
+    you can't use a context manager, always call `close()` to release resources
+    properly.  Otherwise, background operations such as deleting old checkpoints
+    might not finish before your program exits.
+
     Args:
       directory: the top level directory in which to save all files.
       checkpointers: a mapping of object name to Checkpointer object. For
         example, `items` provided to `save` below should have keys matching the
         keys in this argument. Alternatively, a single Checkpointer may be
         provided, in which case `save` and `restore` should always be called
         with a single item rather than a dictionary of items. See below for more
@@ -405,25 +439,24 @@
       item_handlers: A mapping of item name to `CheckpointHandler`. The mapped
         CheckpointHandler must be registered against the `CheckpointArgs` input
         in save/restore operations. Please don't use `checkpointers` and
         `item_handlers` together. It can be used with or without `item_names`.
         The item name key may or may not be present in `item_names`.
         Alternatively, a single CheckpointHandler may be provided, in which case
         `save` and `restore` should always be called in a single item context.
-      primary_host: the host id of the primary host.  Default to 0.  If it's set
-        to None, then all hosts will be considered as primary.  It's useful in
-        the case that all hosts are only working with local storage.
     """
     jax.monitoring.record_event('/jax/orbax/checkpoint_manager/init')
 
     self._options = options or CheckpointManagerOptions()
     if self._options.best_mode not in ['min', 'max']:
       raise ValueError('`best_mode` must be one of: "min", "max"')
 
-    self._primary_host = primary_host
+    self._multiprocessing_options = (
+        self._options.multiprocessing_options or MultiprocessingOptions()
+    )
 
     if checkpointers and item_names:
       raise ValueError(
           '`item_names` and `checkpointers` are mutually exclusive - do not use'
           ' together.'
       )
     if checkpointers and item_handlers:
@@ -456,72 +489,109 @@
       )
 
     self._directory = epath.Path(directory)
     if self._options.read_only:
       logging.warning('Given directory is read only=%s', self._directory)
     if self._options.create:
       if (
-          utils.is_primary_host(self._primary_host)
+          utils.is_primary_host(self._multiprocessing_options.primary_host)
           and not self._directory.exists()
       ):
         self._directory.mkdir(parents=True)
-      utils.sync_global_devices('CheckpointManager:create_directory')
+      utils.sync_global_processes(
+          'CheckpointManager:create_directory',
+          processes=self._multiprocessing_options.active_processes,
+      )
 
 
     # Cleanup directories from previous runs that may not have been finalized.
     if self._options.cleanup_tmp_directories:
       self._cleanup_tmp_directories()
 
+    self._step_name_format = (
+        self._options.step_name_format
+        or step_lib.StandardNameFormat(
+            step_prefix=self._options.step_prefix,
+            step_format_fixed_length=self._options.step_format_fixed_length,
+        )
+    )
+
     self._checkpoints = self._create_checkpoints()
 
+    self._metadata_checkpointer = Checkpointer(
+        JsonCheckpointHandler(
+            primary_host=self._multiprocessing_options.primary_host
+        ),
+        primary_host=self._multiprocessing_options.primary_host,
+        active_processes=self._multiprocessing_options.active_processes,
+    )
     if self._options.read_only and not self._metadata_path().exists():
       self._metadata = {} if metadata is None else metadata
     else:
       self._metadata = None
     if metadata is not None and not self._options.read_only:
       self._save_metadata(metadata)
 
     self._finalize_thread = None
+
+    self._checkpoint_deleter: deleter.CheckpointDeleter = (
+        deleter.create_checkpoint_deleter(
+            self._multiprocessing_options.primary_host,
+            self._directory,
+            self._options.todelete_subdir,
+            self._step_name_format,
+            self._options.enable_background_delete,
+        )
+    )
+
     logging.info(
         'jax.process_index=%s, primary_host=%s. CheckpointManager created: %s',
         jax.process_index(),
-        self._primary_host,
+        self._multiprocessing_options.primary_host,
         self,
     )
 
   def _configure_checkpointer_common(
       self,
       handler: CompositeCheckpointHandler,
       options: CheckpointManagerOptions,
       use_async: bool,
   ) -> Checkpointer:
     if use_async:
       if options.async_options is not None:
         return async_checkpointer.AsyncCheckpointer(
             handler,
             timeout_secs=options.async_options.timeout_secs,
-            primary_host=self._primary_host,
+            primary_host=self._multiprocessing_options.primary_host,
             barrier_sync_fn=options.async_options.barrier_sync_fn,
+            active_processes=self._multiprocessing_options.active_processes,
         )
       else:
         return async_checkpointer.AsyncCheckpointer(
-            handler, primary_host=self._primary_host
+            handler,
+            primary_host=self._multiprocessing_options.primary_host,
+            active_processes=self._multiprocessing_options.active_processes,
         )
     else:
-      return Checkpointer(handler, primary_host=self._primary_host)
+      return Checkpointer(
+          handler,
+          primary_host=self._multiprocessing_options.primary_host,
+          active_processes=self._multiprocessing_options.active_processes,
+      )
 
   def _configure_checkpointer_legacy_init(
       self,
       checkpointers: Union[AbstractCheckpointer, CheckpointersDict],
       options: CheckpointManagerOptions,
   ) -> Checkpointer:
     """Initializes _CompositeCheckpointer with legacy style checkpointers."""
-    if self._primary_host != 0:
+    if self._multiprocessing_options.primary_host != 0:
       raise ValueError(
-          f'`primary_host`={self._primary_host} is not supported in legacy API.'
+          f'`primary_host`={self._multiprocessing_options.primary_host} is not'
+          ' supported in legacy API.'
       )
 
     item_handlers = {}
     if isinstance(checkpointers, Checkpointer):
       use_async = is_async_checkpointer(checkpointers)
       if isinstance(checkpointers, async_checkpointer.AsyncCheckpointer):
         async_timeout = checkpointers._async_manager._timeout_secs  # pylint: disable=protected-access
@@ -570,41 +640,47 @@
         filename=METRIC_ITEM_NAME
     )
     options.async_options = options.async_options or AsyncOptions(
         timeout_secs=async_timeout
     )
     return self._configure_checkpointer_common(
         CompositeCheckpointHandler(
-            primary_host=self._primary_host,
+            composite_options=composite_checkpoint_handler.CompositeOptions(
+                primary_host=self._multiprocessing_options.primary_host,
+            ),
             **item_handlers,
         ),
         options,
         use_async,
     )
 
 
   def _validate_handler(self, handler):
     if (
         hasattr(handler, '_primary_host')
-        and handler._primary_host != self._primary_host  # pylint: disable=protected-access
+        and handler._primary_host != self._multiprocessing_options.primary_host  # pylint: disable=protected-access
     ):
       raise ValueError(
-          f'Inconsistent primary_host, CheckpointManager={self._primary_host}, '
+          'Inconsistent primary_host,'
+          f' CheckpointManager={self._multiprocessing_options.primary_host}, '
           f'handler[{type(handler)}]={handler._primary_host} '  # pylint: disable=protected-access
       )
 
   def _configure_checkpointer(
       self,
       item_names: Optional[Sequence[str]],
       item_handlers: Optional[Union[CheckpointHandler, CheckpointHandlersDict]],
       options: CheckpointManagerOptions,
       single_item: bool,
   ) -> Checkpointer:
     """Initializes _CompositeCheckpointer given `item_names`."""
-    if self._primary_host is None and item_handlers is None:
+    if (
+        self._multiprocessing_options.primary_host is None
+        and item_handlers is None
+    ):
       raise ValueError(
           'When primary_host is set to None, item_handlers must be provided to'
           ' match with the primary_host setting.'
       )
     if single_item:
       item_handler = (
           item_handlers
@@ -629,21 +705,24 @@
     for item_name in all_item_handlers:
       if item_name in RESERVED_ITEM_NAMES:
         raise ValueError(
             f'Found {item_name} in `checkpointers`; this is a reserved key.'
         )
     if options.best_fn:
       all_item_handlers[METRIC_ITEM_NAME] = JsonCheckpointHandler(
-          filename=METRIC_ITEM_NAME, primary_host=self._primary_host
+          filename=METRIC_ITEM_NAME,
+          primary_host=self._multiprocessing_options.primary_host,
       )
     # CompositeCheckpointHandler defers per-item handler creation until
     # save/restore time.
     return self._configure_checkpointer_common(
         CompositeCheckpointHandler(
-            primary_host=self._primary_host,
+            composite_options=composite_checkpoint_handler.CompositeOptions(
+                primary_host=self._multiprocessing_options.primary_host,
+            ),
             **all_item_handlers,
         ),
         options,
         options.enable_async_checkpointing,
     )
 
   @property
@@ -713,22 +792,16 @@
 
   def _get_save_directory(
       self,
       step: int,
       directory: epath.Path,
   ) -> epath.Path:
     """Returns the standardized path to a save directory for a single item."""
-    step_name_format = (
-        self._options.step_name_format
-        or step_lib.StandardNameFormat(
-            step_prefix=self._options.step_prefix,
-            step_format_fixed_length=self._options.step_format_fixed_length,
-        )
-    )
-    return step_lib.build_step_path(directory, step_name_format, step)
+
+    return step_lib.build_step_path(directory, self._step_name_format, step)
 
   def _get_write_step_directory(
       self, step: int, root_dir: epath.Path
   ) -> epath.Path:
     return self._get_save_directory(step, root_dir)
 
   def _get_read_step_directory(
@@ -737,25 +810,39 @@
     if self._options.step_name_format is not None:
       return self._options.step_name_format.find_step(root_dir, step).path
     else:
       return self._get_save_directory(step, root_dir)
 
   def _create_tmp_directory(self, directory: epath.Path) -> epath.Path:
     """Creates a tmp directory based on the given directory."""
-    return utils.create_tmp_directory(directory)
+    return utils.create_tmp_directory(
+        directory,
+        primary_host=self._multiprocessing_options.primary_host,
+        active_processes=self._multiprocessing_options.active_processes,
+    )
 
   def delete(self, step: int):
-    """See superclass documentation."""
+    """See superclass documentation.
+
+    Delete can be run asynchronously if
+    CheckpointManagerOptions.enable_background_delete is set to True.
+
+    Args:
+      step: The step to delete.
+    """
     if self._options.read_only:
       logging.warning('%s is read only, delete will be skipped', self.directory)
       return
     if step not in self.all_steps():
       raise ValueError(f'Requested deleting a non-existent step: {step}.')
-    self._delete_directory(step)
-    utils.sync_global_devices('CheckpointManager:deleted_step')
+    self._checkpoint_deleter.delete(step)
+    utils.sync_global_processes(
+        'CheckpointManager:deleted_step',
+        processes=self._multiprocessing_options.active_processes,
+    )
     for i, info in enumerate(self._checkpoints):
       if info.step == step:
         self._checkpoints.pop(i)
 
   def _validate_args(
       self,
       items: Optional[Union[Any, Mapping[str, Any]]],
@@ -856,26 +943,37 @@
     args = args_lib.Composite(**args_dict)
 
     save_directory = self._get_write_step_directory(step, self.directory)
     # If a folder for the step to save exists and is not finalized, remove the
     # existing folder.
     if utils.is_gcs_path(self.directory):
       if (
-          utils.is_primary_host(self._primary_host)
+          utils.is_primary_host(self._multiprocessing_options.primary_host)
           and save_directory.exists()
           and utils.is_tmp_checkpoint(save_directory)
       ):
         logging.warning(
             'Attempting to save on GCS at step %s which has an unfinalized'
             ' checkpoint from previous runs. Removing the unfinalized'
             ' checkpoint before saving.',
             step,
         )
-        self._delete_directory(step)
-      utils.sync_global_devices('CheckpointManager:delete_unfinalized_step_gcs')
+
+        # make sure to use a synchronous deleter here
+        deleter.create_checkpoint_deleter(
+            self._multiprocessing_options.primary_host,
+            self._directory,
+            self._options.todelete_subdir,
+            self._step_name_format,
+            False,  # no background thread
+        ).delete(step)
+      utils.sync_global_processes(
+          'CheckpointManager:delete_unfinalized_step_gcs',
+          processes=self._multiprocessing_options.active_processes,
+      )
 
     self._checkpointer.save(save_directory, args=args)
 
     self._add_checkpoint_info(step, metrics)
     get_old_steps_start_time = time.time()
     steps_to_remove = self._get_old_steps_to_remove()
     jax.monitoring.record_event_duration_secs(
@@ -884,28 +982,34 @@
     )
     self._checkpoints = [
         info for info in self._checkpoints if info.step not in steps_to_remove
     ]
     # Sync needed to ensure that old steps to remove are retrieved before
     # actually deleting them during finalize, since retrieval can involve
     # looking at the directory.
-    utils.sync_global_devices('CheckpointManager:old_steps_to_remove')
+    utils.sync_global_processes(
+        'CheckpointManager:old_steps_to_remove',
+        processes=self._multiprocessing_options.active_processes,
+    )
 
     assert self._finalize_thread is None
     if is_async_checkpointer(self._checkpointer):
       logging.info('Beginning async checkpoint finalize.')
       t = _FinalizeThread(
           target=self._finalize, args=(save_directory, steps_to_remove)
       )
       t.start()
       self._finalize_thread = t
     else:
       self._finalize(save_directory, steps_to_remove)
       logging.info('Finished synchronous save.')
-      utils.sync_global_devices('CheckpointManager:finalize')
+      utils.sync_global_processes(
+          'CheckpointManager:finalize',
+          processes=self._multiprocessing_options.active_processes,
+      )
     return True
 
   def restore(
       self,
       step: int,
       items: Optional[Union[Any, Mapping[str, Any]]] = None,
       restore_kwargs: Optional[
@@ -1069,24 +1173,22 @@
   def _metadata_path(self) -> epath.Path:
     return self.directory / METADATA_ITEM_NAME
 
   def _save_metadata(self, metadata: Mapping[str, Any]):
     """Saves CheckpointManager level metadata, skips if already present."""
     path = self._metadata_path()
     if not path.exists():  # May have been created by a previous run.
-      checkpointer = Checkpointer(JsonCheckpointHandler())
-      checkpointer.save(path, metadata)
+      self._metadata_checkpointer.save(path, metadata)
 
   def metadata(self) -> Mapping[str, Any]:
     """See superclass documentation."""
     if self._metadata is None:
       path = self._metadata_path()
       if path.exists():
-        checkpointer = Checkpointer(JsonCheckpointHandler())
-        self._metadata = checkpointer.restore(path)
+        self._metadata = self._metadata_checkpointer.restore(path)
       else:
         self._metadata = {}
     return self._metadata
 
   def _sort_checkpoints_by_metrics(
       self, checkpoints: List[CheckpointInfo]
   ) -> Tuple[List[CheckpointInfo], List[CheckpointInfo]]:
@@ -1107,43 +1209,19 @@
     return without_metrics, sorted(
         with_metrics,
         key=lambda info: self._options.best_fn(info.metrics),
         reverse=(self._options.best_mode == 'min'),
     )
 
   def _cleanup_tmp_directories(self):
-    utils.cleanup_tmp_directories(self.directory)
-
-  def _delete_directory(self, step: int):
-    """Deletes step dir or renames it if options.todelete_subdir is set.
-
-    See `CheckpointManagerOptions.todelete_subdir` for details.
-
-    Args:
-      step: checkpointing step number.
-    """
-    if not utils.is_primary_host(self._primary_host):
-      return
-
-    # Delete if storage is on gcs or todelete_subdir is not set.
-    if self._options.todelete_subdir is None or utils.is_gcs_path(
-        self.directory
-    ):
-      self._get_read_step_directory(step, self.directory).rmtree()
-      logging.info('Deleted step %d.', step)
-      return
-
-    # Rename step dir.
-    rename_dir = self.directory / self._options.todelete_subdir
-    if not rename_dir.exists():
-      rename_dir.mkdir(parents=True)
-    src = self._get_read_step_directory(step, self.directory)
-    dst = self._get_write_step_directory(step, rename_dir)
-    src.replace(dst)
-    logging.info('Renamed step %d (todelete_subdir option specified).', step)
+    utils.cleanup_tmp_directories(
+        self.directory,
+        primary_host=self._multiprocessing_options.primary_host,
+        active_processes=self._multiprocessing_options.active_processes,
+    )
 
   def _get_old_steps_to_remove(self) -> List[int]:
     """Returns checkpoints that should be deleted."""
     # Must have set max_to_keep in order to remove any checkpoints.
     if self._options.max_to_keep is None:
       return []
     # Not enough checkpoints accumulated to consider deletion.
@@ -1154,25 +1232,19 @@
     # we abuse a duration metric to count the number of steps examined.
     jax.monitoring.record_event_duration_secs(
         '/jax/checkpoint/write/old_steps_examined_count',
         len(self._checkpoints),
     )
 
     # Exclude the latest checkpoint, since it is not finalized.
-    step_name_format = (
-        self._options.step_name_format
-        or step_lib.StandardNameFormat(
-            step_prefix=self._options.step_prefix,
-            step_format_fixed_length=self._options.step_format_fixed_length,
-        )
-    )
+
     are_locked = utils.are_locked(
         self.directory,
         steps=tuple([info.step for info in self._checkpoints[:-1]]),
-        step_name_format=step_name_format,
+        step_name_format=self._step_name_format,
     )
     self._checkpoints[:-1] = [
         dataclasses.replace(info, is_locked=is_locked)
         for info, is_locked in zip(self._checkpoints, are_locked)
     ]
 
     if self._track_best:
@@ -1271,15 +1343,18 @@
         # save, we clean up since that checkpoint was never actually saved.
         assert self._checkpoints
         self._checkpoints = self._checkpoints[:-1]
         raise e
       # Additional work is being done on process 0 of the finalize threads.
       # When joining the threads, we must wait for all threads to complete
       # before proceeding.
-      utils.sync_global_devices('CheckpointManager:join_finalize_thread')
+      utils.sync_global_processes(
+          'CheckpointManager:join_finalize_thread',
+          processes=self._multiprocessing_options.active_processes,
+      )
 
   def check_for_errors(self):
     """See superclass documentation."""
     if is_async_checkpointer(self._checkpointer):
       self._checkpointer.check_for_errors()  # pytype: disable=attribute-error
 
   def _finalize_checkpoint(self, step: int):
@@ -1287,15 +1362,15 @@
 
     * Logs error if any.
     * Records duration saved due to preemption if any.
 
     Args:
       step: finalized checkpoint step.
     """
-    if utils.is_primary_host(self._primary_host):
+    if utils.is_primary_host(self._multiprocessing_options.primary_host):
       try:
         self.check_for_errors()
       except Exception as e:  # pylint: disable=broad-except
         logging.error(
             (
                 'Received error: %s from Checkpointer. One or more items may'
                 ' not be finalized. Skipping finalization of step checkpoint.'
@@ -1322,46 +1397,26 @@
   def _finalize(self, directory: epath.Path, steps_to_remove: List[int]):
     """Cleans up old checkpoints and synchronizes hosts."""
     self._wait_for_checkpointers()
     # If an error is encountered while waiting for commit futures to complete,
     # we will not proceed past this point.
     self._finalize_checkpoint(utils.step_from_checkpoint_name(directory.name))
     remove_steps_start_time = time.time()
-    for step in steps_to_remove:
-      self._delete_directory(step)
+    self._checkpoint_deleter.delete_steps(steps_to_remove)
     jax.monitoring.record_event_duration_secs(
         '/jax/checkpoint/write/remove_steps_duration_secs',
         time.time() - remove_steps_start_time,
     )
 
   def close(self):
     """See superclass documentation."""
     self.wait_until_finished()
     self._checkpointer.close()
+    self._checkpoint_deleter.close()
 
-
-@contextlib.contextmanager
-def checkpoint_manager_context(*args, **kwargs):
-  """Context manager for CheckpointManager.
-
-  Initializes CheckpointManager and closes the object when the context is
-  exited.
-
-  Args:
-    *args: Arguments to initialize CheckpointManager.
-    **kwargs: Keyword arguments to initialize CheckpointManager.
-
-  Usage::
-
-    with checkpoint_manager_context(
-        directory, checkpointers, options) as mngr:
-      mngr.save(...)
-      mngr.all_steps()
-
-  Yields:
-    CheckpointManager
-  """
-  manager = CheckpointManager(*args, **kwargs)
-  try:
-    yield manager
-  finally:
-    manager.close()
+  def __contextmanager__(
+      self,
+  ) -> Iterable[Self]:
+    try:
+      yield self
+    finally:
+      self.close()
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_utils.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/checkpoint_utils_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/checkpointer.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpointer.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Synchronous Checkpointer implementation."""
 
-import contextlib
 import time
-from typing import Any, Optional
+from typing import Any, Iterable, Optional, Set
 
 from absl import logging
 from etils import epath
+from etils import epy
 import jax
 from orbax.checkpoint import abstract_checkpointer
 from orbax.checkpoint import checkpoint_args
 from orbax.checkpoint import checkpoint_handler
 from orbax.checkpoint import checkpoint_utils
 from orbax.checkpoint import composite_checkpoint_handler
 from orbax.checkpoint import utils
+from typing_extensions import Self  # for Python version < 3.11
 
 
 
 CheckpointArgs = checkpoint_args.CheckpointArgs
 register_with_handler = checkpoint_args.register_with_handler
 get_legacy_handler_wrapper = (
     composite_checkpoint_handler.get_legacy_handler_wrapper
@@ -55,15 +56,17 @@
   )
   if for_save:
     return save_arg_cls(*args, **kwargs)
   else:
     return restore_arg_cls(*args, **kwargs)
 
 
-class Checkpointer(abstract_checkpointer.AbstractCheckpointer):
+class Checkpointer(
+    abstract_checkpointer.AbstractCheckpointer, epy.ContextManager
+):
   """A synchronous implementation of AbstractCheckpointer.
 
   This class saves synchronously to a given directory using an underlying
   `CheckpointHandler`. Atomicity of the operation is guaranteed.
 
   IMPORTANT: Async checkpointing can often be faster for saving. Strongly
   consider using `AsyncCheckpointer` instead.
@@ -91,30 +94,30 @@
     ckptr.restore(path, state=abstract_pytree_target)
   """
 
   def __init__(
       self,
       handler: checkpoint_handler.CheckpointHandler,
       primary_host: Optional[int] = 0,
+      active_processes: Optional[Set[int]] = None,
   ):
     if not checkpoint_args.has_registered_args(handler):
       logging.warning(
           'No registered CheckpointArgs found for handler type: %s',
           type(handler),
       )
       handler = get_legacy_handler_wrapper(handler)
     self._handler = handler
     self._primary_host = primary_host
+    self._active_processes = active_processes
     jax.monitoring.record_event('/jax/orbax/checkpointer/init')
 
-  def save(self,
-           directory: epath.PathLike,
-           *args,
-           force: bool = False,
-           **kwargs):
+  def save(
+      self, directory: epath.PathLike, *args, force: bool = False, **kwargs
+  ):
     """Saves the given item to the provided directory.
 
     Delegates to the underlying CheckpointHandler. Ensures save operation
     atomicity.
 
     This method should be called by all hosts - process synchronization and
     actions that need to be performed on only one host are managed internally.
@@ -137,40 +140,40 @@
       if force:
         if utils.is_primary_host(self._primary_host):
           logging.info('Specified `force`: removing existing directory.')
           directory.rmtree()  # Post-sync handled by create_tmp_directory.
       else:
         raise ValueError(f'Destination {directory} already exists.')
     tmpdir = utils.create_tmp_directory(
-        directory, primary_host=self._primary_host
+        directory,
+        primary_host=self._primary_host,
+        active_processes=self._active_processes,
     )
     ckpt_args = construct_checkpoint_args(self._handler, True, *args, **kwargs)
     self._handler.save(tmpdir, args=ckpt_args)
-    utils.sync_global_devices('Checkpointer:write')
+    utils.sync_global_processes('Checkpointer:write', self._active_processes)
 
     # Ensure save operation atomicity and record time saved by checkpoint.
     if utils.is_primary_host(self._primary_host):
       self._handler.finalize(tmpdir)
       utils.on_commit_callback(tmpdir, directory, checkpoint_start_time)
-    utils.sync_global_devices('Checkpointer:save')
+    utils.sync_global_processes('Checkpointer:save', self._active_processes)
 
-  def restore(self,
-              directory: epath.PathLike,
-              *args,
-              **kwargs) -> Any:
+  def restore(self, directory: epath.PathLike, *args, **kwargs) -> Any:
     """See superclass documentation."""
     directory = epath.Path(directory)
     if not directory.exists():
       raise FileNotFoundError(f'Checkpoint at {directory} not found.')
     if not utils.is_checkpoint_finalized(directory):
       raise ValueError(f'Found incomplete checkpoint at {directory}.')
     logging.info('Restoring item from %s.', directory)
     ckpt_args = construct_checkpoint_args(self._handler, False, *args, **kwargs)
     restored = self._handler.restore(directory, args=ckpt_args)
     logging.info('Finished restoring checkpoint from %s.', directory)
+    utils.sync_global_processes('Checkpointer:restore', self._active_processes)
     return restored
 
   def metadata(self, directory: epath.PathLike) -> Optional[Any]:
     """See superclass documentation."""
     directory = epath.Path(directory)
     return self._handler.metadata(directory)
 
@@ -178,33 +181,14 @@
     """Closes the underlying CheckpointHandler."""
     self._handler.close()
 
   @property
   def handler(self) -> checkpoint_handler.CheckpointHandler:
     return self._handler
 
-
-@contextlib.contextmanager
-def checkpointer_context(*args, **kwargs):
-  """Context manager for Checkpointer.
-
-  Initializes Checkpointer and closes the object when the context is
-  exited.
-
-  Args:
-    *args: Arguments to initialize Checkpointer.
-    **kwargs: Keyword arguments to initialize Checkpointer.
-
-  Usage::
-
-    with checkpointer_context(PyTreeCheckpointHandler()) as ckptr:
-      ckptr.save(...)
-      ckptr.restore(...)
-
-  Yields:
-    Checkpointer
-  """
-  ckptr = Checkpointer(*args, **kwargs)
-  try:
-    yield ckptr
-  finally:
-    ckptr.close()
+  def __contextmanager__(
+      self,
+  ) -> Iterable[Self]:
+    try:
+      yield self
+    finally:
+      self.close()
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/composite_checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/composite_checkpoint_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 json_dict = restored.metadata
 ```
 """
 
 import asyncio
 from collections.abc import Collection, KeysView
 import concurrent.futures
-from typing import AbstractSet, Any, List, Mapping, Optional, Tuple
+import dataclasses
+from typing import AbstractSet, Any, List, Mapping, Optional, Tuple, Set
 import uuid
 
 from absl import logging
 from etils import epath
 import nest_asyncio
 from orbax.checkpoint import async_checkpoint_handler
 from orbax.checkpoint import checkpoint_args
@@ -173,14 +174,20 @@
 
 
 def _maybe_raise_reserved_item_error(item_name: str):
   if item_name in RESERVED_ITEM_NAMES:
     raise ValueError(f'Cannot specify reserved item name: "{item_name}".')
 
 
+@dataclasses.dataclass
+class CompositeOptions:
+  primary_host: Optional[int] = 0
+  active_processes: Optional[Set[int]] = None
+
+
 class CompositeCheckpointHandler(AsyncCheckpointHandler):
   """CheckpointHandler for saving multiple items.
 
   As with all `CheckpointHandler` implementations, use only in conjunction with
   an instance of `AbstractCheckpointer`.
 
   `CompositeCheckpointHandler` allows dealing with multiple items of different
@@ -255,26 +262,24 @@
   """
 
   _known_handlers: dict[str, Optional[CheckpointHandler]] = {}
 
   def __init__(
       self,
       *item_names: str,
-      primary_host: Optional[int] = 0,
+      composite_options: CompositeOptions = CompositeOptions(),
       **items_and_handlers: CheckpointHandler,
   ):
     """Constructor.
 
     All items must be provided up-front, at initialization.
 
     Args:
       *item_names: A list of string item names that this handler will manage.
-      enable_descriptor: Whether to enable descriptor for lineage logging.
-      primary_host: Host treated as primary. If None, all hosts are considered
-        to be primary.
+      composite_options: Options.
       **items_and_handlers: A mapping of item name to `CheckpointHandler`
         instance, which will be used as the handler for objects of the
         corresponding name.
     """
     self._known_handlers: dict[str, Optional[CheckpointHandler]] = (
         items_and_handlers
     )
@@ -285,15 +290,16 @@
       _maybe_raise_reserved_item_error(item_name)
       if handler and not checkpoint_args.has_registered_args(handler):
         logging.warning(
             'No registered CheckpointArgs found for handler type: %s',
             type(handler),
         )
         self._known_handlers[item_name] = get_legacy_handler_wrapper(handler)
-    self._primary_host = primary_host
+    self._primary_host = composite_options.primary_host
+    self._active_processes = composite_options.active_processes
 
   def _get_or_set_handler(
       self,
       item_name: str,
       args: Optional[CheckpointArgs],
   ) -> CheckpointHandler:
     if item_name not in self._known_handlers:
@@ -340,18 +346,19 @@
   ) -> Optional[List[Future]]:
     """Saves multiple items to individual subdirectories."""
     futures = []
     item_directories = [
         self._get_item_directory(directory, item_name)
         for item_name in args.keys()
     ]
-    if utils.is_primary_host(self._primary_host):
-      for path in item_directories:
-        path.mkdir(parents=False, exist_ok=False)
-    utils.sync_global_devices('CompositeCheckpointHandler:create_item_subdirs')
+    # NOTE: ocp.multihost.sync_global_processes may appear to work here, but
+    # it is not async-compatible.
+    # TODO(b/328525223) Replace with async-compatible barrier function.
+    for path in item_directories:
+      path.mkdir(parents=False, exist_ok=True)
 
     # Sort keys to maintain consistent ordering across processes, otherwise
     # we may hit timeouts if processes wait at different barriers in per-item
     # handlers.
     # TODO(b/295899152): Find a less brittle solution or support
     # async-compatible barrier function.
     for item_name in sorted(args.keys()):
@@ -375,15 +382,14 @@
       nest_asyncio.apply()
       commit_futures = await self.async_save(*args, **kwargs)
       if commit_futures:
         for f in commit_futures:
           f.result()
 
     asyncio.run(async_save())
-    utils.sync_global_devices('CompositeCheckpointHandler:save')
 
   def _items_exist(
       self, directory: epath.Path, item_names: List[str]
   ) -> Mapping[str, bool]:
     with concurrent.futures.ThreadPoolExecutor(
         max_workers=_CONCURRENT_WORKERS
     ) as executor:
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/composite_checkpoint_handler_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/composite_checkpoint_handler_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 StandardCheckpointHandler = (
     standard_checkpoint_handler.StandardCheckpointHandler
 )
 CompositeCheckpointHandler = (
     composite_checkpoint_handler.CompositeCheckpointHandler
 )
 ProtoCheckpointHandler = proto_checkpoint_handler.ProtoCheckpointHandler
+CompositeOptions = composite_checkpoint_handler.CompositeOptions
 
 
 class CompositeArgsTest(absltest.TestCase):
 
   def test_args(self):
     args = CompositeArgs(a=1, b=2, d=4)
     self.assertEqual(1, args.a)
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/conftest.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/experimental/__init__.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/experimental/emergency/__init__.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/emergency/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/future.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/json_checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/msgpack_utils.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/msgpack_utils_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax_checkpoint-0.5.8/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999907612712491%*

 * *Differences: {"'cells'": '{53: {\'source\': {insert: [(21, "    '*

 * *            'orbax.checkpoint.utils.sync_global_processes(\'ShardedFileCheckpointHandler:save\')\\n")], '*

 * *            'delete: [21]}}}'}*

```diff
@@ -826,15 +826,15 @@
                 "    async def async_save(*args, **kwargs):\n",
                 "      commit_futures = await self.async_save(*args, **kwargs)\n",
                 "      # Futures are already running, so sequential waiting is equivalent to\n",
                 "      # concurrent waiting.\n",
                 "      for future in commit_futures:\n",
                 "        future.result()  # Block on result.\n",
                 "    asyncio.run(async_save(directory, item, *args, **kwargs))\n",
-                "    orbax.checkpoint.utils.sync_global_devices('ShardedFileCheckpointHandler:save')\n",
+                "    orbax.checkpoint.utils.sync_global_processes('ShardedFileCheckpointHandler:save')\n",
                 "\n",
                 "  def restore(self,\n",
                 "              directory: epath.Path,\n",
                 "              item: Optional[bytes] = None) -> str:\n",
                 "    del item\n",
                 "    path = directory / str(jax.process_index())\n",
                 "    return path.read_text()\n",
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/path/__init__.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/path/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/path/step.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/path/step.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/path/step_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/path/step_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/proto/__init__.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/proto/testing/__init__.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/proto/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/proto_checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/proto_checkpoint_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,34 +22,36 @@
 import dataclasses
 import functools
 from typing import List, Optional, Type
 
 from etils import epath
 from google.protobuf import message
 from google.protobuf import text_format
-import jax
 from orbax.checkpoint import async_checkpoint_handler
 from orbax.checkpoint import checkpoint_args
 from orbax.checkpoint import future
+from orbax.checkpoint import utils
 
 
 CheckpointArgs = checkpoint_args.CheckpointArgs
 register_with_handler = checkpoint_args.register_with_handler
 
 
 class ProtoCheckpointHandler(async_checkpoint_handler.AsyncCheckpointHandler):
   """Serializes/deserializes protocol buffers."""
 
-  def __init__(self, filename: str):
+  def __init__(self, filename: str, primary_host: Optional[int] = 0):
     """Initializes ProtoCheckpointHandler.
 
     Args:
       filename: file name given to the written file.
+      primary_host: primary host to write on. If None, writes on all hosts.
     """
     self._filename = filename
+    self._primary_host = primary_host
     self._executor = futures.ThreadPoolExecutor(max_workers=1)
 
   async def async_save(
       self,
       directory: epath.Path,
       item: Optional[message.Message] = None,
       args: Optional["ProtoSaveArgs"] = None,
@@ -64,15 +66,15 @@
     Returns:
       A commit future.
     """
     if args is not None:
       item = args.item
 
     def _save_fn(x):
-      if jax.process_index() == 0:
+      if utils.is_primary_host(self._primary_host):
         path = directory / self._filename
         return path.write_text(text_format.MessageToString(x))
       return 0
 
     return [self._executor.submit(functools.partial(_save_fn, item))]
 
   def save(self, *args, **kwargs):
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -858,15 +858,15 @@
                 jax.tree_util.tree_map(
                     _create_param_save_dir,
                     param_infos,
                     save_args,
                 )
             )[0]
         )
-      utils.sync_global_devices(
+      utils.sync_global_processes(
           'PyTreeCheckpointHandler:create_param_save_dirs'
       )
 
     if all_params_aggregated:
       commit_futures = []
     else:
       serialize_ops = []
@@ -924,15 +924,14 @@
       # Futures are already running, so sequential waiting is equivalent to
       # concurrent waiting.
       if commit_futures:  # May be None.
         for f in commit_futures:
           f.result()  # Block on result.
 
     asyncio.run(async_save(directory, *args, **kwargs))
-    utils.sync_global_devices('PyTreeCheckpointHandler:save')
 
   async def _maybe_deserialize(
       self, structure: PyTree, param_infos: PyTree, restore_args: PyTree
   ) -> PyTree:
     """Deserializes values or gets them from the aggregate file."""
 
     # Handle parameters from aggregate file.
@@ -1136,15 +1135,14 @@
       restored_item = _transform_checkpoint(
           item,
           restored_item,
           restore_args,
           transforms,
           transforms_default_to_original,
       )
-    utils.sync_global_devices('PyTreeCheckpointHandler:restore')
 
     if logging.level_debug():
       logging.debug('param_infos: %s', param_infos)
       logging.debug('checkpoint_restore_args: %s', checkpoint_restore_args)
       logging.debug(
           'restored_item: %s', jax.tree_util.tree_structure(restored_item)
       )
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/pytree_checkpointer.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/pytree_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/random_key_checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/random_key_checkpoint_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from orbax.checkpoint import async_checkpoint_handler
 from orbax.checkpoint import checkpoint_args
 from orbax.checkpoint import composite_checkpoint_handler
 from orbax.checkpoint import future
 from orbax.checkpoint import json_checkpoint_handler
 from orbax.checkpoint import pytree_checkpoint_handler
 from orbax.checkpoint import type_handlers
-from orbax.checkpoint import utils
 
 NumpyRandomKeyType = Union[tuple, dict]
 
 ArrayRestoreArgs = array_checkpoint_handler.ArrayRestoreArgs
 ArraySaveArgs = array_checkpoint_handler.ArraySaveArgs
 CheckpointArgs = checkpoint_args.CheckpointArgs
 CompositeArgs = composite_checkpoint_handler.CompositeArgs
@@ -131,15 +130,14 @@
       commit_futures = await self.async_save(directory, *args, **kwargs)  # pytype: disable=bad-return-type
       # Futures are already running, so sequential waiting is equivalent to
       # concurrent waiting.
       for f in commit_futures:
         f.result()  # Block on result.
 
     asyncio.run(async_save())
-    utils.sync_global_devices('RandomKeyCheckpointHandler:save')
 
   def restore(
       self,
       directory: epath.Path,
       args: CheckpointArgs,
   ) -> Any:
     """Restores a random key.
@@ -156,19 +154,17 @@
         directory,
         args=CompositeArgs(**{
             self._key_name: item_arg,
             self._key_metadata: JsonRestoreArgs(),
         }),
     )
 
-    final_result = self.post_restore(
+    return self.post_restore(
         result[self._key_name], result[self._key_metadata]
     )
-    utils.sync_global_devices('RandomKeyCheckpointHandler:restore')
-    return final_result
 
   def finalize(self, directory: epath.Path):
     self._handler.finalize(directory)
 
   def close(self):
     self._handler.close()
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/random_key_checkpoint_handler_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/random_key_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/sharding_metadata.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/sharding_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 """ShardingMetadata representing Sharding property."""
 
 import abc
 import dataclasses
 import enum
 import json
-from typing import List, Tuple, Union
+import logging
+from typing import List, Optional, Tuple, Union
 import jax
 import numpy as np
 
 PartitionSpecElement = Union[None, str, Tuple[str, ...]]
 
 _PARTITION_SPEC = 'partition_spec'
 _SHARDING = '_sharding'
@@ -46,15 +47,15 @@
 
   converted_spec = []
   for element in jax_spec:
     if element is None:
       converted_element = None
     elif isinstance(element, str):
       converted_element = element
-    elif isinstance(element, tuple):
+    elif isinstance(element, (tuple, list)):
       converted_element = tuple(element)
     else:
       raise ValueError(f'Unsupported element type: {type(element)}')
     converted_spec.append(converted_element)
   return tuple(converted_spec)
 
 
@@ -154,15 +155,15 @@
     return (
         f'NamedShardingMetadata(shape={self.shape},'
         f' axis_names={self.axis_names}, partition_spec={self.partition_spec})'
     )
 
   def __eq__(self, other):
     return (
-        self.shape == other.shape
+        np.array_equal(self.shape, other.shape)
         and self.axis_names == other.axis_names
         and self.partition_spec == other.partition_spec
     )
 
 
 @dataclasses.dataclass
 class SingleDeviceShardingMetadata(ShardingMetadata):
@@ -218,23 +219,23 @@
 
 
 @dataclasses.dataclass
 class PositionalShardingMetadata(ShardingMetadata):
   pass
 
 
-def from_jax_sharding(jax_sharding) -> ShardingMetadata:
+def from_jax_sharding(jax_sharding) -> Optional[ShardingMetadata]:
   """Converts `jax.sharding.Sharding` to `ShardingMetadata`."""
   if isinstance(jax_sharding, jax.sharding.NamedSharding):
     return NamedShardingMetadata.from_jax_sharding(jax_sharding)
   elif isinstance(jax_sharding, jax.sharding.SingleDeviceSharding):
     return SingleDeviceShardingMetadata.from_jax_sharding(jax_sharding)
   else:
-    raise NotImplementedError(
-        f'Conversion for {type(jax_sharding)} has not been implemented.'
+    logging.warning(
+        'Conversion for %s has not been implemented.', type(jax_sharding)
     )
 
 
 def from_serialized_string(serialized_str) -> ShardingMetadata:
   """Converts `serialized_string` to `ShardingMetadata`."""
   deserialized_dict = json.loads(serialized_str)
   if deserialized_dict[_SHARDING_TYPE] == ShardingTypes.NAMED_SHARDING.value:
@@ -247,7 +248,14 @@
         deserialized_dict
     )
   else:
     raise NotImplementedError(
         f'Conversion for {deserialized_dict[_SHARDING_TYPE]} has not been'
         ' implemented.'
     )
+
+
+def get_sharding_or_none(serialized_string):
+  try:
+    return from_serialized_string(serialized_string.item()).to_jax_sharding()
+  except ValueError as e:
+    logging.error(e)
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/sharding_metadata_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/sharding_metadata_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from absl.testing import absltest
 import jax
 import numpy as np
 from orbax.checkpoint import sharding_metadata
-import pytest
 
 
 class TestShardingMetadata(absltest.TestCase):
 
   def test_convert_between_jax_named_sharding_and_sharding_metadata(self):
     # Convert from `jax.sharding.NamedSharding` to `NamedShardingMetadata`
     jax_sharding = jax.sharding.NamedSharding(
@@ -133,12 +132,18 @@
     self.assertEqual(
         converted_single_device_sharding_metadata,
         single_device_sharding_metadata,
     )
 
   def test_convert_to_jax_sharding_unsupported_types(self):
     jax_sharding = jax.sharding.PositionalSharding(jax.devices())
-    with pytest.raises(NotImplementedError):
+    warning_message = (
+        "Conversion for <class 'jax._src.sharding_impls.PositionalSharding'>"
+        " has not been implemented."
+    )
+    with self.assertLogs(level="WARNING") as log_output:
       sharding_metadata.from_jax_sharding(jax_sharding)
+      self.assertEqual(log_output[0][0].message, warning_message)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/single_host_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/single_host_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     pytree_checkpoint_handler.PyTreeCheckpointHandler
 ):
 
   def save(self, directory, *args, **kwargs):
     super().save(directory, *args, **kwargs)
     if jax.process_index() == 0:
       self.finalize(directory)
-    utils.sync_global_devices('PyTreeCheckpointHandler:finalize')
+    utils.sync_global_processes('PyTreeCheckpointHandler:finalize')
 
 
 class SingleHostTest(parameterized.TestCase):
 
   def setUp(self):
     super().setUp()
     self.ckpt_dir = epath.Path(self.create_tempdir('ckpt').full_path)
@@ -267,47 +267,54 @@
     # default is fine
     checkpoint_manager.CheckpointManager(
         options=options,
         directory=self.ckpt_dir,
     )
 
     with self.assertRaises(ValueError):
+      options.multiprocessing_options = (
+          checkpoint_manager.MultiprocessingOptions(primary_host=None)
+      )
       checkpoint_manager.CheckpointManager(
-          options=options, directory=self.ckpt_dir, primary_host=None
+          options=options, directory=self.ckpt_dir
       )
 
     # single handler with non-zero primary_host
     with self.assertRaises(ValueError):
+      options.multiprocessing_options = None
       checkpoint_manager.CheckpointManager(
           options=options,
           directory=self.ckpt_dir,
           item_handlers=pytree_checkpoint_handler.PyTreeCheckpointHandler(
               primary_host=None,
           ),
       )
 
     # multple handlers with non-zero primary_host
     with self.assertRaises(ValueError):
+      options.multiprocessing_options = None
       checkpoint_manager.CheckpointManager(
           options=options,
           directory=self.ckpt_dir,
           item_names={'x', 'y'},
           item_handlers={
               'x': pytree_checkpoint_handler.PyTreeCheckpointHandler(),
               'y': json_checkpoint_handler.JsonCheckpointHandler(
                   primary_host=None
               ),
           },
       )
 
     # manager is set to non-zero
     with self.assertRaises(ValueError):
+      options.multiprocessing_options = (
+          checkpoint_manager.MultiprocessingOptions(primary_host=None)
+      )
       checkpoint_manager.CheckpointManager(
           options=options,
           directory=self.ckpt_dir,
-          primary_host=None,
           item_handlers=pytree_checkpoint_handler.PyTreeCheckpointHandler(),
       )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/standard_checkpoint_handler.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/standard_checkpoint_handler_test_utils.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpoint_handler_test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,30 +26,30 @@
 import numpy as np
 import optax
 from orbax.checkpoint import standard_checkpoint_handler
 from orbax.checkpoint import test_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 
-
 PyTree = Any
 SaveArgs = type_handlers.SaveArgs
 StandardSaveArgs = standard_checkpoint_handler.StandardSaveArgs
 StandardRestoreArgs = standard_checkpoint_handler.StandardRestoreArgs
 
 
 class StandardCheckpointHandler(
     standard_checkpoint_handler.StandardCheckpointHandler
 ):
 
   def save(self, directory, *args, **kwargs):
     super().save(directory, *args, **kwargs)
+    utils.sync_global_processes('StandardCheckpointHandler:save')
     if jax.process_index() == 0:
       self.finalize(directory)
-    utils.sync_global_devices('StandardCheckpointHandler:finalize')
+    utils.sync_global_processes('StandardCheckpointHandler:finalize')
 
 
 # Not in common util because we need to eliminate OSS dependency on flax.
 def init_flax_model(model):
   params = model.init(jax.random.PRNGKey(0), jnp.ones([8, 8]))
   tx = optax.adamw(learning_rate=0.001)
   state = flax.training.train_state.TrainState.create(
@@ -88,18 +88,18 @@
       }
 
       self.directory = epath.Path(
           self.create_tempdir(name='checkpointing_test').full_path
       )
       test_utils.set_tensorstore_driver_for_test()
 
-      utils.sync_global_devices('StandardCheckpointHandler:setup_complete')
+      utils.sync_global_processes('StandardCheckpointHandler:setup_complete')
 
     def tearDown(self):
-      utils.sync_global_devices('StandardCheckpointHandler:tests_complete')
+      utils.sync_global_processes('StandardCheckpointHandler:tests_complete')
       self.handler.close()
       super().tearDown()
 
     @property
     def handler(self) -> StandardCheckpointHandler:
       return StandardCheckpointHandler()
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/standard_checkpointer.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/test_utils.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 """Utils for orbax tests."""
 
 from concurrent import futures
 import contextlib
 import functools
 import string
 import time
+import typing
 from typing import List, Optional, Tuple
 
 from absl import logging
 from etils import epath
 import jax
-from jax import sharding
 from jax.experimental import pjit
 from jax.experimental.array_serialization import serialization
 import jax.numpy as jnp
 import numpy as np
 from orbax.checkpoint import async_checkpoint_handler
 from orbax.checkpoint import checkpoint_args
 from orbax.checkpoint import pytree_checkpoint_handler
@@ -50,22 +50,22 @@
   step_tmp_dir = utils.create_tmp_directory(
       directory / (step_prefix + str(step))
   )
   item_tmp_dir = utils.create_tmp_directory(step_tmp_dir / item)
   if jax.process_index() == 0:
     for sub in subdirs:
       (item_tmp_dir / sub).mkdir(parents=True)
-  utils.sync_global_devices('save_fake_tmp_dir')
+  utils.sync_global_processes('save_fake_tmp_dir')
   return item_tmp_dir
 
 
 def replicate_sharded_array(arr: jax.Array):
   """Returns the input array, but replicated across all devices."""
   mesh = jax.sharding.Mesh(np.asarray(jax.devices()), ('x',))
-  replicated_sharding = sharding.NamedSharding(
+  replicated_sharding = jax.sharding.NamedSharding(
       mesh,
       jax.sharding.PartitionSpec(
           None,
       ),
   )
   return pjit.pjit(lambda x: x, out_shardings=replicated_sharding)(arr)
 
@@ -174,40 +174,69 @@
 
   pytree = jax.tree_util.tree_map(
       create_sharded_array, pytree, mesh_tree, axes_tree, is_leaf=is_leaf
   )
   return pytree, mesh_tree, axes_tree
 
 
-def setup_sharded_array_for_broadcasting(
-    array_size: int,
-    shape: Tuple[int, ...],
+def setup_replica_sharded_arrays(
+    arrays: List[jax.Array],
+    mesh_shape: Tuple[int, ...],
     is_replica_first: Optional[bool] = True,
 ):
   """Creates a tuple of sharded arrays for testing."""
-
-  array = (np.arange(array_size*8).reshape((8, array_size)) * 1,
-           np.arange(array_size*16).reshape((16, array_size)) * 2,
-           np.arange(array_size*8).reshape((8, array_size)) * 3,
-           np.arange(array_size*16).reshape((16, array_size)) * 4,)
   devices = jax.devices()
   devices = np.asarray(devices)
 
-  dim = len(shape)
+  dim = len(mesh_shape)
   axis_names = list(string.ascii_lowercase)
-  mesh = jax.sharding.Mesh(
-      devices.reshape(shape), axis_names[-dim:]
-  )
+  mesh = jax.sharding.Mesh(devices.reshape(mesh_shape), axis_names[-dim:])
   if is_replica_first:
     mesh_axes = jax.sharding.PartitionSpec(None, axis_names[-dim+1:])
   else:
     mesh_axes = jax.sharding.PartitionSpec(axis_names[-dim:-1], None)
 
-  sharded_arr = [create_sharded_array(arr, mesh, mesh_axes) for arr in array]
-  return sharded_arr, mesh, mesh_axes
+  sharded_arrs = [create_sharded_array(arr, mesh, mesh_axes) for arr in arrays]
+  return sharded_arrs, mesh, mesh_axes
+
+
+def select_single_replica(
+    arrays: List[jax.Array], global_mesh: jax.sharding.Mesh
+) -> List[jax.Array]:
+  """Returns arrays sharded over single slice."""
+  slice_devices = global_mesh.devices[0]
+  single_slice_mesh = jax.sharding.Mesh(
+      slice_devices, global_mesh.axis_names[1:]
+  )
+
+  def _get_single_slice_sharding(arr: jax.Array):
+    sharding = typing.cast(jax.sharding.NamedSharding, arr.sharding)
+    return jax.sharding.NamedSharding(
+        single_slice_mesh,
+        jax.sharding.PartitionSpec(*sharding.spec),  # exclude 'replica' axis
+    )
+
+  single_slice_shardings = jax.tree_util.tree_map(
+      _get_single_slice_sharding,
+      arrays,
+  )
+
+  def _make_single_slice_array(
+      arr: jax.Array, single_slice_sharding: jax.sharding.NamedSharding
+  ):
+    data = [
+        arr.addressable_data(idx) for idx in range(len(arr.addressable_shards))
+    ]
+    return jax.make_array_from_single_device_arrays(
+        arr.shape, single_slice_sharding, data
+    )
+
+  return jax.tree_util.tree_map(
+      _make_single_slice_array, arrays, single_slice_shardings
+  )
 
 
 def is_leaf(x):
   return (
       isinstance(x, np.ndarray)
       or isinstance(x, jax.sharding.Mesh)
       or isinstance(x, jax.sharding.PartitionSpec)
@@ -216,20 +245,23 @@
 
 
 def create_sharded_array(arr, mesh, mesh_axes):
   """Create sharded jax.Array."""
   if isinstance(arr, (int, float)):
     arr = np.asarray(arr)
   return jax.make_array_from_callback(
-      arr.shape, sharding.NamedSharding(mesh, mesh_axes), lambda idx: arr[idx]
+      arr.shape,
+      jax.sharding.NamedSharding(mesh, mesh_axes),
+      lambda idx: arr[idx],
   )
 
 
-def print_directory(directory: epath.Path, level: int = 0):
+def print_directory(directory: epath.PathLike, level: int = 0):
   """Prints a directory tree for debugging purposes."""
+  directory = epath.Path(directory)
   assert directory.is_dir()
   level_str = '..' * level
   if level == 0:
     logging.info('Printing directory tree: %s/', directory)
   else:
     logging.info('%s%s/', level_str, directory.name)
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/transform_utils.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/transform_utils_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/type_handlers.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/type_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 """Provides utils for PytreeCheckpointHandler."""
 
 import abc
 import asyncio
 import base64
 import dataclasses
-import enum
 import functools
 import json
 import os
 import re
 import time
 from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union, cast
 import warnings
@@ -30,155 +29,54 @@
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental.array_serialization import serialization
 import jax.numpy as jnp
 import numpy as np
 from orbax.checkpoint import future
+from orbax.checkpoint import sharding_metadata
 from orbax.checkpoint import utils
 from orbax.checkpoint import value_metadata
 import tensorstore as ts
 
 
 Scalar = Union[int, float, np.number]
 Metadata = value_metadata.Metadata
 NamedSharding = jax.sharding.NamedSharding
-SingleDeviceSharding = jax.sharding.SingleDeviceSharding
 ScalarMetadata = value_metadata.ScalarMetadata
 ArrayMetadata = value_metadata.ArrayMetadata
 StringMetadata = value_metadata.StringMetadata
-_MESH_AXES = 'axis_names'
-_MESH_SHAPE = 'shape'
-_NAMED_SHARDING = 'NamedSharding'
+ShardingMetadata = sharding_metadata.ShardingMetadata
 _OCDBT_MANIFEST_FILE = 'manifest.ocdbt'
 _COORDINATOR_SETUP_TIMEOUT_SECS = 300
 _OCDBT_TS_CONTEXT = None
 _OCDBT_COORDINATOR_SERVER = None
 _DEFAULT_OCDBT_TS_CONTEXT = ts.Context(
     {
         # Provide cache pool for B-tree nodes to avoid repeated reads.
         # 100MB limit.
         'cache_pool#ocdbt': {'total_bytes_limit': 100000000},
     },
     parent=serialization.TS_CONTEXT,
 )
 
-_PARTITION_SPEC = 'partition_spec'
-_SHARDING = '_sharding'
-_SHARDING_TYPE = 'sharding_type'
-_DEVICE_STR = 'device_str'
 
 RESTORE_TYPE_NONE = 'None'
 RESTORE_TYPE_DICT = 'Dict'
 RESTORE_TYPE_LIST = 'List'
 
 _DEFAULT_DRIVER = 'file'
 _PROCESS_SUBDIR_PREFIX = 'ocdbt.process_'
 _OCDBT_PROCESS_ID_RE = r'[A-Za-z0-9]+'
+_SHARDING = '_sharding'
 
 ZARR_VER2 = 'zarr'
 ZARR_VER3 = 'zarr3'
 
 
-class ShardingTypes(enum.Enum):
-  NAMED_SHARDING = 'NamedSharding'
-  SINGLE_DEVICE_SHARDING = 'SingleDeviceSharding'
-  POSITIONAL_SHARDING = 'PositionalSharding'
-  GSPMD_SHARDING = 'GSPMDSharding'
-
-
-def _serialize_sharding(sharding: jax.sharding.Sharding) -> str:
-  """Serializes `jax.sharding.Sharding` into a json string."""
-
-  sharding_data = {}
-  if isinstance(sharding, NamedSharding):
-    sharding_data[_SHARDING_TYPE] = ShardingTypes.NAMED_SHARDING.value
-    sharding_data[_MESH_SHAPE] = list(sharding.mesh.shape.values())
-    sharding_data[_MESH_AXES] = sharding.mesh.axis_names
-    sharding_data[_PARTITION_SPEC] = sharding.spec
-
-  elif isinstance(sharding, jax.sharding.SingleDeviceSharding):
-    sharding_data[_SHARDING_TYPE] = ShardingTypes.SINGLE_DEVICE_SHARDING.value
-    # There is no serialization method for Device.
-    # Get the Device object and then retreive the str representation
-    sharding_data[_DEVICE_STR] = str(next(iter(sharding.device_set)))
-
-  elif isinstance(sharding, jax.sharding.PositionalSharding):
-    warnings.warn(
-        'Serialization for `jax.sharding.PositionalSharding` has not been'
-        ' implemented.'
-    )
-
-  elif isinstance(sharding, jax.sharding.GSPMDSharding):
-    warnings.warn(
-        'Serialization for `jax.sharding.PositionalSharding` has not been'
-        ' implemented.'
-    )
-
-  else:
-    warnings.warn(f'Sharding type {type(sharding)} is not supported.')
-
-  if _SHARDING_TYPE in sharding_data:
-    serialized_string = json.dumps(sharding_data)
-    return serialized_string
-  else:
-    return ''
-
-
-def _deserialize_sharding_from_json_string(
-    sharding_string: str,
-) -> Optional[jax.sharding.Sharding]:
-  """Deserializes a json string to `jax.sharding.Sharding`."""
-
-  deserialized_dict = json.loads(sharding_string)
-
-  if deserialized_dict[_SHARDING_TYPE] == ShardingTypes.NAMED_SHARDING.value:
-    shape = deserialized_dict[_MESH_SHAPE]
-    axis_names = list(deserialized_dict[_MESH_AXES])
-    partition_spec = tuple(deserialized_dict[_PARTITION_SPEC])
-
-    if len(jax.devices()) != np.prod(shape):
-      return None
-    else:
-      return NamedSharding(
-          jax.sharding.Mesh(
-              np.array(jax.devices()).reshape(shape), axis_names=axis_names
-          ),
-          jax.sharding.PartitionSpec(*partition_spec),
-      )
-
-  elif (
-      deserialized_dict[_SHARDING_TYPE]
-      == ShardingTypes.SINGLE_DEVICE_SHARDING.value
-  ):
-    # Initialize a 'cached' Dict[str, Device] to help look up Devices by
-    # their str representation.
-    # Cache tip: See Function Attributes https://peps.python.org/pep-0232/.
-    if not hasattr(_deserialize_sharding_from_json_string, 'device_map'):
-      _deserialize_sharding_from_json_string.device_map = {
-          str(device): device for device in jax.local_devices()
-      }
-    device_str = deserialized_dict[_DEVICE_STR]
-    if device := _deserialize_sharding_from_json_string.device_map.get(
-        device_str, None
-    ):
-      return SingleDeviceSharding(device)
-
-    raise ValueError(
-        f'{ShardingTypes.SINGLE_DEVICE_SHARDING.value} with'
-        f' Device={device_str} was not found in jax.local_devices().'
-    )
-
-  else:
-    raise NotImplementedError(
-        'Sharding types other than `jax.sharding.NamedSharding` have not been '
-        'implemented.'
-    )
-
-
 def _get_coordinator_address_without_port(coordinator_address: str) -> str:
   """Returns JAX coordinator address stripped of port number."""
   return coordinator_address.split(':')[0]
 
 
 def create_coordinator_server_and_context() -> Tuple[None, None]:
   # TODO(b/293331479) remove this once OCDBT is enabled by default.
@@ -401,15 +299,20 @@
 
   def __post_init__(self):
     if self.aggregate:
       logging.log_every_n_seconds(
           logging.WARNING,
           'SaveArgs.aggregate is deprecated, please use custom TypeHandler'
           ' (https://orbax.readthedocs.io/en/latest/custom_handlers.html#typehandler)'
-          ' or contact Orbax team to migrate before May 1st, 2024.',
+          ' or contact Orbax team to migrate before May 1st, 2024. If your'
+          ' Pytree has empty ([], {}, None) values then use'
+          ' PyTreeCheckpointHandler(..., write_tree_metadata=True, ...) or use'
+          ' StandardCheckpointHandler to avoid TypeHandler Registry error.'
+          ' Please note that PyTreeCheckpointHandler.write_tree_metadata'
+          ' default value is already set to True.',
           n_seconds=12 * 60 * 60,  # once every 12 hours
       )
 
 
 @dataclasses.dataclass
 class RestoreArgs:
   """Extra arguments that can be provided for restoration.
@@ -955,15 +858,17 @@
       # Large value allows a single root node to support faster traversal.
       'max_decoded_node_bytes': 100000000,
   }
   return tspec
 
 
 def _array_metadata_from_tensorstore(
-    t: Any, info: ParamInfo, sharding: Optional[jax.sharding.Sharding] = None
+    t: Any,
+    info: ParamInfo,
+    sharding: Optional[sharding_metadata.ShardingMetadata] = None,
 ) -> ArrayMetadata:
   return ArrayMetadata(
       name=info.name,
       directory=info.parent_dir,
       shape=t.shape,
       dtype=jnp.dtype(t.dtype.name),
       sharding=sharding,
@@ -1226,30 +1131,32 @@
   """Arguments used when restoring with ArrayHandler.
 
   mesh:
     The device mesh that the array should be restored as. Cannot be None.
   mesh_axes:
     The mesh_axes that the array should be restored as. Cannot be None.
   sharding:
-    jax.sharding.Sharding object which takes precedence over mesh and
+   `jax.sharding.Sharding` object which takes precedence over mesh and
     mesh_axes if provided. Otherwise, mesh and mesh_axes will be used to
-    construct a NamedSharding object.
+    construct a NamedSharding object OR `ShardingMetadata` which is an orbax
+    representation of `jax.sharding.Sharding` that stores the same properties
+    but does not require accessing real devices.
   global_shape:
     The global shape that the array should be restored into. If not
     provided, the shape will be restored as written. Presently, arbitrary shape
     transformations are not supported (for example, reshaping to different
     dimensions). Padding and truncating are supported. When the global_shape is
     greater than that of the saved array, 0's will be appended. If the
     global_shape is shorter than that of the saved array, excess elements will
     be dropped from the end of the array.
   """
 
   mesh: Optional[jax.sharding.Mesh] = None
   mesh_axes: Optional[jax.sharding.PartitionSpec] = None
-  sharding: Optional[jax.sharding.Sharding] = None
+  sharding: Optional[Union[jax.sharding.Sharding, ShardingMetadata]] = None
   global_shape: Optional[Tuple[int, ...]] = None
 
 
 @dataclasses.dataclass
 class SingleReplicaArrayRestoreArgs(ArrayRestoreArgs):
   """Arguments used when restoring with SingleReplicaArrayHandler.
 
@@ -1262,18 +1169,22 @@
   single_replica_sharding:
     jax.sharding.NamedSharding object which describes the single replica
     sharding to which current host belongs to.
   replica_axis_index:
     The index of the axis dimension of the array, along which the replicas are
     defined. Currently works only when replica is taken along the first
     dimension, i.e. replica_axis_index is 0.
+  primary_replica_id:
+    The id of the replica hosts that is used to load and broadcast the
+    checkpoint.
   """
 
   single_replica_sharding: Optional[jax.sharding.NamedSharding] = None
   replica_axis_index: Optional[int] = 0
+  primary_replica_id: Optional[int] = 0
 
 
 class ArrayHandler(TypeHandler):
   """An implementation of TypeHandler for jax.Array."""
 
   def __init__(
       self,
@@ -1396,18 +1307,18 @@
       sharding_tensorstores = await asyncio.gather(*sharding_open_ops)
       for sharding_tensorstore in sharding_tensorstores:
         if sharding_tensorstore:
           sharding_string = await sharding_tensorstore.read()
           if not sharding_string.item():
             shardings.append(None)
             continue
-          deserialized = _deserialize_sharding_from_json_string(
+          deserialized = sharding_metadata.from_serialized_string(
               sharding_string.item()
           )
-          shardings.append(deserialized or None)
+          shardings.append(deserialized)
         else:
           shardings.append(None)
     else:
       shardings = [None] * len(tensorstores)
     return [
         _array_metadata_from_tensorstore(t, info, sharding)
         for (t, info, sharding) in zip(tensorstores, infos, shardings)
@@ -1497,15 +1408,20 @@
           # OCDBT is not used for sharding metadata.
           sharding_ts_context = get_ts_context(use_ocdbt=False)
           t = await ts.open(
               tspec_sharding,
               open=True,
               context=sharding_ts_context,
           )
-          serialized_sharding = _serialize_sharding(value.sharding)
+          serialized_sharding = None
+          sharding_metadata_value = sharding_metadata.from_jax_sharding(
+              value.sharding
+          )
+          if sharding_metadata_value is not None:
+            serialized_sharding = sharding_metadata_value.to_serialized_string()
           if serialized_sharding is not None:
             write_future = t.with_transaction(txn).write(serialized_sharding)
             synchronous_ops += [write_future.copy]
     await asyncio.gather(*synchronous_ops)
 
     if logging.level_debug():
       logging.debug(
@@ -1538,48 +1454,48 @@
     check_input_arguments(infos, args)
     deserialize_ops = []
     if infos[0].parent_dir is None:
       raise ValueError('parent_dir cannot be None')
     sharding_file_path = infos[0].parent_dir / _SHARDING
     sharding_file_exists = await utils.async_exists(sharding_file_path)
     for info, arg in zip(infos, args):
+      sharding = None
       arg = cast(ArrayRestoreArgs, arg)
       if (
           isinstance(arg, ArrayRestoreArgs)
           and arg.mesh is not None
           and arg.mesh_axes is not None
       ):
         sharding = NamedSharding(arg.mesh, arg.mesh_axes)
       elif isinstance(arg, ArrayRestoreArgs) and arg.sharding is not None:
-        sharding = arg.sharding
+        if isinstance(arg.sharding, ShardingMetadata):
+          sharding = arg.sharding.to_jax_sharding()
+        else:
+          sharding = arg.sharding
       elif sharding_file_exists:
         warnings.warn(
             "Couldn't find sharding info under RestoreArgs. Populating sharding"
             ' info from sharding file. Please note restoration time will be'
             ' slightly increased due to reading from file instead of directly'
             ' from RestoreArgs.'
         )
-        sharding = None
         if info.name:
           tspec_sharding = get_sharding_tensorstore_spec(
               os.fspath(info.parent_dir), info.name
           )
           t = await ts.open(
               tspec_sharding,
               # OCDBT is not used for sharding metadata.
               context=get_ts_context(use_ocdbt=False),
               open=True,
               read=True,
           )
           serialized_string = await t.read()
           if serialized_string:
-            sharding = (
-                _deserialize_sharding_from_json_string(serialized_string.item())
-                or None
-            )
+            sharding = sharding_metadata.get_sharding_or_none(serialized_string)
         else:
           raise ValueError('Unable to deserialize sharding.')
       else:
         raise ValueError(
             'Sharding of jax.Array cannot be None. Provide `mesh`'
             ' and `mesh_axes` OR `sharding`'
         )
@@ -1701,40 +1617,48 @@
     deserialize_ops = []
     shardings = []
     primary_replica_pids = set()
     single_replica_shardings = []
     replica_axis_index = None
     for info, arg in zip(infos, args):
       arg = cast(SingleReplicaArrayRestoreArgs, arg)
-      if isinstance(arg, SingleReplicaArrayRestoreArgs):
-        if arg.sharding is not None:
-          sharding = arg.sharding
-          shardings.append(sharding)
-          replica_axis_index = arg.replica_axis_index
-          primary_replica_ids, primary_replica_pids = (
-              utils.get_primary_replica_ids_and_pids(
-                  replica_axis_index, sharding.mesh  # pytype: disable=attribute-error
-              )
+
+      if not isinstance(arg, SingleReplicaArrayRestoreArgs):
+        raise ValueError(
+            'Must provide `SingleReplicaArrayRestoreArgs`, but got'
+            f' {type(arg)}.'
+        )
+
+      if arg.sharding is None:
+        raise ValueError('Must provide `sharding`.')
+
+      sharding = arg.sharding
+      shardings.append(sharding)
+      replica_axis_index = arg.replica_axis_index
+      primary_replica_ids, primary_replica_pids = (
+          utils.get_primary_replica_ids_and_pids(
+              replica_axis_idx=replica_axis_index,
+              mesh=sharding.mesh,  # pytype: disable=attribute-error
+              primary_replica_id=arg.primary_replica_id,
           )
-          if not _is_sharding_valid(primary_replica_ids, primary_replica_pids):
-            raise ValueError(
-                'The provided sharding configuration is invalid because it'
-                ' includes a host with devices assigned to the primary replica'
-                ' and devices outside of the primary replica.'
-            )
-        else:
-          raise ValueError('Must provide `sharding`.')
+      )
+      if not _is_sharding_valid(primary_replica_ids, primary_replica_pids):
+        raise ValueError(
+            'The provided sharding configuration is invalid because it'
+            ' includes a host with devices assigned to the primary replica and'
+            ' devices outside of the primary replica.'
+            f' primary_replica_ids={primary_replica_ids}'
+            f', primary_replica_pids={primary_replica_pids}'
+        )
+
+      if arg.single_replica_sharding is None:
+        raise ValueError('Must provide `single_replica_sharding`.')
+      single_replica_sharding = arg.single_replica_sharding
+      single_replica_shardings.append(single_replica_sharding)
 
-        if arg.single_replica_sharding is not None:
-          single_replica_sharding = arg.single_replica_sharding
-          single_replica_shardings.append(single_replica_sharding)
-        else:
-          raise ValueError('Must provide `sharding`.')
-      else:
-        raise ValueError('Must provide `SingleReplicaArrayRestoreArgs`.')
       if not info.is_ocdbt_checkpoint:
         await _assert_parameter_files_exist(  # pylint: disable=protected-access
             info.path, self._metadata_key
         )
 
       use_ocdbt = info.is_ocdbt_checkpoint
       tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
@@ -1758,15 +1682,26 @@
     )
     def create_zeros(shape_dtype_tup):
       return jax.tree_util.tree_map(
           lambda sd: jnp.zeros(sd.shape, dtype=sd.dtype), shape_dtype_tup
       )
 
     if _is_host_for_primary_replica(primary_replica_pids):
+      start_deserialization = time.time()
       deserialized = await asyncio.gather(*deserialize_ops)
+      deserialzation_elasped_s = time.time() - start_deserialization
+      jax.monitoring.record_event_duration_secs(
+          '/jax/checkpoint/read/primary_replica_deserialization_duration_secs',
+          deserialzation_elasped_s,
+      )
+      logging.info(
+          'Finished primary replica deserialization in %.2f',
+          deserialzation_elasped_s,
+      )
+
     else:
       single_replica_shardings = [arg.single_replica_sharding for arg in args]
       shape_dtype = [
           jax.ShapeDtypeStruct(arg.global_shape, arg.dtype) for arg in args
       ]
       deserialized = create_zeros(tuple(shape_dtype))
 
@@ -1780,18 +1715,19 @@
         global_mesh.mesh,
         single_replica_shardings,
         replica_axis_index,
         is_source=_is_host_for_primary_replica(primary_replica_pids),
     )
 
     jax.block_until_ready(shared_state)
-    end_broadcast = time.time()
-    logging.info(
-        'Finished broadcasting in %.2f', end_broadcast - start_broadcast
+    broadcast_elapsed_s = time.time() - start_broadcast
+    jax.monitoring.record_event_duration_secs(
+        '/jax/checkpoint/read/broadcast_duration_secs', broadcast_elapsed_s
     )
+    logging.info('Finished broadcasting in %.2f', broadcast_elapsed_s)
     return shared_state
 
 
 class StringHandler(TypeHandler):
   """TypeHandler for strings."""
 
   def __init__(
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/utils.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utility functions for Orbax.
 
 TODO(b/266449081) Increase unit test coverage.
-TODO(b/306715247) Move multihost_utils functions to new dedicated module.
+TODO(b/306715247) Move multihost functions to new dedicated module.
 """
 
 import asyncio
 import concurrent.futures
 import functools
 import os
 import re
 import time
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union, Set
 
 from absl import logging
 from etils import epath
 import jax
-from jax.experimental import multihost_utils
 import jax.numpy as jnp
 import numpy as np
+from orbax.checkpoint import multihost
+from orbax.checkpoint import sharding_metadata
 from orbax.checkpoint import value_metadata
 from orbax.checkpoint.path import step as step_lib
 
 # pylint: disable=g-bad-import-order
 # pylint: enable=g-bad-import-order
 
 TMP_DIR_SUFFIX = '.orbax-checkpoint-tmp-'
@@ -54,46 +55,18 @@
 _COMMIT_SUCCESS_FILE = 'commit_success.txt'
 _GCS_PATH_PREFIX = 'gs://'
 _LOCK_ITEM_NAME = 'LOCKED'
 _LAST_CHECKPOINT_WRITE_TIME = time.time()
 CheckpointDirs = Tuple[str, str]
 PyTree = Any
 
-
-
-
-def should_skip_device_sync() -> bool:
-  return False
-
-
-def sync_global_devices(name: str):
-  """Thin wrapper to provide additional features support."""
-  if should_skip_device_sync():
-    logging.info('Skipping global device sync, barrier name: %s', name)
-    return
-  logging.debug('sync_global_devices: %s', name)
-  sync_start_time = time.time()
-  multihost_utils.sync_global_devices(name)
-  # This may end up just being too noisy given how many barriers there are, but
-  # it does represent how long different processes waited around waiting for
-  # other processes to reach a barrier.
-  jax.monitoring.record_event_duration_secs(
-      '/jax/checkpoint/sync_global_devices_duration_sec',
-      time.time() - sync_start_time,
-  )
-
-
-def broadcast_one_to_all(pytree: PyTree) -> PyTree:
-  """Thin wrapper to provide additional features support."""
-  return multihost_utils.broadcast_one_to_all(pytree)
-
-
-def reached_preemption(step: int) -> bool:
-  """Returns True if a preemption sync point has been reached."""
-  return multihost_utils.reached_preemption_sync_point(step)
+sync_global_processes = multihost.sync_global_processes
+sync_global_devices = multihost.sync_global_processes
+broadcast_one_to_all = multihost.broadcast_one_to_all
+reached_preemption = multihost.reached_preemption
 
 
 def _wrap(func):
   """Wraps a function to make it async."""
 
   @functools.wraps(func)
   async def run(*args, loop=None, executor=None, **kwargs):
@@ -433,39 +406,56 @@
     if k.name == '_sharding':
       continue
     tree = add_nested_key(tree, k.name.split('.'), k.name)
   return tree
 
 
 def cleanup_tmp_directories(
-    directory: epath.PathLike, primary_host: Optional[int] = 0
+    directory: epath.PathLike,
+    primary_host: Optional[int] = 0,
+    active_processes: Optional[Set[int]] = None,
 ):
   """Cleanup steps in `directory` with tmp files, as these are not finalized."""
   directory = epath.Path(directory)
   if is_primary_host(primary_host):
     logging.info('Cleaning up existing temporary directories at %s.', directory)
     tmp_files = tmp_checkpoints(directory)
     for tmp_file in tmp_files:
       (directory / tmp_file).rmtree()
-
-  sync_global_devices('cleanup_tmp_dirs')
+  sync_global_processes('cleanup_tmp_dirs', processes=active_processes)
 
 
 def is_gcs_path(path: epath.Path):
   return os.fspath(path).startswith(_GCS_PATH_PREFIX)
 
 
-def get_tmp_directory(path: epath.Path) -> epath.Path:
+def get_tmp_directory(
+    path: epath.Path,
+    *,
+    primary_host: Optional[int] = 0,
+    active_processes: Optional[Set[int]] = None,
+) -> epath.Path:
   """Returns a tmp directory for the given path. Does not create it."""
   if is_gcs_path(path):
     return path
   now = time.time()
   sec = int(now)
   usec = int((now - sec) * 1000000)
-  timestamp = broadcast_one_to_all((np.int32(sec), np.int32(usec)))
+
+  # Impossible for all hosts to be the source if primary_host is None.
+  # Allow broadcast function to pick an arbitrary host to act as source if
+  # primary_host is None.
+  is_source = (
+      is_primary_host(primary_host) if primary_host is not None else None
+  )
+  timestamp = multihost.broadcast_one_to_some(
+      (np.int32(sec), np.int32(usec)),
+      is_source=is_source,
+      processes=active_processes,
+  )
   return epath.Path(path.parent) / (
       path.name + TMP_DIR_SUFFIX + f'{timestamp[0]}{timestamp[1]:06}'
   )
 
 
 def get_save_directory(
     step: int,
@@ -507,29 +497,34 @@
     result = step_lib.build_step_path(directory, step_name_format, step)
   if name is not None:
     result /= name
   return result
 
 
 def create_tmp_directory(
-    final_dir: epath.PathLike, primary_host: Optional[int] = 0
+    final_dir: epath.PathLike,
+    *,
+    primary_host: Optional[int] = 0,
+    active_processes: Optional[Set[int]] = None,
 ) -> epath.Path:
   """Creates a temporary directory for saving at the given path."""
   # Share a timestamp across devices.
   final_dir = epath.Path(final_dir)
   # Renames are not atomic in GCS. Save directly to final_dir and rely on commit
   # completion file to indicate success.
   if is_gcs_path(final_dir):
     tmp_dir = final_dir
   else:
-    tmp_dir = get_tmp_directory(final_dir)
+    tmp_dir = get_tmp_directory(
+        final_dir, primary_host=primary_host, active_processes=active_processes
+    )
 
   # Sync before existence is checked and directory is created because there are
   # additional existence checks happening in the callers of this function.
-  sync_global_devices('create_tmp_directory:pre')
+  sync_global_processes('create_tmp_directory:pre', processes=active_processes)
 
   if is_primary_host(primary_host):
     if tmp_dir.exists():
       if is_gcs_path(tmp_dir):
         if is_tmp_checkpoint(tmp_dir):
           logging.warning(
               'Attempted to create temporary directory %s which already exists.'
@@ -546,15 +541,15 @@
         raise AssertionError(
             f'Attempted to create temporary directory {tmp_dir} which already'
             ' exists. This condition should never arise on non-GCS'
             ' filesystems.'
         )
     tmp_dir.mkdir(parents=True)
 
-  sync_global_devices('create_tmp_directory:post')
+  sync_global_processes('create_tmp_directory:post', processes=active_processes)
   return tmp_dir
 
 
 def ensure_atomic_save(temp_ckpt_dir: epath.Path, final_ckpt_dir: epath.Path):
   """Finalizes atomic save by renaming tmp_dir or writing a success file."""
   if temp_ckpt_dir == final_ckpt_dir:
     (final_ckpt_dir / _COMMIT_SUCCESS_FILE).write_text(
@@ -695,15 +690,15 @@
     # Read the step list only from host 0, and then broadcast the list.
     # This minimizes queries on non-leader processes.
     padded_step_list = np.array([-1] * max_steps)
     if jax.process_index() == 0:
       steps = np.array(_checkpoint_steps(checkpoint_dir))
       assert len(steps) <= max_steps
       padded_step_list[0 : len(steps)] = steps
-    padded_step_list = multihost_utils.broadcast_one_to_all(padded_step_list)
+    padded_step_list = multihost.broadcast_one_to_all(padded_step_list)
     return [step for step in padded_step_list if step >= 0]
   return _checkpoint_steps(checkpoint_dir)
 
 
 def any_checkpoint_step(checkpoint_dir: epath.PathLike) -> Optional[int]:
   """Returns any finalized checkpoint step in the directory or None.
 
@@ -855,15 +850,17 @@
 
 def to_shape_dtype_struct(x, dtype=None, scalar_dtype=None):
   """Get ShapeDtypeStruct from array."""
   if isinstance(x, jax.ShapeDtypeStruct):
     return jax.ShapeDtypeStruct(
         shape=x.shape,
         dtype=dtype if dtype is not None else x.dtype,
-        sharding=x.sharding,
+        sharding=x.sharding
+        if isinstance(x.sharding, jax.sharding.Sharding)
+        else x.sharding.to_jax_sharding(),
     )
   elif isinstance(x, jax.Array):
     dtype = dtype or x.dtype
     return jax.ShapeDtypeStruct(x.shape, dtype, sharding=x.sharding)
   elif isinstance(x, np.ndarray):
     dtype = dtype or x.dtype
     return jax.ShapeDtypeStruct(x.shape, dtype)
@@ -874,15 +871,17 @@
   elif isinstance(x, value_metadata.Metadata):
     if not isinstance(x, value_metadata.ArrayMetadata):
       raise ValueError(f'Unexpected Metadata type: {type(x)}.')
     dtype = dtype or x.dtype
     return jax.ShapeDtypeStruct(
         shape=x.shape,
         dtype=dtype,
-        sharding=x.sharding,
+        sharding=x.sharding.to_jax_sharding()
+        if isinstance(x.sharding, sharding_metadata.ShardingMetadata)
+        else x.sharding,
     )
   else:
     raise ValueError(f'Unexpected type: {type(x)}.')
 
 
 def _sum(x, replica_axis_index):
   return jax.tree_map(functools.partial(jnp.sum, axis=replica_axis_index), x)
@@ -942,20 +941,20 @@
 
   return out_tree
 
 
 def get_primary_replica_ids_and_pids(
     replica_axis_idx: int,
     mesh: jax.sharding.Mesh,
-    primary_replica_idx: int = 0,
+    primary_replica_id: int,
 ):
   """Returns the primary replica ids and process ids."""
   replica_devices = np.take(
       mesh.devices,
-      primary_replica_idx,
+      primary_replica_id,
       axis=replica_axis_idx,
   ).flatten()
   pids = set([d.process_index for d in replica_devices])
   ids = set([d.id for d in replica_devices])
   return ids, pids
```

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/utils_test.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/orbax/checkpoint/value_metadata.py` & `orbax_checkpoint-0.5.8/orbax/checkpoint/value_metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import dataclasses
 from typing import Optional
 
 from etils import epath
 import jax
 from jax import numpy as jnp
+from orbax.checkpoint import sharding_metadata
 
 
 @dataclasses.dataclass
 class Metadata:
   """Metadata describing PyTree values.
 
   name:
@@ -43,23 +44,23 @@
 @dataclasses.dataclass
 class ArrayMetadata(Metadata):
   """Metadata describing an array.
 
   shape:
     Tuple of integers describing the array shape.
   sharding:
-    jax.sharding.Sharding to indicate how the array is sharded. In most of the
-    cases, it's NamedSharding.
-    May be None if the array is not sharded.
+    ShardingMetadata to indicate how the array is sharded. ShardingMetadata is
+    an orbax representation of `jax.sharding.Sharding` which stores the same
+    properties but not require accessing real devices.
   dtype:
     Dtype of array elements.
   """
 
   shape: tuple[int, ...]
-  sharding: Optional[jax.sharding.Sharding]
+  sharding: Optional[sharding_metadata.ShardingMetadata]
   dtype: Optional[jnp.dtype]
 
   def __eq__(self, other: 'Metadata') -> bool:
     return (
         isinstance(other, ArrayMetadata)
         and self.shape == other.shape
         and self.sharding == other.sharding
@@ -87,15 +88,15 @@
   """Metadata describing a scalar value.
 
   dtype:
     Scalar dtype.
   """
 
   shape: tuple[int, ...] = tuple([])
-  sharding: Optional[jax.sharding.Sharding] = None
+  sharding: Optional[sharding_metadata.ShardingMetadata] = None
   dtype: Optional[jnp.dtype] = None
 
   def __eq__(self, other: 'Metadata') -> bool:
     return isinstance(other, ScalarMetadata) and self.dtype == other.dtype
 
 
 @dataclasses.dataclass
```

### Comparing `orbax_checkpoint-0.5.7/pyproject.toml` & `orbax_checkpoint-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.7/PKG-INFO` & `orbax_checkpoint-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.5.7
+Version: 0.5.8
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

