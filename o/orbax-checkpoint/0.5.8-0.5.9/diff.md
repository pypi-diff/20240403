# Comparing `tmp/orbax_checkpoint-0.5.8.tar.gz` & `tmp/orbax_checkpoint-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax_checkpoint-0.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orbax_checkpoint-0.5.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax_checkpoint-0.5.8.tar` & `orbax_checkpoint-0.5.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11357 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/LICENSE
--rw-r--r--   0        0        0      556 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/README.md
--rw-r--r--   0        0        0     3433 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0    11844 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/abstract_checkpoint_manager.py
--rw-r--r--   0        0        0     2824 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2919 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     2589 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/args.py
--rw-r--r--   0        0        0     6886 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1377 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0    12580 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     5055 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_args.py
--rw-r--r--   0        0        0     5447 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_args_test.py
--rw-r--r--   0        0        0     2324 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    54299 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0    16384 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0    12282 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     7098 2024-04-03 19:16:55.431774 orbax_checkpoint-0.5.8/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0    21616 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/composite_checkpoint_handler.py
--rw-r--r--   0        0        0    13128 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/composite_checkpoint_handler_test.py
--rw-r--r--   0        0        0      740 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0      583 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/__init__.py
--rw-r--r--   0        0        0      583 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/emergency/__init__.py
--rw-r--r--   0        0        0    13071 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/emergency/checkpoint_manager.py
--rw-r--r--   0        0        0     1576 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     3196 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     2018 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     7672 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0      977 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/multihost/__init__.py
--rw-r--r--   0        0        0     5022 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/multihost/utils.py
--rw-r--r--   0        0        0    45658 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0      583 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/__init__.py
--rw-r--r--   0        0        0     5194 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/deleter.py
--rw-r--r--   0        0        0     2131 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/deleter_test.py
--rw-r--r--   0        0        0     6257 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/step.py
--rw-r--r--   0        0        0     6781 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/path/step_test.py
--rw-r--r--   0        0        0      757 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/proto/__init__.py
--rw-r--r--   0        0        0      757 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/proto/testing/__init__.py
--rw-r--r--   0        0        0      136 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/proto/testing/foo.proto
--rw-r--r--   0        0        0     3946 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/proto_checkpoint_handler.py
--rw-r--r--   0        0        0    56506 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     1284 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/pytree_checkpointer.py
--rw-r--r--   0        0        0     8907 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/random_key_checkpoint_handler.py
--rw-r--r--   0        0        0     6883 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/random_key_checkpoint_handler_test.py
--rw-r--r--   0        0        0     8385 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/sharding_metadata.py
--rw-r--r--   0        0        0     5542 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/sharding_metadata_test.py
--rw-r--r--   0        0        0    10702 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/single_host_test.py
--rw-r--r--   0        0        0     7098 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpoint_handler.py
--rw-r--r--   0        0        0     9916 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpoint_handler_test_utils.py
--rw-r--r--   0        0        0     1213 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpointer.py
--rw-r--r--   0        0        0    10827 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0    12624 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    15251 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    65030 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    31488 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0    10277 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     2870 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/orbax/checkpoint/value_metadata.py
--rw-r--r--   0        0        0     1153 2024-04-03 19:16:55.435774 orbax_checkpoint-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 orbax_checkpoint-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/LICENSE
+-rw-r--r--   0        0        0      556 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/README.md
+-rw-r--r--   0        0        0     3433 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0    11844 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/abstract_checkpoint_manager.py
+-rw-r--r--   0        0        0     2824 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2919 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     2589 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/args.py
+-rw-r--r--   0        0        0     6886 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1377 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0    12580 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     5055 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_args.py
+-rw-r--r--   0        0        0     5447 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_args_test.py
+-rw-r--r--   0        0        0     2324 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    54299 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0    16384 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0    12282 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     7098 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0    21616 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/composite_checkpoint_handler.py
+-rw-r--r--   0        0        0    13128 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/composite_checkpoint_handler_test.py
+-rw-r--r--   0        0        0      740 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0      583 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/experimental/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/experimental/emergency/__init__.py
+-rw-r--r--   0        0        0    13071 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/experimental/emergency/checkpoint_manager.py
+-rw-r--r--   0        0        0     1576 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     3196 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     2018 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     7672 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2024-04-03 20:37:35.368452 orbax_checkpoint-0.5.9/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0      977 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/multihost/__init__.py
+-rw-r--r--   0        0        0     5025 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/multihost/utils.py
+-rw-r--r--   0        0        0    45658 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0      583 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/path/__init__.py
+-rw-r--r--   0        0        0     5194 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/path/deleter.py
+-rw-r--r--   0        0        0     2131 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/path/deleter_test.py
+-rw-r--r--   0        0        0     6257 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/path/step.py
+-rw-r--r--   0        0        0     6781 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/path/step_test.py
+-rw-r--r--   0        0        0      757 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/proto/__init__.py
+-rw-r--r--   0        0        0      757 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/proto/testing/__init__.py
+-rw-r--r--   0        0        0      136 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/proto/testing/foo.proto
+-rw-r--r--   0        0        0     3946 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/proto_checkpoint_handler.py
+-rw-r--r--   0        0        0    56506 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     1284 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/pytree_checkpointer.py
+-rw-r--r--   0        0        0     8907 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/random_key_checkpoint_handler.py
+-rw-r--r--   0        0        0     6883 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/random_key_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     8385 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/sharding_metadata.py
+-rw-r--r--   0        0        0     5542 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/sharding_metadata_test.py
+-rw-r--r--   0        0        0    10702 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/single_host_test.py
+-rw-r--r--   0        0        0     7098 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/standard_checkpoint_handler.py
+-rw-r--r--   0        0        0     9916 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/standard_checkpoint_handler_test_utils.py
+-rw-r--r--   0        0        0     1213 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/standard_checkpointer.py
+-rw-r--r--   0        0        0    10827 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0    12624 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    15251 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    65030 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    31488 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0    10277 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     2870 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/orbax/checkpoint/value_metadata.py
+-rw-r--r--   0        0        0     1153 2024-04-03 20:37:35.372452 orbax_checkpoint-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 orbax_checkpoint-0.5.9/PKG-INFO
```

### Comparing `orbax_checkpoint-0.5.8/LICENSE` & `orbax_checkpoint-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/README.md` & `orbax_checkpoint-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/__init__.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
   nest_asyncio.apply()
 except RuntimeError:
   pass
 
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
 # Also modify version and date in CHANGELOG.
