# Comparing `tmp/cval-lib-0.0.2.50.tar.gz` & `tmp/cval-lib-0.0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.2.50.tar", last modified: Wed Apr  3 17:16:55 2024, max compression
+gzip compressed data, was "cval-lib-0.0.2.8.tar", last modified: Fri Jul  7 10:26:12 2023, max compression
```

## Comparing `cval-lib-0.0.2.50.tar` & `cval-lib-0.0.2.8.tar`

### file list

```diff
@@ -1,78 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.152556 cval-lib-0.0.2.50/
--rw-rw-rw-   0        0        0    11558 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/LICENSE
--rw-rw-rw-   0        0        0      309 2024-04-03 17:16:55.151556 cval-lib-0.0.2.50/PKG-INFO
--rw-rw-rw-   0        0        0     7020 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.111556 cval-lib-0.0.2.50/cval_lib/
--rw-rw-rw-   0        0        0     2252 2024-04-03 17:16:05.000000 cval-lib-0.0.2.50/cval_lib/__init__.py
--rw-rw-rw-   0        0        0     8925 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/api.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.115556 cval-lib-0.0.2.50/cval_lib/configs/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/configs/__init__.py
--rw-rw-rw-   0        0        0      133 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/configs/main_config.py
--rw-rw-rw-   0        0        0     2707 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/connection.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.125556 cval-lib-0.0.2.50/cval_lib/examples/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/__init__.py
--rw-rw-rw-   0        0        0      421 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/annotation.py
--rw-rw-rw-   0        0        0      921 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/api.py
--rw-rw-rw-   0        0        0     1125 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/classification.py
--rw-rw-rw-   0        0        0     1678 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/dataset.py
--rw-rw-rw-   0        0        0     1489 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/detection.py
--rw-rw-rw-   0        0        0     1331 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/detection_entropy_multiclass.py
--rw-rw-rw-   0        0        0     2031 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/embeddings.py
--rw-rw-rw-   0        0        0     2181 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/embeddings_clustering.py
--rw-rw-rw-   0        0        0      975 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/frames.py
--rw-rw-rw-   0        0        0     3065 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/method_combination.py
--rw-rw-rw-   0        0        0     1283 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/monkey_patch.py
--rw-rw-rw-   0        0        0     1990 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/on_pemise.py
--rw-rw-rw-   0        0        0     2426 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/polling.py
--rw-rw-rw-   0        0        0     1407 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/examples/result.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.135556 cval-lib-0.0.2.50/cval_lib/handlers/
--rw-rw-rw-   0        0        0     1286 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/__async.py
--rw-rw-rw-   0        0        0        0 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/__init__.py
--rw-rw-rw-   0        0        0     3249 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/_abstract_handler.py
--rw-rw-rw-   0        0        0     1229 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/_based_on_json.py
--rw-rw-rw-   0        0        0     3845 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/annotation.py
--rw-rw-rw-   0        0        0     2036 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/classification.py
--rw-rw-rw-   0        0        0     5373 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/dataset.py
--rw-rw-rw-   0        0        0     2443 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/detection.py
--rw-rw-rw-   0        0        0     4970 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/embedding.py
--rw-rw-rw-   0        0        0      984 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/frame.py
--rw-rw-rw-   0        0        0     2746 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/frames.py
--rw-rw-rw-   0        0        0     2818 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/result.py
--rw-rw-rw-   0        0        0     2747 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/storage.py
--rw-rw-rw-   0        0        0     1302 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/handlers/weights.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.143556 cval-lib-0.0.2.50/cval_lib/models/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/__init__.py
--rw-rw-rw-   0        0        0      849 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/_base.py
--rw-rw-rw-   0        0        0     3175 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/annotation.py
--rw-rw-rw-   0        0        0     3207 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/classification.py
--rw-rw-rw-   0        0        0     2939 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/dataset.py
--rw-rw-rw-   0        0        0     6419 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/detection.py
--rw-rw-rw-   0        0        0     2092 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/embedding.py
--rw-rw-rw-   0        0        0     1633 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/frame.py
--rw-rw-rw-   0        0        0      488 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/queue.py
--rw-rw-rw-   0        0        0     2913 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/result.py
--rw-rw-rw-   0        0        0     1007 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/storage.py
--rw-rw-rw-   0        0        0     2454 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/models/weights.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.144556 cval-lib-0.0.2.50/cval_lib/patterns/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/patterns/__init__.py
--rw-rw-rw-   0        0        0      248 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/patterns/singleton.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.146556 cval-lib-0.0.2.50/cval_lib/tools/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/tools/__init__.py
--rw-rw-rw-   0        0        0     3690 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/tools/annotation.py
--rw-rw-rw-   0        0        0    12914 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/tools/get_embeddings.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.150556 cval-lib-0.0.2.50/cval_lib/utils/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/utils/__init__.py
--rw-rw-rw-   0        0        0      946 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/utils/base_conn.py
--rw-rw-rw-   0        0        0     2195 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/utils/entrypoint.py
--rw-rw-rw-   0        0        0      801 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/utils/exceptions.py
--rw-rw-rw-   0        0        0      419 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/utils/install_dynamically.py
--rw-rw-rw-   0        0        0     1782 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/utils/lib_tools.py
--rw-rw-rw-   0        0        0      968 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/cval_lib/utils/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:16:55.151556 cval-lib-0.0.2.50/cval_lib.egg-info/
--rw-rw-rw-   0        0        0      309 2024-04-03 17:16:55.000000 cval-lib-0.0.2.50/cval_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3789 2024-04-03 17:16:55.000000 cval-lib-0.0.2.50/cval_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 17:16:55.000000 cval-lib-0.0.2.50/cval_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-03 17:16:55.000000 cval-lib-0.0.2.50/cval_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-03 17:16:55.000000 cval-lib-0.0.2.50/cval_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 17:16:55.152556 cval-lib-0.0.2.50/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-04-03 17:02:25.000000 cval-lib-0.0.2.50/setup.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/LICENSE
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     6568 2023-07-07 09:13:46.000000 cval-lib-0.0.2.8/README.md
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.8/cval_lib/__init__.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/configs/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/configs/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.8/cval_lib/configs/main_config.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/connection.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/examples/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/examples/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1637 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1829 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/embeddings.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1258 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/monkey_patch.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/on_pemise.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2367 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/polling.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1383 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/examples/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/handlers/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/handlers/__async.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/handlers/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/_abstract_handler.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.8/cval_lib/handlers/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1984 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/handlers/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.8/cval_lib/handlers/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/frame.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/frames.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2449 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/handlers/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/models/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/models/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/models/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.8/cval_lib/models/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.8/cval_lib/models/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2210 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/models/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/patterns/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/patterns/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/patterns/singleton.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib.egg-info/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1083 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/requires.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/top_level.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/setup.cfg
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      448 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/setup.py
```

### Comparing `cval-lib-0.0.2.50/LICENSE` & `cval-lib-0.0.2.8/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `cval-lib-0.0.2.50/cval_lib/examples/dataset.py` & `cval-lib-0.0.2.8/cval_lib/examples/dataset.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-
-if __name__ == '__main__':
-    from cval_lib.connection import CVALConnection
-
-    # set up your user_api_key
-    user_api_key = 'USER_API_KEY'
-    # set up session
-    cval = CVALConnection(user_api_key)
-    # choose strategy
-    ds = cval.dataset()
-    # create your dataset
-    ds_id = ds.create()
-    print(ds_id)
-    # update your dataset
-    update = ds.update(name='any')
-    print('', update)
-    # watch changes
-    get = ds.get()
-    print(get)
-    # also you can use dataset_id for watch changes
-    get = ds.get(ds_id)
-    print(get)
-    # get all datasets
-    print(ds.get_all())
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+
+if __name__ == '__main__':
+    from cval_lib.connection import CVALConnection
+
+    # set up your user_api_key
+    user_api_key = 'USER_API_KEY'
+    # set up session
+    cval = CVALConnection(user_api_key)
+    # choose strategy
+    ds = cval.dataset()
+    # create your dataset
+    ds_id = ds.create()
+    print(ds_id)
+    # update your dataset
+    update = ds.update(name='any')
+    print('', update)
+    # watch changes
+    get = ds.get()
+    print(get)
+    # also you can use dataset_id for watch changes
+    get = ds.get(ds_id)
+    print(get)
+    # get all datasets
+    print(ds.get_all())
```

