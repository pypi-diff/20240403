# Comparing `tmp/gink-0.20240401.1711930006.tar.gz` & `tmp/gink-0.20240403.1712115567.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240401.1711930006.tar", last modified: Mon Apr  1 00:06:50 2024, max compression
+gzip compressed data, was "gink-0.20240403.1712115567.tar", last modified: Wed Apr  3 03:39:30 2024, max compression
```

## Comparing `gink-0.20240401.1711930006.tar` & `gink-0.20240403.1712115567.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:50.536136 gink-0.20240401.1711930006/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-01 00:06:50.536136 gink-0.20240401.1711930006/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:50.520135 gink-0.20240401.1711930006/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:50.524136 gink-0.20240401.1711930006/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-04-01 00:06:47.000000 gink-0.20240401.1711930006/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:50.532136 gink-0.20240401.1711930006/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17862 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    53266 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/impl/websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:50.536136 gink-0.20240401.1711930006/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10202 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-01 00:06:44.000000 gink-0.20240401.1711930006/gink/tests/test_websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:06:50.536136 gink-0.20240401.1711930006/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-01 00:06:50.000000 gink-0.20240401.1711930006/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-01 00:06:50.000000 gink-0.20240401.1711930006/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:06:50.000000 gink-0.20240401.1711930006/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-01 00:06:50.000000 gink-0.20240401.1711930006/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 00:06:50.000000 gink-0.20240401.1711930006/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 00:06:50.536136 gink-0.20240401.1711930006/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-01 00:06:46.000000 gink-0.20240401.1711930006/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:30.500241 gink-0.20240403.1712115567/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-03 03:39:30.500241 gink-0.20240403.1712115567/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:30.488241 gink-0.20240403.1712115567/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:30.492241 gink-0.20240403.1712115567/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:30.496241 gink-0.20240403.1712115567/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17862 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53266 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/impl/websocket_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:30.500241 gink-0.20240403.1712115567/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10202 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-03 03:39:25.000000 gink-0.20240403.1712115567/gink/tests/test_websocket_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:39:30.500241 gink-0.20240403.1712115567/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-03 03:39:30.000000 gink-0.20240403.1712115567/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-03 03:39:30.000000 gink-0.20240403.1712115567/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:39:30.000000 gink-0.20240403.1712115567/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 03:39:30.000000 gink-0.20240403.1712115567/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 03:39:30.000000 gink-0.20240403.1712115567/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:39:30.500241 gink-0.20240403.1712115567/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-03 03:39:27.000000 gink-0.20240403.1712115567/setup.py
```

### Comparing `gink-0.20240401.1711930006/LICENSE` & `gink-0.20240403.1712115567/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/PKG-INFO` & `gink-0.20240403.1712115567/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240401.1711930006
+Version: 0.20240403.1712115567
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240401.1711930006/README.md` & `gink-0.20240403.1712115567/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/__init__.py` & `gink-0.20240403.1712115567/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/__main__.py` & `gink-0.20240403.1712115567/gink/__main__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/behavior_pb2.py` & `gink-0.20240403.1712115567/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/bundle_pb2.py` & `gink-0.20240403.1712115567/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/change_pb2.py` & `gink-0.20240403.1712115567/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/claim_pb2.py` & `gink-0.20240403.1712115567/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/clearance_pb2.py` & `gink-0.20240403.1712115567/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/container_pb2.py` & `gink-0.20240403.1712115567/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/entry_pb2.py` & `gink-0.20240403.1712115567/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/key_pb2.py` & `gink-0.20240403.1712115567/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/log_file_pb2.py` & `gink-0.20240403.1712115567/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/movement_pb2.py` & `gink-0.20240403.1712115567/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/muid_pb2.py` & `gink-0.20240403.1712115567/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/pair_pb2.py` & `gink-0.20240403.1712115567/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/sync_message_pb2.py` & `gink-0.20240403.1712115567/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/builders/value_pb2.py` & `gink-0.20240403.1712115567/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/abstract_store.py` & `gink-0.20240403.1712115567/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/addressable.py` & `gink-0.20240403.1712115567/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/attribution.py` & `gink-0.20240403.1712115567/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/box.py` & `gink-0.20240403.1712115567/gink/impl/box.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 class Box(Container):
     BEHAVIOR = BOX
 
     def __init__(self,
                  muid: Optional[Muid] = None,
                  database: Optional[Database] = None,
-                 root: bool = False,
+                 arche: bool = False,
                  bundler: Optional[Bundler] = None,
                  contents = None,
                  comment: Optional[str] = None,
                  ):
         """
         muid: the global id of this sequence, created on the fly if None
         database: where to send commits through, or last db instance created if None
         """