-__version__ = '0.5.8'
+__version__ = '0.5.9'
```

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/abstract_checkpoint_manager.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/abstract_checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/abstract_checkpointer.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/aggregate_handlers.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/args.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/args.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/array_checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/async_checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/async_checkpointer.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_args.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_args.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_args_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_args_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_manager.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_utils.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpoint_utils_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/checkpointer.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/composite_checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/composite_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/composite_checkpoint_handler_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/composite_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/conftest.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/__init__.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/emergency/__init__.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/experimental/emergency/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/experimental/emergency/checkpoint_manager.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/experimental/emergency/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/future.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/json_checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/msgpack_utils.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/msgpack_utils_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/multihost/__init__.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/multihost/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/multihost/utils.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/multihost/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
       out_shardings=jax.sharding.NamedSharding(
           global_mesh, jax.sharding.PartitionSpec()
       ),
   )(in_tree)
   return jax.tree.map(post_jit, out_tree)
 
 
-def broadcast_one_to_all(in_tree, is_source: bool | None = None):
+def broadcast_one_to_all(in_tree, is_source: Optional[bool] = None):
   """Broadcast data from a source host to all other hosts."""
   return broadcast_one_to_some(in_tree, is_source=is_source)
 
 
 def should_skip_process_sync() -> bool:
   return False
```

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax_checkpoint-0.5.9/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/path/__init__.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/path/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/path/deleter.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/path/deleter.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/path/deleter_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/path/deleter_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/path/step.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/path/step.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/path/step_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/path/step_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/proto/__init__.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/proto/testing/__init__.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/proto/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/proto_checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/proto_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/pytree_checkpointer.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/pytree_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/random_key_checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/random_key_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/random_key_checkpoint_handler_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/random_key_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/sharding_metadata.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/sharding_metadata.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/sharding_metadata_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/sharding_metadata_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/single_host_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/single_host_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpoint_handler.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/standard_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpoint_handler_test_utils.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/standard_checkpoint_handler_test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/standard_checkpointer.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/standard_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/test_utils.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/transform_utils.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/transform_utils_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/type_handlers.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/type_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/utils.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/utils_test.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/orbax/checkpoint/value_metadata.py` & `orbax_checkpoint-0.5.9/orbax/checkpoint/value_metadata.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/pyproject.toml` & `orbax_checkpoint-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.5.8/PKG-INFO` & `orbax_checkpoint-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.5.8
+Version: 0.5.9
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