### Comparing `cval-lib-0.0.2.50/cval_lib/examples/embeddings.py` & `cval-lib-0.0.2.8/cval_lib/examples/embeddings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-import time
-
-if __name__ == '__main__':
-    from random import random
-    import uuid
-
-    from cval_lib.connection import CVALConnection
-    from cval_lib.models.embedding import EmbeddingModel, FrameEmbeddingModel
-
-    embeddings = tuple(
-        map(
-            lambda x: FrameEmbeddingModel(
-                frame_id=uuid.uuid4().hex,
-                embeddings=[
-                    EmbeddingModel(embedding_id=uuid.uuid4().hex, embedding=list(map(lambda x: random(), range(500))))]
-            ),
-            range(10_000)
-        )
-    )
-
-    print(embeddings)
-    user_api_key = '50b524bcae7b7bf77e2fcd34fefaf6c7192cbeef1ea55939d5f86a88f42bc809'
-    cval = CVALConnection(user_api_key)
-    ds = cval.dataset()
-    emb = cval.embedding(ds.create(), 'training')
-    t0 = time.time()
-    emb.upload_many(embeddings)
-    t1 = time.time()
-    print(t1-t0)
-    ds.embedding(part_of_dataset='training').get_many()
-    print(emb.get_many())
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+if __name__ == '__main__':
+    from random import random
+    import uuid
+
+    from cval_lib.connection import CVALConnection
+    from cval_lib.models.embedding import ImageEmbeddingModel
+
+    img_id_1 = str(uuid.uuid4().hex)
+    img_id_2 = str(uuid.uuid4().hex)
+
+    embeddings = [
+        ImageEmbeddingModel(id=img_id_1, image_embedding=list(map(lambda x: random(), range(1000)))),
+        ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(), range(1000)))),
+    ]
+
+    print(embeddings)
+    user_api_key = 'USER_API_KEY'
+    cval = CVALConnection(user_api_key)
+    ds = cval.dataset()
+    ds.create()
+    emb = cval.embedding("ID", 'training')
+    emb.upload_many(embeddings)
+    ds.embedding(type_of_dataset='training').get_many()
+    print(emb.get_many())
```

### Comparing `cval-lib-0.0.2.50/cval_lib/examples/monkey_patch.py` & `cval-lib-0.0.2.8/cval_lib/examples/monkey_patch.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-
-if __name__ == '__main__':
-    from cval_lib.connection import CVALConnection
-    api_key = 'USER_API_KEY'
-    cval = CVALConnection(api_key)
-    ds = cval.dataset()
-    ds.create()
-    print(ds.result.get_many())
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+
+if __name__ == '__main__':
+    from cval_lib.connection import CVALConnection
+    api_key = 'USER_API_KEY'
+    cval = CVALConnection(api_key)
+    ds = cval.dataset()
+    ds.create()
+    print(ds.result.get_many())
```

### Comparing `cval-lib-0.0.2.50/cval_lib/examples/on_pemise.py` & `cval-lib-0.0.2.8/cval_lib/examples/on_pemise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-if __name__ == '__main__':
-    from random import random, randint
-
-    from cval_lib.connection import CVALConnection
-    from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
-
-    frames_predictions = list(
-        map(
-            lambda x: FramePrediction(
-                frame_id=randint(0, 100),
-                predictions=list(map(lambda _: BBoxScores(category_id=randint(0, 100), score=random()), range(100)))
-            ),
-            range(100)
-        )
-    )
-
-    print(frames_predictions)
-
-    request = DetectionSamplingOnPremise(
-        num_of_samples=200,
-        bbox_selection_policy='min',
-        selection_strategy='margin',
-        sort_strategy='ascending',
-        frames=frames_predictions,
-    )
-    api_key = ...
-    cval = CVALConnection(api_key)
-    detection = cval.detection()
-    print(detection.on_premise_sampling(request))
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+if __name__ == '__main__':
+    import uuid
+    from random import random
+
+    from cval_lib.connection import CVALConnection
+    from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
+
+    frames_predictions = list(
+        map(
+            lambda x: FramePrediction(
+                frame_id=str(uuid.uuid4().hex),
+                predictions=list(map(lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
+            ),
+            range(100)
+        )
+    )
+
+    print(frames_predictions)
+
+    request = DetectionSamplingOnPremise(
+        num_of_samples=200,
+        bbox_selection_policy='min',
+        selection_strategy='margin',
+        sort_strategy='ascending',
+        frames=frames_predictions,
+    )
+    api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
+    cval = CVALConnection(api_key)
+    detection = cval.detection()
+    print(detection.on_premise_sampling(request))
```

### Comparing `cval-lib-0.0.2.50/cval_lib/examples/polling.py` & `cval-lib-0.0.2.8/cval_lib/examples/polling.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-if __name__ == '__main__':
-    import uuid
-    from random import random
-    from time import sleep
-
-    from cval_lib.connection import CVALConnection
-    from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
-
-    frames_predictions = list(
-            map(
-                lambda x: FramePrediction(
-                    frame_id=str(uuid.uuid4().hex),
-                    predictions=list(
-                        map(
-                            lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()),
-                            range(10000)
-                        ),
-                    )
-                ),
-                range(10000)
-            )
-        )
-
-    request = DetectionSamplingOnPremise(
-            num_of_samples=200,
-            bbox_selection_policy='min',
-            selection_strategy='margin',
-            sort_strategy='ascending',
-            frames=frames_predictions,
-        )
-    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
-    cval = CVALConnection(user_api_key)
-    emb = cval.detection()
-    result = None
-    sleep_sec = 1
-
-    while result is None:
-        result = emb.result.get()
-        print(f'Polling... {sleep_sec} s')
-        sleep(sleep_sec)
-        sleep_sec *= 2
-    print(result)
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+if __name__ == '__main__':
+    import uuid
+    from random import random
+    from time import sleep
+
+    from cval_lib.connection import CVALConnection
+    from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
+
+    frames_predictions = list(
+            map(
+                lambda x: FramePrediction(
+                    frame_id=str(uuid.uuid4().hex),
+                    predictions=list(
+                        map(
+                            lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()),
+                            range(10000)
+                        ),
+                    )
+                ),
+                range(10000)
+            )
+        )
+
+    request = DetectionSamplingOnPremise(
+            num_of_samples=200,
+            bbox_selection_policy='min',
+            selection_strategy='margin',
+            sort_strategy='ascending',
+            frames=frames_predictions,
+        )
+    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
+    cval = CVALConnection(user_api_key)
+    emb = cval.detection()
+    result = None
+    sleep_sec = 1
+
+    while result is None:
+        result = emb.result.get()
+        print(f'Polling... {sleep_sec} s')
+        sleep(sleep_sec)
+        sleep_sec *= 2
+    print(result)
```

### Comparing `cval-lib-0.0.2.50/cval_lib/examples/result.py` & `cval-lib-0.0.2.8/cval_lib/examples/result.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-
-if __name__ == '__main__':
-    from cval_lib.connection import CVALConnection
-    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
-    cval = CVALConnection(user_api_key)
-    print(cval.result().get('ecb8a52b-9bc0-4e56-a496-e69ce74cc0ec'))
-    print(cval.result().get(cval.result().get_many()[0].task_id))
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+
+if __name__ == '__main__':
+    from cval_lib.connection import CVALConnection
+    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
+    cval = CVALConnection(user_api_key)
+    print(cval.result().get('ecb8a52b-9bc0-4e56-a496-e69ce74cc0ec'))
+    print(cval.result().get(cval.result().get_many()[0].task_id))
```

### Comparing `cval-lib-0.0.2.50/cval_lib/handlers/__async.py` & `cval-lib-0.0.2.8/cval_lib/handlers/__async.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-import asyncio
-
-
-def asyncio_runner(func, *args, **kwargs):
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    res = loop.run_until_complete(func(*args, *kwargs))
-    loop.close()
-    return res
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+import asyncio
+
+
+def asyncio_runner(func, *args, **kwargs):
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
+    res = loop.run_until_complete(func(*args, *kwargs))
+    loop.close()
+    return res
```

### Comparing `cval-lib-0.0.2.50/cval_lib/handlers/_abstract_handler.py` & `cval-lib-0.0.2.8/cval_lib/handlers/_abstract_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,76 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-from functools import wraps
-
-from requests import Request, Session, Response
-
-from cval_lib.utils.exceptions import (
-    Forbidden,
-    Conflict,
-    NotFound,
-    NotAcceptable,
-    SchemaException,
-    UnknownException,
-)
-
-
-class AbstractHandler(Request):
-    __exceptions_chain__ = (
-        Forbidden,
-        Conflict,
-        NotFound,
-        NotAcceptable,
-        SchemaException
-    )
-
-    def __init__(self, session: Session, sub: str = '', url='',):
-        self.session = session
-        self.sub = sub
-
-        super().__init__(
-            method=None,
-            url=url,
-            headers=session.headers,
-            files=None,
-            data=None,
-            params=None,
-            auth=None,
-            cookies=None,
-            hooks=None,
-            json=None,
-        )
-
-    @staticmethod
-    def pos_val(func):
-        @wraps(func)
-        def _(*args, **kwargs):
-            if args:
-                raise ValueError()
-            return func(**kwargs)
-        return _
-
-    def _get(self, url: str, params=None, stream=False, json=None):
-        self.url = url
-        self.method = 'get'
-        self.params = params
-        self.stream = stream
-
-    def _delete(self, url: str, params=None, json=None):
-        self._get(url, params=params)
-        self.method = 'delete'
-
-    def _post(self, url: str, json=None, params=None, stream=False, files=None):
-        self._get(url, params=params, stream=stream)
-        self.method = 'post'
-        self.json = json
-        self.files = files
-
-    def _put(self, url: str, json=None, params=None, stream=False, files=None):
-        self._post(url, json, params, stream=stream, files=files)
-        self.method = 'put'
-
-    def _validate_response(self, resp: Response):
-        if resp.status_code >= 400:
-            for exc in self.__exceptions_chain__:
-                exc().handle(resp)
-            raise UnknownException((resp.json()) if resp.status_code != 500 else 'Internal Server Error :(')
-
-    def send(self):
-        resp = self.session.send(self.prepare())
-        self._validate_response(resp)
-        return resp
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+from functools import wraps
+
+from requests import Request, Session, Response
+
+
+class AbstractHandler(Request):
+    def __init__(self, session: Session, sub: str = '', url=''):
+        self.session = session
+        self.sub = sub
+        super().__init__(
+            method=None,
+            url=url,
+            headers=session.headers,
+            files=None,
+            data=None,
+            params=None,
+            auth=None,
+            cookies=None,
+            hooks=None,
+            json=None,
+        )
+
+    @staticmethod
+    def pos_val(func):
+        @wraps(func)
+        def _(*args, **kwargs):
+            if args:
+                raise ValueError()
+            return func(**kwargs)
+        return _
+
+    def _get(self, url: str, params=None, stream=False):
+        self.url = url
+        self.method = 'get'
+        self.params = params
+        self.stream = stream
+
+    def _delete(self, url: str, params=None):
+        self._get(url, params=params)
+        self.method = 'delete'
+
+    def _post(self, url: str, json=None, params=None, stream=False, **files):
+        self._get(url, params=params, stream=stream)
+        self.method = 'post'
+        self.json = json
+        self.files = files
+
+    def _put(self, url: str, json=None, params=None, stream=False, **files):
+        self._post(url, json, params, stream=stream, **files)
+        self.method = 'put'
+
+    @staticmethod
+    def validate_response(resp: Response):
+        if resp.status_code >= 400:
+            raise Exception(resp.json() if resp.status_code != 500 else 'Internal Server Error :(')
+
+    def send(self):
+        resp = self.session.send(self.prepare())
+        self.validate_response(resp)
+        return resp
```

### Comparing `cval-lib-0.0.2.50/cval_lib/handlers/classification.py` & `cval-lib-0.0.2.8/cval_lib/handlers/result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,60 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-from cval_lib.handlers._based_on_json import BasedOnJSON
-from cval_lib.models.classification import (
-    ClassificationTest,
-    ClassificationSampling,
-)
-from cval_lib.models.result import ResultResponse
-
-
-class Classification(BasedOnJSON):
-    def saas_sampling(self, dataset_id, config: ClassificationSampling) -> ResultResponse:
-        """
-        Start Active Learning selection for a specific dataset ID.
-        """
-        return self.__processing__(
-            f'/dataset/{dataset_id}/sampling/classification',
-            self._post,
-            ResultResponse,
-            config,
-        )
-
-    def saas_test(self, dataset_id: str, config: ClassificationTest) -> ResultResponse:
-        """
-        Start model test for a specific dataset ID.
-        """
-        return self.__processing__(
-            f'/dataset/{dataset_id}/test/classification',
-            self._post,
-            ResultResponse,
-            config,
-        )
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+from requests import Session
+
+from cval_lib.configs.main_config import MainConfig
+from cval_lib.handlers._abstract_handler import AbstractHandler
+from cval_lib.models.result import ResultResponse
+
+
+class Result(AbstractHandler):
+    """
+    The result is the entity in which the processing data is stored
+    """
+    def __init__(
+            self,
+            session: Session,
+    ):
+        self.route = f'{MainConfig.main_url}/result'
+        self.result_id = None
+        super().__init__(session)
+
+    def _set_result_id(self, result_id: str = None):
+        if result_id is None:
+            result_id = self.result_id
+        if result_id is None:
+            raise ValueError('task_id cannot be None')
+        self.result_id = result_id
+
+    def get(self, result_id: str = None) -> ResultResponse:
+        """
+        :param result_id: id of result
+        :return: ResultResponse
+        """
+        self._set_result_id(result_id)
+        self._get(self.route + f'/{self.result_id}')
+        return ResultResponse.parse_obj(self.send().json())
+
+    def get_many(self, dataset_id: str = None, limit=100, ):
+        """
+        :param dataset_id: id of dataset
+        :param limit: limit of returned objects
+        :return:
+        """
+        self._get(self.route + 's', params={'limit': limit, 'dataset_id': dataset_id})
+        return [ResultResponse.parse_obj(i) for i in self.send().json()]
```

### Comparing `cval-lib-0.0.2.50/cval_lib/handlers/dataset.py` & `cval-lib-0.0.2.8/cval_lib/handlers/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,127 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-from typing import List
-
-from requests import Session
-
-from cval_lib.configs.main_config import MainConfig
-from cval_lib.handlers._abstract_handler import AbstractHandler
-from cval_lib.handlers.detection import Detection
-from cval_lib.handlers.embedding import Embedding
-from cval_lib.handlers.result import Result
-from cval_lib.models.dataset import DatasetModel, DatasetResponse
-
-
-class Dataset(AbstractHandler):
-    """
-    Within the framework of the created system,
-    datasets are spaces in which data for machine learning is stored.
-    Creating a dataset is similar to creating a folder.
-    """
-
-    def __init__(self, session: Session):
-        self.dataset_request = DatasetModel(dataset_name='', dataset_description='')
-        self.route = f'{MainConfig().main_url}/dataset'
-        self.dataset_id = None
-        self.result = Result(session)
-        self._embedding = Embedding(session, _is_not_second=False)
-        self.embedding = self._embedding.monkey_patch_url
-        self.detection = Detection(session)
-        super().__init__(session)
-
-    def __repr__(self):
-        return f'<dataset {self.dataset_id}>'
-
-    def _construct_request(self, name: str, description: str):
-        self.dataset_request = DatasetModel()
-        if name is not None:
-            self.dataset_request.dataset_name = name
-        if description is not None:
-            self.dataset_request.dataset_description = description
-
-    def create(
-            self,
-            name: str = None,
-            description: str = None,
-    ) -> str:
-        """
-        this method creates a dataset
-        :param name: the name of dataset
-        :param description: the name of dataset
-        :return: id of dataset (dataset_id)
-        """
-        self._construct_request(name, description)
-        self._post(url=self.route, json=self.dataset_request.dict())
-        self.dataset_id = self.send().json().get('dataset_id')
-        self._embedding.dataset_id = self.dataset_id
-        return self.dataset_id
-
-    def update(
-            self,
-            dataset_id: str = None,
-            name: str = None,
-            description: str = None,
-    ) -> 'DatasetModel':
-        """
-        this method updates a dataset
-        :param dataset_id: id of dataset
-        :param name: the name of dataset
-        :param description: the description of dataset
-        :return: DatasetResponse model with updates
-        """
-        dataset_id = self.set_dataset_id(dataset_id)
-        self._construct_request(name, description)
-        self._put(url=self.route + f'/{dataset_id}', json=self.dataset_request.dict(), )
-        self.dataset_request = self.send().json()
-        return self.dataset_request
-
-    def set_dataset_id(self, dataset_id: str = None):
-        if dataset_id is None:
-            dataset_id = self.dataset_id
-        self.dataset_id = dataset_id
-        if self.dataset_id is None:
-            raise ValueError('dataset_id cannot be None')
-        self._embedding.dataset_id = dataset_id
-        return self.dataset_id
-
-    def get(
-            self,
-            dataset_id: str = None,
-    ) -> 'DatasetModel':
-        """
-        this method returns a dataset name and description by dataset_id
-        :param dataset_id: id of dataset
-        :return: DatasetResponse model with updates
-        """
-        dataset_id = self.set_dataset_id(dataset_id)
-        self._get(url=self.route + f'/{dataset_id}')
-        return DatasetModel.parse_obj(self.send().json())
-
-    def get_all(
-            self,
-            name: str = None,
-            description: str = None,
-    ) -> List['DatasetResponse']:
-        """
-        this method returns a dataset name and description by dataset_id
-        :param name: the name of dataset. regexp
-        :param description: the description of dataset. regexp
-        :return: DatasetResponse model with updates
-        """
-        self._construct_request(name, description)
-        self._get(url=self.route + 's/all', params=self.dataset_request.dict())
-        return [DatasetResponse.parse_obj(i) for i in self.send().json()]
-
-    def synchronize(self, _id):
-        self._put(f"{self.route}/{_id}/synchronize")
-        return self.send()
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+from typing import List
+
+from requests import Session
+
+from cval_lib.configs.main_config import MainConfig
+from cval_lib.handlers._abstract_handler import AbstractHandler
+from cval_lib.handlers.detection import Detection
+from cval_lib.handlers.embedding import Embedding
+from cval_lib.handlers.result import Result
+from cval_lib.models.dataset import DatasetModel, DatasetResponse
+
+
+class Dataset(AbstractHandler):
+    """
+    Within the framework of the created system,
+    datasets are spaces in which data for machine learning is stored.
+    Creating a dataset is similar to creating a folder.
+    """
+    def __init__(self, session: Session):
+        self.dataset_request = DatasetModel()
+        self.route = f'{MainConfig().main_url}/dataset'
+        self.dataset_id = None
+        self.result = Result(session)
+        self._embedding = Embedding(session, _is_not_second=False)
+        self.embedding = self._embedding.monkey_patch_url
+        self.detection = Detection(session)
+        super().__init__(session)
+
+    def __repr__(self):
+        return f'<dataset {self.dataset_id}>'
+
+    def _construct_request(self, name: str, description: str):
+        self.dataset_request = DatasetModel()
+        if name is not None:
+            self.dataset_request.dataset_name = name
+        if description is not None:
+            self.dataset_request.dataset_description = description
+
+    def create(
+            self,
+            name: str = None,
+            description: str = None,
+    ) -> str:
+        """
+        this method creates a dataset
+        :param name: the name of dataset
+        :param description: the name of dataset
+        :return: id of dataset (dataset_id)
+        """
+        self._construct_request(name, description)
+        self._post(url=self.route, json=self.dataset_request.dict())
+        self.dataset_id = self.send().json().get('dataset_id')
+        self._embedding.dataset_id = self.dataset_id
+        return self.dataset_id
+
+    def update(
+            self,
+            dataset_id: str = None,
+            name: str = None,
+            description: str = None,
+    ) -> DatasetModel:
+        """
+        this method updates a dataset
+        :param dataset_id: id of dataset
+        :param name: the name of dataset
+        :param description: the description of dataset
+        :return: DatasetResponse model with updates
+        """
+        dataset_id = self.set_dataset_id(dataset_id)
+        self._construct_request(name, description)
+        self._put(url=self.route+f'/{dataset_id}', json=self.dataset_request.dict(), )
+        self.dataset_request = self.send().json()
+        return self.dataset_request
+
+    def set_dataset_id(self, dataset_id: str = None):
+        if dataset_id is None:
+            dataset_id = self.dataset_id
+        self.dataset_id = dataset_id
+        if self.dataset_id is None:
+            raise ValueError('dataset_id cannot be None')
+        self._embedding.dataset_id = dataset_id
+        return self.dataset_id
+
+    def get(
+            self,
+            dataset_id: str = None,
+    ) -> DatasetModel:
+        """
+        this method returns a dataset name and description by dataset_id
+        :param dataset_id: id of dataset
+        :return: DatasetResponse model with updates
+        """
+        dataset_id = self.set_dataset_id(dataset_id)
+        self._get(url=self.route+f'/{dataset_id}')
+        return DatasetModel.parse_obj(self.send().json())
+
+    def get_all(
+            self,
+            name: str = None,
+            description: str = None,
+    ) -> List[DatasetResponse]:
+        """
+        this method returns a dataset name and description by dataset_id
+        :param name: the name of dataset. regexp
+        :param description: the description of dataset. regexp
+        :return: DatasetResponse model with updates
+        """
+        self._construct_request(name, description)
+        self._get(url=self.route+'s/all', params=self.dataset_request.dict())
+        return [DatasetResponse.parse_obj(i) for i in self.send().json()]
```

### Comparing `cval-lib-0.0.2.50/cval_lib/handlers/embedding.py` & `cval-lib-0.0.2.8/cval_lib/handlers/embedding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,115 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-from typing import List
-
-from requests import Session, Response
-
-from cval_lib.configs.main_config import MainConfig
-from cval_lib.handlers._abstract_handler import AbstractHandler
-from cval_lib.models.embedding import FrameEmbeddingModel, EmbeddingsMetaResponse
-
-
-class Embedding(AbstractHandler):
-    """
-    Embeddings are vector representations of images
-    obtained using pytorch or any other library
-    """
-
-    def __init__(
-            self,
-            session: Session,
-            dataset_id: str = None,
-            part_of_dataset: str = None,
-            _is_not_second=True,
-    ):
-        if _is_not_second and dataset_id is None:
-            raise ValueError('dataset_id must be not None')
-        if _is_not_second and part_of_dataset is None:
-            raise ValueError('part_of_dataset must be not None')
-        self.dataset_id = dataset_id
-        self.part_of_dataset = part_of_dataset
-        self.route = f'{MainConfig().main_url}/dataset/{dataset_id}/{part_of_dataset}/'
-        super().__init__(session)
-
-    def monkey_patch_url(self, part_of_dataset: str, ) -> 'Embedding':
-        self.part_of_dataset = part_of_dataset
-        return self
-
-    def get_meta(self, start_limit: int = 0, stop_limit: int = 1000) -> 'EmbeddingsMetaResponse':
-        """
-        :param start_limit: upper limit of items
-        :param stop_limit: lower limit of items
-        :return: List[ImageEmbeddingModel]
-        """
-        self._get(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.part_of_dataset}/embeddings/meta',
-                  params={'start_limit': start_limit, 'stop_limit': stop_limit})
-        return EmbeddingsMetaResponse.parse_obj(self.send().json())
-
-    def get_many(self, start_limit: int = 0, stop_limit: int = 1000) -> List['FrameEmbeddingModel']:
-        """
-        :param start_limit: upper limit of items
-        :param stop_limit: lower limit of items
-        :return: List[ImageEmbeddingModel]
-        """
-        self._get(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.part_of_dataset}/embeddings',
-                  params={'start_limit': start_limit, 'stop_limit': stop_limit})
-        return [FrameEmbeddingModel.parse_obj(i) for i in self.send().json()]
-
-    def get_by_id(
-            self,
-            frame_id: str,
-            embedding_id: str,
-    ) -> 'FrameEmbeddingModel':
-        """
-        :param embedding_id: id of embedding
-        :param frame_id: id of frame
-        :return: ImageEmbeddingModel
-        """
-        self._get(self.route + f'/embedding/{frame_id}/{embedding_id}')
-        return FrameEmbeddingModel.parse_obj(self.send().json())
-
-    def upload_many(self, embeddings: List[FrameEmbeddingModel]) -> 'EmbeddingsMetaResponse':
-        """
-        :param embeddings: List[ImageEmbeddingModel]
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._post(
-            f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.part_of_dataset}/embeddings',
-            json=[i.dict() if not isinstance(i, dict) else i for i in embeddings]
-        )
-        return EmbeddingsMetaResponse.parse_obj(self.send().json())
-
-    def delete_all(self, ) -> Response:
-        """
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._delete(self.route + 'embeddings')
-        return self.send()
-
-    def delete_by_id(self, frame_id: str, embedding_id: str = 'all') -> Response:
-        """
-        :param embedding_id: id of embedding
-        :param frame_id: id of frame
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._delete(self.route + f'embedding/{frame_id}/{embedding_id}')
-        return self.send()
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+from typing import List
+from requests import Session, Response
+
+from cval_lib.configs.main_config import MainConfig
+from cval_lib.handlers._abstract_handler import AbstractHandler
+from cval_lib.models.embedding import ImageEmbeddingModel
+
+
+class Embedding(AbstractHandler):
+    """
+    Embeddings are vector representations of images
+    obtained using pytorch or any other library
+    """
+    def __init__(
+            self,
+            session: Session,
+            dataset_id: str = None,
+            type_of_dataset: str = None,
+            _is_not_second=True
+    ):
+        if _is_not_second and dataset_id is None:
+            raise ValueError('dataset_id must be not None')
+        if _is_not_second and type_of_dataset is None:
+            raise ValueError('type_of_dataset must be not None')
+        self.dataset_id = dataset_id
+        self.type_of_dataset = type_of_dataset
+        self.route = f'{MainConfig().main_url}/dataset/{dataset_id}/{type_of_dataset}/'
+        super().__init__(session)
+
+    def monkey_patch_url(self, type_of_dataset: str, ) -> None:
+        self.route = f'{MainConfig().main_url}/dataset/{self.dataset_id}/{type_of_dataset}/'
+        return self
+
+    def get_many(self, start_limit: int = 0, stop_limit: int = 1000) -> List[ImageEmbeddingModel]:
+        """
+        :param start_limit: upper limit of items
+        :param stop_limit: lower limit of items
+        :return: List[ImageEmbeddingModel]
+        """
+        self._get(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.type_of_dataset}/embeddings', params={'start_limit': start_limit, 'stop_limit': stop_limit})
+        return [ImageEmbeddingModel.parse_obj(i) for i in self.send().json()]
+
+    def get_by_id(self, embedding_id: str, ) -> [ImageEmbeddingModel]:
+        """
+        :param embedding_id: id of embedding
+        :return: ImageEmbeddingModel
+        """
+        self._get(self.route + f'embedding/{embedding_id}')
+        return ImageEmbeddingModel.parse_obj(self.send().json())
+
+    def upload_many(self, embeddings: List[ImageEmbeddingModel]) -> Response:
+        """
+        :param embeddings: List[ImageEmbeddingModel]
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._post(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.type_of_dataset}/embeddings', json=[i.dict() for i in embeddings])
+        return self.send()
+
+    def upload_by_id(self, embedding_id: str, embedding: ImageEmbeddingModel) -> Response:
+        """
+        :param embedding: List[ImageEmbeddingModel]
+        :param embedding_id: id of embedding
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._post(self.route + f'/embedding/{embedding_id}', json=embedding.dict())
+        return self.send()
+
+    def update_many(self, embeddings: List[ImageEmbeddingModel]) -> Response:
+        """
+        :param embeddings: List[ImageEmbeddingModel]
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._put(self.route + f'embeddings', json=[i.dict() for i in embeddings])
+        return self.send()
+
+    def update_by_id(self, embedding_id: str, embedding: ImageEmbeddingModel) -> Response:
+        """
+        :param embedding: List[ImageEmbeddingModel]
+        :param embedding_id: id of embedding
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._put(self.route + f'embedding/{embedding_id}', json=embedding.dict())
+        return self.send()
+
+    def delete_all(self) -> Response:
+        """
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._delete(self.route + f'embeddings')
+        return self.send()
+
+    def delete_by_id(self, embedding_id: str) -> Response:
+        """
+        :param embedding_id: id of embedding
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._delete(self.route + f'embedding/{embedding_id}')
+        return self.send()
```

### Comparing `cval-lib-0.0.2.50/cval_lib/models/weights.py` & `cval-lib-0.0.2.8/cval_lib/models/result.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,61 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-from __future__ import annotations
-
-from typing import Optional
-
-from pydantic import BaseModel
-
-from typing import List
-
-from cval_lib.models._base import fields
-
-
-@fields(
-    'weights_id: str',
-    'retrain_model: bool = False',
-    'weights_version: Optional[str]',
-)
-class WeightsConfigModel(BaseModel):
-    """
-    :param weights_id: weights ID to be used in active learning
-    :param retrain_model: perform a model retrain
-    :param weights_version: Weights Version to be used in the operation
-    """
-    weights_id: str
-    retrain_model: bool = False
-    weights_version: Optional[str]
-
-
-@fields(
-    'ID: str',
-    'timestamp: float',
-    'ver: str',
-    'task_id: str',
-)
-class Version(BaseModel):
-    """
-    :param ID: internal id of version
-    :param timestamp: UNIX timestamp creation time
-    :param ver: version
-    :param task_id: id of task
-    """
-    ID: str
-    timestamp: float
-    ver: str
-    task_id: str
-
-
-@fields(
-    'ID: str',
-    'model: float',
-)
-class WeightsOfModel(BaseModel):
-    ID: str
-    model: str
-
-
-@fields(
-    'weights_of_model: WeightsOfModel',
-    'versions: List[Version]',
-)
-class WeightsBase(BaseModel):
-    """
-    :param weights_of_model: internal id of version
-    :param versions: list of versions
-    """
-    weights_of_model: WeightsOfModel
-    versions: List[Version]
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+from typing import Any
+
+from pydantic import BaseModel
+
+
+class WeightsConfigResponse(BaseModel):
+    """
+    :param weights_id: id of weights
+    :param retrain_model: use model retrain
+    :param old_weights_version: previous weights version
+    :param new_weights_version: current weights version
+    """
+    weights_id: str
+    retrain_model: bool
+    old_weights_version: str
+    new_weights_version: str
+
+
+class WeightsSimpleResponse(BaseModel):
+    """
+    :param weights_id: id of weights
+    :param version: current weights version
+    """
+    weights_id: str | None
+    version: str | None
+
+
+class ResultResponse(BaseModel):
+    """
+    :param task_id: id of result for polling
+    :param dataset_id: id of dataset
+    :param time_start: starting unix timestamp
+    :param time_end: ending unix timestamp
+    :param type_of_task: type of task: detection, classification
+    :param action: action of result: sampling or test
+    :param weights: weights of result
+    """
+    task_id: str
+    dataset_id: str | None
+    time_start: float
+    time_end: float | None
+    type_of_task: str
+    action: str
+    weights: WeightsConfigResponse | None
+    result: Any
```