-        if root:
+        if arche:
             muid = Muid(-1, -1, BOX)
         database = database or Database.get_last()
         immediate = False
         if bundler is None:
             immediate = True
             bundler = Bundler(comment)
         if muid is None:
@@ -63,15 +63,15 @@
         contents = self._get_occupant(found.builder, found.address)
 
         return contents
 
     def dumps(self, as_of: GenericTimestamp = None) -> str:
         """ Dumps the contents of this box to a string. """
         if self._muid.medallion == -1 and self._muid.timestamp == -1:
-            identifier = "root=True"
+            identifier = "arche=True"
         else:
             identifier = repr(str(self._muid))
 
         as_of = self._database.resolve_timestamp(as_of)
         found = self._database.get_store().get_entry_by_key(container=self._muid, key=None, as_of=as_of)
 
         if found is None or found.builder.deletion: #type: ignore
```

### Comparing `gink-0.20240401.1711930006/gink/impl/builders.py` & `gink-0.20240403.1712115567/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/bundle_info.py` & `gink-0.20240403.1712115567/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/bundle_wrapper.py` & `gink-0.20240403.1712115567/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/bundler.py` & `gink-0.20240403.1712115567/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/chain_tracker.py` & `gink-0.20240403.1712115567/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/coding.py` & `gink-0.20240403.1712115567/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/connection.py` & `gink-0.20240403.1712115567/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/container.py` & `gink-0.20240403.1712115567/gink/impl/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .addressable import Addressable
 
 class Container(Addressable, ABC):
     """ Abstract base class for mutable data types (directories, sequences, etc). """
 
     def __repr__(self):
         if self._muid.timestamp == -1 and self._muid.medallion == -1:
-            return f"{self.__class__.__name__}(root=True)"
+            return f"{self.__class__.__name__}(arche=True)"
         return f"{self.__class__.__name__}('{self._muid}')"
 
     def _get_container(self) -> Muid:
         return self._muid
 
     @abstractmethod
     def dumps(self, as_of: GenericTimestamp = None) -> str:
```

### Comparing `gink-0.20240401.1711930006/gink/impl/database.py` & `gink-0.20240403.1712115567/gink/impl/database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/deferred.py` & `gink-0.20240403.1712115567/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/directory.py` & `gink-0.20240403.1712115567/gink/impl/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 
 
 class Directory(Container):
     """ the Gink mutable mapping object """
     _missing = object()
     BEHAVIOR = DIRECTORY
 
-    def __init__(self, *ordered, root: Optional[bool] = None, bundler: Optional[Bundler] = None,
+    def __init__(self, *ordered, arche: Optional[bool] = None, bundler: Optional[Bundler] = None,
                  contents=None, muid: Optional[Muid] = None, database=None, comment: Optional[str] = None):
         """
         Constructor for a directory proxy.
 
         muid: the global id of this directory, created on the fly if None
         db: database send commits through, or last db instance created if None
         """
         self._logger = getLogger(self.__class__.__name__)
 
         if ordered:
             if isinstance(ordered[0], str):
                 muid = Muid.from_str(ordered[0])
-        if root:
+        if arche:
             muid = Muid(-1, -1, DIRECTORY)
         database = database or Database.get_last()
         immediate = False
         if bundler is None:
             immediate = True
             bundler = Bundler(comment)
         if muid is None:
@@ -51,15 +51,15 @@
         if immediate and len(bundler):
             self._database.commit(bundler)
 
     def dumps(self, as_of: GenericTimestamp = None) -> str:
         """ Dumps the contents of this directory to a string.
         """
         if self._muid.medallion == -1 and self._muid.timestamp == -1:
-            identifier = "root=True"
+            identifier = "arche=True"
         else:
             identifier = repr(str(self._muid))
         result = f"""{self.__class__.__name__}({identifier}, contents="""
         result += "{"
         stuffing = [f"{key!r}: {val!r}" for key, val in self.items(as_of=as_of)]
         as_one_line = result + ", ".join(stuffing) + "})"
         if len(as_one_line) < 80:
```

### Comparing `gink-0.20240401.1711930006/gink/impl/graph.py` & `gink-0.20240403.1712115567/gink/impl/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
 
 @experimental
 class Vertex(Container):
     BEHAVIOR = VERTEX
 
     def __init__(self, *,
-                 root: bool = False,
+                 arche: bool = False,
                  muid: Optional[Muid] = None,
                  bundler: Optional[Bundler] = None,
                  database: Optional[Database] = None):
         """
         Creates a placeholder node to contain the idea of something.
 
         muid: the global id of this vertex, created on the fly if None
         db: database send commits through, or last db instance created if None
         """
         database = database or Database.get_last()
         immediate = False
         if not isinstance(bundler, Bundler):
             immediate = True
             bundler = Bundler()
-        if root:
+        if arche:
             muid = Muid(-1, -1, VERTEX)
         if muid is None:
             muid = Container._create(VERTEX, database=database, bundler=bundler)
         Container.__init__(self, muid=muid, database=database)
         if len(bundler) and immediate:
             self._database.commit(bundler)
 
@@ -94,21 +94,21 @@
 
 
 @experimental
 class Verb(Container):
     BEHAVIOR = VERB
 
     def __init__(self, *,
-                 root=False,
+                 arche=False,
                  muid: Optional[Muid] = None,
                  database: Optional[Database] = None,
                  contents: Optional[Iterable[Edge]] = None):
         database = database or Database.get_last()
         bundler = Bundler()
-        if root:
+        if arche:
             muid = Muid(-1, -1, VERB)
         if muid is None:
             muid = Container._create(VERB, database=database, bundler=bundler)
         Container.__init__(self, muid=muid, database=database)
         if contents:
             pass  # This is intentional! The edge constructors will restore them!
         if len(bundler):
@@ -154,15 +154,15 @@
             count += 1
         return count
 
     def dumps(self, as_of: GenericTimestamp = None) -> str:
         """ Dump all the edges for this verb.
         """
         if self._muid.medallion == -1 and self._muid.timestamp == -1:
-            identifier = "root=True"
+            identifier = "arche=True"
         else:
             identifier = repr(str(self._muid))
         result = f"""{self.__class__.__name__}({identifier}, contents=["""
         if self.size() == 0:
             return result + "])"
         stuffing = [edge.dumps(2) for edge in self.get_edges(as_of=as_of)]
         result += "\n\n"
```

### Comparing `gink-0.20240401.1711930006/gink/impl/key_set.py` & `gink-0.20240403.1712115567/gink/impl/key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 from .typedefs import UserKey, GenericTimestamp
 from .builders import Behavior
 
 class KeySet(Container):
     _missing = object()
     BEHAVIOR = KEY_SET
 
-    def __init__(self, root: Optional[bool] = None, bundler: Optional[Bundler] = None, contents = None,
+    def __init__(self, arche: Optional[bool] = None, bundler: Optional[Bundler] = None, contents = None,
                  muid: Optional[Muid] = None, database = None, comment: Optional[str] = None):
         """
         Constructor for a set proxy.
 
         muid: the global id of this set, created on the fly if None
         db: database to send commits through, or last db instance created if None
         """
-        if root:
+        if arche:
             muid = Muid(-1, -1, KEY_SET)
         database = database or Database.get_last()
         immediate = False
         if bundler is None:
             immediate = True
             bundler = Bundler(comment)
         if muid is None:
```

### Comparing `gink-0.20240401.1711930006/gink/impl/listener.py` & `gink-0.20240403.1712115567/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/lmdb_store.py` & `gink-0.20240403.1712115567/gink/impl/lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/lmdb_utilities.py` & `gink-0.20240403.1712115567/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/log_backed_store.py` & `gink-0.20240403.1712115567/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/memory_store.py` & `gink-0.20240403.1712115567/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/muid.py` & `gink-0.20240403.1712115567/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/pair_map.py` & `gink-0.20240403.1712115567/gink/impl/pair_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 from .graph import Vertex
 from .typedefs import GenericTimestamp, UserValue
 
 class PairMap(Container):
     _missing = object()
     BEHAVIOR = PAIR_MAP
 
-    def __init__(self, root: Optional[bool] = None, bundler: Optional[Bundler] = None,
+    def __init__(self, arche: Optional[bool] = None, bundler: Optional[Bundler] = None,
                  contents: Optional[dict] = None, muid: Optional[Muid] = None,
                  database = None, comment: Optional[str] = None):
         """
         Constructor for a pair set proxy.
 
         contents: dictionary of (Vertex, Vertex): Value to populate the pair map
         muid: the global id of this pair set, created on the fly if None
         db: database to send commits through, or last db instance created if None
         """
-        if root:
+        if arche:
             muid = Muid(-1, -1, PAIR_MAP)
         database = database or Database.get_last()
         immediate = False
         if bundler is None:
             immediate = True
             bundler = Bundler(comment)
         if muid is None:
@@ -107,15 +107,15 @@
     def __delitem__(self, key):
         self.delete(key)
 
     def dumps(self, as_of: GenericTimestamp = None) -> str:
         """ return the contents of this container as a string """
         as_of = self._database.resolve_timestamp(as_of)
         if self._muid.medallion == -1 and self._muid.timestamp == -1:
-            identifier = "root=True"
+            identifier = "arche=True"
         else:
             identifier = repr(str(self._muid))
         result = f"""{self.__class__.__name__}({identifier}, contents="""
         result += "{"
         stuffing = ""
         iterable = self._database.get_store().get_keyed_entries(
             container=self._muid, as_of=as_of, behavior=PAIR_MAP)
```

### Comparing `gink-0.20240401.1711930006/gink/impl/pair_set.py` & `gink-0.20240403.1712115567/gink/impl/pair_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 from .graph import Vertex
 from .typedefs import GenericTimestamp
 
 class PairSet(Container):
     _missing = object()
     BEHAVIOR = PAIR_SET
 
-    def __init__(self, root: Optional[bool] = None, bundler: Optional[Bundler] = None,
+    def __init__(self, arche: Optional[bool] = None, bundler: Optional[Bundler] = None,
                  contents: Union[Iterable[Tuple[Vertex, Vertex]], None] = None,
                  muid: Optional[Muid] = None, database = None, comment: Optional[str] = None):
         """
         Constructor for a pair set proxy.
 
         muid: the global id of this pair set, created on the fly if None
         contents: an iterable of pairs (an iterable of tuples) to populate the pair set at initialization
         db: database to send commits through, or last db instance created if None
         """
-        if root:
+        if arche:
             muid = Muid(-1, -1, PAIR_SET)
         database = database or Database.get_last()
         immediate = False
         if bundler is None:
             immediate = True
             bundler = Bundler(comment)
         if muid is None:
```

### Comparing `gink-0.20240401.1711930006/gink/impl/property.py` & `gink-0.20240403.1712115567/gink/impl/property.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 from .bundler import Bundler
 from .graph import Edge
 
 
 class Property(Container):
     BEHAVIOR = PROPERTY
 
-    def __init__(self, *, root: bool=False, muid: Optional[Muid] = None, database: Optional[Database]=None,
+    def __init__(self, *, arche: bool=False, muid: Optional[Muid] = None, database: Optional[Database]=None,
                  contents: Optional[Dict[Union[Container, Edge], Union[UserValue, Container]]]=None):
         """
         Constructor for a property definition.
 
         muid: the global id of this directory, created on the fly if None
         db: database send commits through, or last db instance created if None
         """
         database = database or Database.get_last()
         bundler = Bundler()
-        if root:
+        if arche:
             muid = Muid(-1, -1, PROPERTY)
         if muid is None:
             muid = Container._create(PROPERTY, database=database, bundler=bundler)
         Container.__init__(self, muid=muid, database=database)
         if contents:
             self.clear(bundler=bundler)
             self.update(contents, bundler=bundler)
@@ -36,15 +36,15 @@
         if len(bundler):
             self._database.commit(bundler)
 
     def dumps(self, as_of: GenericTimestamp = None) -> str:
         """ Dumps the contents of this property to a string.
         """
         if self._muid.medallion == -1 and self._muid.timestamp == -1:
-            identifier = "root=True"
+            identifier = "arche=True"
         else:
             identifier = repr(str(self._muid))
         result = f"""{self.__class__.__name__}({identifier}, contents="""
         result += "{"
         stuffing = [f"{k!r}:{v!r}" for k, v in self.items(as_of=as_of)]
         as_one_line = result + ",".join(stuffing) + "})"
         if len(as_one_line) < 80:
```

### Comparing `gink-0.20240401.1711930006/gink/impl/role.py` & `gink-0.20240403.1712115567/gink/impl/role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/selectable_console.py` & `gink-0.20240403.1712115567/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/sequence.py` & `gink-0.20240403.1712115567/gink/impl/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,26 +16,26 @@
     BEHAVIOR = SEQUENCE
 
     def __init__(self,
                  *ordered,
                  contents: Optional[Iterable] = None,
                  muid: Optional[Muid] = None,
                  database: Optional[Database] = None,
-                 root: bool = False,
+                 arche: bool = False,
                  bundler: Optional[Bundler] = None,
                  comment: Optional[str] = None,
                  ):
         """
         muid: the global id of this sequence, created on the fly if None
         database: where to send commits through, or last db instance created if None
         """
         if ordered:
             if isinstance(ordered[0], str):
                 muid = Muid.from_str(ordered[0])
-        if root:
+        if arche:
             muid = Muid(-1, -1, SEQUENCE)
         database = database or Database.get_last()
         immediate = False
         if bundler is None:
             immediate = True
             bundler = Bundler(comment)
         if muid is None:
@@ -52,15 +52,15 @@
 
     def __iter__(self):
         for thing in self.values():
             yield thing
 
     def dumps(self, as_of: GenericTimestamp = None) -> str:
         if self._muid.medallion == -1 and self._muid.timestamp == -1:
-            identifier = "root=True"
+            identifier = "arche=True"
         else:
             identifier = repr(str(self._muid))
         result = f"""{self.__class__.__name__}({identifier}, contents=["""
         stuffing = [repr(val) for val in self.values(as_of=as_of)]
         as_one_line = result + ", ".join(stuffing) + "])"
         if len(as_one_line) < 80:
             return as_one_line
```

### Comparing `gink-0.20240401.1711930006/gink/impl/tuples.py` & `gink-0.20240403.1712115567/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/typedefs.py` & `gink-0.20240403.1712115567/gink/impl/typedefs.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/utilities.py` & `gink-0.20240403.1712115567/gink/impl/utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/watcher.py` & `gink-0.20240403.1712115567/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/impl/websocket_connection.py` & `gink-0.20240403.1712115567/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_box.py` & `gink-0.20240403.1712115567/gink/tests/test_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
             global_box.set("test value")
             result = global_box.dumps()
 
             if global_box._muid.medallion != -1 and global_box._muid.timestamp != -1:
                 identifier = repr(str(global_box._muid))
             else:
-                identifier = "root=True"
+                identifier = "arche=True"
 
             assert result == f"""{global_box.__class__.__name__}({identifier}, contents='test value')"""
 
 
 
 def test_size():
     """ tests size method of Box class, returns either 1 or 0 """
```

### Comparing `gink-0.20240401.1711930006/gink/tests/test_chain_tracker.py` & `gink-0.20240403.1712115567/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_change_set_info.py` & `gink-0.20240403.1712115567/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_code_values.py` & `gink-0.20240403.1712115567/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_container.py` & `gink-0.20240403.1712115567/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_database.py` & `gink-0.20240403.1712115567/gink/tests/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,16 +115,16 @@
 
         store1a = store_class(path1)
         store1b = store_class(path1)
 
         db1a = Database(store1a)
         db1b = Database(store1b)
 
-        root1a = Directory(root=True, database=db1a)
-        root1b = Directory(root=True, database=db1b)
+        root1a = Directory(arche=True, database=db1a)
+        root1b = Directory(arche=True, database=db1b)
 
         db1b.run(0.01)
         bundle_infos = list()
         db1b.add_callback(lambda bi: bundle_infos.append(bi))
         root1a.set("foo", "bar", comment="abc")
         db1b.run(0.01)
         assert bundle_infos and bundle_infos[-1].comment == "abc"
```

### Comparing `gink-0.20240401.1711930006/gink/tests/test_demo.py` & `gink-0.20240403.1712115567/gink/tests/test_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def test_as_of():
     for store in [MemoryStore(), LmdbStore()]:
         with store:
             assert isinstance(store, AbstractStore)
             database = Database(store=store)
-            root = Directory(root=True, database=database)
+            root = Directory(arche=True, database=database)
             root["hello"] = "world"
             root["hello"] = "universe"
             assert root["hello"] == "universe"
             assert root.get("hello", as_of=-1) == "world"
             assert root.get("hello", as_of=-2) is None
             assert dict(root) == {"hello": "universe"}
             assert dict(root.items(as_of=-1)) == {"hello": "world"}, store
```

### Comparing `gink-0.20240401.1711930006/gink/tests/test_directory.py` & `gink-0.20240403.1712115567/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_graph.py` & `gink-0.20240403.1712115567/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_key_set.py` & `gink-0.20240403.1712115567/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_lmdb_store.py` & `gink-0.20240403.1712115567/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_logbackedstore.py` & `gink-0.20240403.1712115567/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_muid.py` & `gink-0.20240403.1712115567/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_names.py` & `gink-0.20240403.1712115567/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_pair_map.py` & `gink-0.20240403.1712115567/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_pair_set.py` & `gink-0.20240403.1712115567/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_property.py` & `gink-0.20240403.1712115567/gink/tests/test_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             namer = Property.get_global_instance(database=database)
             directory = Directory.get_global_instance()
             namer.set(directory, "fred")
             named = namer.get(directory)
             assert named == "fred", named
             assert namer.size() == 1, store
             dumped = namer.dumps()
-            assert dumped == "Property(root=True, contents={Directory(root=True):'fred'})", dumped
+            assert dumped == "Property(arche=True, contents={Directory(arche=True):'fred'})", dumped
             namer.set(directory, "joe")
             assert namer.get(directory) == "joe"
             eval(dumped)
             assert namer.get(directory) == "fred"
             namer.delete(directory)
             assert namer.size() ==  0
```

### Comparing `gink-0.20240401.1711930006/gink/tests/test_role.py` & `gink-0.20240403.1712115567/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_sequence.py` & `gink-0.20240403.1712115567/gink/tests/test_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """ test that I can create sequences and represent them """
     for store in [MemoryStore(), LmdbStore()]:
         with closing(store):
             database = Database(store=store)
             sequence = Sequence.get_global_instance(database)
             sequence.append("Hello, World!")
             assert list(sequence) == ["Hello, World!"]
-            assert repr(sequence) == "Sequence(root=True)"
+            assert repr(sequence) == "Sequence(arche=True)"
             sequence = Sequence(muid=Muid(1673009484969039, 362514588210531, 1))
             assert repr(sequence) == "Sequence('05F197E00EB44F-149B481419563-00001')"
 
 
 def test_basics():
     """ test that I can append and look at contents """
     for store in [MemoryStore(), LmdbStore()]:
@@ -227,11 +227,11 @@
     """ make sure that sequence.reset behaves as expected """
     for store in [LmdbStore()]:
         with closing(store):
             database = Database(store=store)
             queue = Sequence.get_global_instance(database)
             change_muid = queue.append("something")
             assert database.resolve_timestamp(-1) == change_muid.timestamp
-            assert queue.dumps() == "Sequence(root=True, contents=['something'])"
+            assert queue.dumps() == "Sequence(arche=True, contents=['something'])"
             reset_bundle = queue.reset(-1)
             assert reset_bundle is not None
-            assert queue.dumps() == "Sequence(root=True, contents=[])"
+            assert queue.dumps() == "Sequence(arche=True, contents=[])"
```

### Comparing `gink-0.20240401.1711930006/gink/tests/test_store.py` & `gink-0.20240403.1712115567/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink/tests/test_websocket_connection.py` & `gink-0.20240403.1712115567/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/gink.egg-info/PKG-INFO` & `gink-0.20240403.1712115567/gink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240401.1711930006
+Version: 0.20240403.1712115567
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240401.1711930006/gink.egg-info/SOURCES.txt` & `gink-0.20240403.1712115567/gink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gink-0.20240401.1711930006/setup.py` & `gink-0.20240403.1712115567/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240401.1711930006',
+    version='0.20240403.1712115567',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

