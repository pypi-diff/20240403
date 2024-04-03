# Comparing `tmp/apollo-orm-2.1.3.tar.gz` & `tmp/apollo-orm-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-orm-2.1.3.tar", last modified: Tue Apr  2 21:12:45 2024, max compression
+gzip compressed data, was "apollo-orm-2.1.4.tar", last modified: Wed Apr  3 00:17:31 2024, max compression
```

## Comparing `apollo-orm-2.1.3.tar` & `apollo-orm-2.1.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.044436 apollo-orm-2.1.3/
--rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.3/LICENSE
--rw-rw-rw-   0        0        0     3273 2024-04-02 21:12:45.043362 apollo-orm-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.014722 apollo-orm-2.1.3/apollo_orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.3/apollo_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.017923 apollo-orm-2.1.3/apollo_orm/domains/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.3/apollo_orm/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.018924 apollo-orm-2.1.3/apollo_orm/domains/models/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.3/apollo_orm/domains/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.020034 apollo-orm-2.1.3/apollo_orm/domains/models/entities/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.021101 apollo-orm-2.1.3/apollo_orm/domains/models/entities/column/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/column/__init__.py
--rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/column/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.022172 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/
--rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.023175 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
--rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.024224 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/result_list/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
--rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.026314 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/result_process/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.027446 apollo-orm-2.1.3/apollo_orm/domains/models/entities/connection_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/connection_config/__init__.py
--rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/connection_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.028498 apollo-orm-2.1.3/apollo_orm/domains/models/entities/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/credentials/__init__.py
--rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/credentials/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.030553 apollo-orm-2.1.3/apollo_orm/domains/models/entities/table_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/table_config/__init__.py
--rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.3/apollo_orm/domains/models/entities/table_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.031664 apollo-orm-2.1.3/apollo_orm/orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.3/apollo_orm/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.033786 apollo-orm-2.1.3/apollo_orm/orm/abstracts/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.3/apollo_orm/orm/abstracts/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.3/apollo_orm/orm/abstracts/icredential.py
--rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.3/apollo_orm/orm/abstracts/idatabase.py
--rw-rw-rw-   0        0        0    21347 2024-04-02 21:12:13.000000 apollo-orm-2.1.3/apollo_orm/orm/core.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.036959 apollo-orm-2.1.3/apollo_orm/orm/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.3/apollo_orm/orm/credentials/__init__.py
--rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.3/apollo_orm/orm/credentials/credential_service.py
--rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.3/apollo_orm/orm/credentials/json_credential_service.py
--rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.3/apollo_orm/orm/credentials/secrets_manager_credential_service.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.038031 apollo-orm-2.1.3/apollo_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.3/apollo_orm/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.039092 apollo-orm-2.1.3/apollo_orm/utils/exceptions/
--rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.3/apollo_orm/utils/exceptions/CommonBaseException.py
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.3/apollo_orm/utils/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.041138 apollo-orm-2.1.3/apollo_orm/utils/logger/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.3/apollo_orm/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.3/apollo_orm/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.043362 apollo-orm-2.1.3/apollo_orm.egg-info/
--rw-rw-rw-   0        0        0     3273 2024-04-02 21:12:44.000000 apollo-orm-2.1.3/apollo_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2024-04-02 21:12:45.000000 apollo-orm-2.1.3/apollo_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 21:12:44.000000 apollo-orm-2.1.3/apollo_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 21:12:44.000000 apollo-orm-2.1.3/apollo_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-04-02 21:12:04.000000 apollo-orm-2.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 21:12:45.044436 apollo-orm-2.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 21:12:45.041138 apollo-orm-2.1.3/tests/
--rw-rw-rw-   0        0        0    13745 2024-03-27 21:46:59.000000 apollo-orm-2.1.3/tests/test_full_process.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.579534 apollo-orm-2.1.4/
+-rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3273 2024-04-03 00:17:31.578509 apollo-orm-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.551128 apollo-orm-2.1.4/apollo_orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.4/apollo_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.554213 apollo-orm-2.1.4/apollo_orm/domains/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.4/apollo_orm/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.554213 apollo-orm-2.1.4/apollo_orm/domains/models/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.4/apollo_orm/domains/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.555764 apollo-orm-2.1.4/apollo_orm/domains/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.556795 apollo-orm-2.1.4/apollo_orm/domains/models/entities/column/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/column/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/column/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.557826 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/
+-rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.558853 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.560926 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/result_list/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
+-rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.561955 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/result_process/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.562981 apollo-orm-2.1.4/apollo_orm/domains/models/entities/connection_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/connection_config/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/connection_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.565040 apollo-orm-2.1.4/apollo_orm/domains/models/entities/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/credentials/__init__.py
+-rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/credentials/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.566067 apollo-orm-2.1.4/apollo_orm/domains/models/entities/table_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/table_config/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.4/apollo_orm/domains/models/entities/table_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.568156 apollo-orm-2.1.4/apollo_orm/orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.4/apollo_orm/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.570220 apollo-orm-2.1.4/apollo_orm/orm/abstracts/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.4/apollo_orm/orm/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.4/apollo_orm/orm/abstracts/icredential.py
+-rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.4/apollo_orm/orm/abstracts/idatabase.py
+-rw-rw-rw-   0        0        0    21103 2024-04-03 00:17:19.000000 apollo-orm-2.1.4/apollo_orm/orm/core.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.572343 apollo-orm-2.1.4/apollo_orm/orm/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.4/apollo_orm/orm/credentials/__init__.py
+-rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.4/apollo_orm/orm/credentials/credential_service.py
+-rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.4/apollo_orm/orm/credentials/json_credential_service.py
+-rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.4/apollo_orm/orm/credentials/secrets_manager_credential_service.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.573344 apollo-orm-2.1.4/apollo_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.4/apollo_orm/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.574371 apollo-orm-2.1.4/apollo_orm/utils/exceptions/
+-rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.4/apollo_orm/utils/exceptions/CommonBaseException.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.4/apollo_orm/utils/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.576450 apollo-orm-2.1.4/apollo_orm/utils/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.4/apollo_orm/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.4/apollo_orm/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.577481 apollo-orm-2.1.4/apollo_orm.egg-info/
+-rw-rw-rw-   0        0        0     3273 2024-04-03 00:17:31.000000 apollo-orm-2.1.4/apollo_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2024-04-03 00:17:31.000000 apollo-orm-2.1.4/apollo_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 00:17:31.000000 apollo-orm-2.1.4/apollo_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 00:17:31.000000 apollo-orm-2.1.4/apollo_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-03 00:17:08.000000 apollo-orm-2.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 00:17:31.579534 apollo-orm-2.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 00:17:31.576450 apollo-orm-2.1.4/tests/
+-rw-rw-rw-   0        0        0    13594 2024-04-02 21:17:43.000000 apollo-orm-2.1.4/tests/test_full_process.py
```

### Comparing `apollo-orm-2.1.3/LICENSE` & `apollo-orm-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/PKG-INFO` & `apollo-orm-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.3
+Version: 2.1.4
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.3/README.md` & `apollo-orm-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py` & `apollo-orm-2.1.4/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/domains/models/entities/connection_config/entity.py` & `apollo-orm-2.1.4/apollo_orm/domains/models/entities/connection_config/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/domains/models/entities/credentials/entity.py` & `apollo-orm-2.1.4/apollo_orm/domains/models/entities/credentials/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/orm/abstracts/idatabase.py` & `apollo-orm-2.1.4/apollo_orm/orm/abstracts/idatabase.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/orm/core.py` & `apollo-orm-2.1.4/apollo_orm/orm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from cassandra.auth import PlainTextAuthProvider
 from cassandra.cluster import Cluster, Session, NoHostAvailable, ExecutionProfile, ResultSet, ResponseFuture, \
     EXEC_PROFILE_DEFAULT
 from cassandra.concurrent import execute_concurrent_with_args
 from cassandra.connection import ConnectionException
 from cassandra.policies import RoundRobinPolicy, DCAwareRoundRobinPolicy, TokenAwarePolicy, HostDistance, RetryPolicy, \
-    ExponentialReconnectionPolicy, ConstantSpeculativeExecutionPolicy
+    ExponentialReconnectionPolicy
 from cassandra.query import PreparedStatement
 from apollo_orm.domains.models.entities.column.entity import Column
 from apollo_orm.domains.models.entities.concurrent.pre_processed_insert.entity import PreProcessedInsertData
 from apollo_orm.domains.models.entities.concurrent.result_list.entity import ResultList
 from apollo_orm.domains.models.entities.concurrent.result_process.entity import ResultProcess
 from apollo_orm.domains.models.entities.connection_config.entity import ConnectionConfig
 from apollo_orm.domains.models.entities.table_config.entity import TableConfig
@@ -119,17 +119,15 @@
         self._in_process = []
         self._semaphore: Optional[Semaphore] = None
         self._policy = DCAwareRoundRobinPolicy(
             connection_config.credential.datacenter) if connection_config.credential.datacenter else RoundRobinPolicy()
         self._load_balancing_policy = TokenAwarePolicy(self._policy)
         self._execution_profile = ExecutionProfile(load_balancing_policy=self._load_balancing_policy,
                                                    request_timeout=client_timeout,
-                                                   retry_policy=RetryPolicy(),
-                                                   speculative_execution_policy=ConstantSpeculativeExecutionPolicy(
-                                                       delay=0.1, max_attempts=attempts))
+                                                   retry_policy=RetryPolicy())
         self._connection_config = connection_config
         self._attempts = attempts
         self._table_config: Optional[List[TableConfig]] = None
         self._prepared_statements: Dict[str, PreparedStatement] = {}
         self.cluster: Optional[Cluster] = None
         self.session: Optional[Session] = None
         self.connect()
```

### Comparing `apollo-orm-2.1.3/apollo_orm/orm/credentials/credential_service.py` & `apollo-orm-2.1.4/apollo_orm/orm/credentials/credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/orm/credentials/json_credential_service.py` & `apollo-orm-2.1.4/apollo_orm/orm/credentials/json_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/orm/credentials/secrets_manager_credential_service.py` & `apollo-orm-2.1.4/apollo_orm/orm/credentials/secrets_manager_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/utils/exceptions/CommonBaseException.py` & `apollo-orm-2.1.4/apollo_orm/utils/exceptions/CommonBaseException.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm/utils/logger/logger.py` & `apollo-orm-2.1.4/apollo_orm/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/apollo_orm.egg-info/PKG-INFO` & `apollo-orm-2.1.4/apollo_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.3
+Version: 2.1.4
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.3/apollo_orm.egg-info/SOURCES.txt` & `apollo-orm-2.1.4/apollo_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.3/pyproject.toml` & `apollo-orm-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apollo-orm"
-version = "2.1.3"
+version = "2.1.4"
 authors = [
     { name="Danilo Rodrigues", email="daniloarodrigues@outlook.com" },
 ]
 description = "ORM Cassandra/Scylla Stable Version (2.x.x)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `apollo-orm-2.1.3/tests/test_full_process.py` & `apollo-orm-2.1.4/tests/test_full_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,18 @@
         "active_persons_value": 0,
         "parameter_representation": "{ \"_id\" : { \"$oid\" : \"654ebd9a56ed11aa74ccbbaa\" }, \"rewardCode\" : 8, \"version\" : 12, \"country\" : 1, \"businessModel\" : 1, \"structureLevel\" : 2, \"structureCode\" : 6, \"structureName\" : \"CENTRO OESTE\", \"updateUserCode\" : \"NOT_FOUND\", \"updateUserName\" : \"Larissa Nair Oliveira De Souza\", \"cycle\" : 202317, \"customIndexes\" : [], \"bonuses\" : [{ \"active\" : false, \"growthPlanCode\" : 2, \"planName\" : \"Plano Natura - Líder de Negócio\", \"leaderLevelCode\" : 8, \"leaderLevelName\" : \"Líder Prata\", \"_id\" : { \"$oid\" : \"654ebd9a56ed113d2bccbbad\" }, \"rows\" : [] }, { \"active\" : false, \"growthPlanCode\" : 2, \"planName\" : \"Plano Natura - Líder de Negócio\", \"leaderLevelCode\" : 9, \"leaderLevelName\" : \"Líder Ouro\", \"_id\" : { \"$oid\" : \"654ebd9a56ed112472ccbbac\" }, \"rows\" : [] }, { \"active\" : false, \"growthPlanCode\" : 2, \"planName\" : \"Plano Natura - Líder de Negócio\", \"leaderLevelCode\" : 10, \"leaderLevelName\" : \"Líder Diamante\", \"_id\" : { \"$oid\" : \"654ebd9a56ed118073ccbbab\" }, \"rows\" : [] }], \"matrices\" : [{ \"active\" : true, \"growthPlanCode\" : 2, \"planName\" : \"Plano Natura - Líder de Negócio\", \"leaderLevelCode\" : 8, \"leaderLevelName\" : \"Líder Prata\", \"parameterRowType\" : 28, \"parameterColumnType\" : 424, \"_id\" : { \"$oid\" : \"654ebd9a56ed112462ccbbc2\" }, \"columns\" : [{ \"column\" : 1, \"rangeBegin\" : 0, \"rangeEnd\" : 999, \"_id\" : { \"$oid\" : \"654ebd9a56ed113796ccbbc3\" }, \"rows\" : [{ \"row\" : 1, \"rangeBegin\" : 0, \"rangeEnd\" : 89.99, \"value\" : 5.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed112b60ccbbcb\" } }, { \"row\" : 2, \"rangeBegin\" : 90, \"rangeEnd\" : 94.99, \"value\" : 6.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed111124ccbbca\" } }, { \"row\" : 3, \"rangeBegin\" : 95, \"rangeEnd\" : 99.99, \"value\" : 7.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed1171b1ccbbc9\" } }, { \"row\" : 4, \"rangeBegin\" : 100, \"rangeEnd\" : 104.99, \"value\" : 10.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed1126baccbbc8\" } }, { \"row\" : 5, \"rangeBegin\" : 105, \"rangeEnd\" : 109.99, \"value\" : 13.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed11ca0dccbbc7\" } }, { \"row\" : 6, \"rangeBegin\" : 110, \"rangeEnd\" : 114.99, \"value\" : 14.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed119908ccbbc6\" } }, { \"row\" : 7, \"rangeBegin\" : 115, \"rangeEnd\" : 119.99, \"value\" : 16, \"_id\" : { \"$oid\" : \"654ebd9a56ed111b95ccbbc5\" } }, { \"row\" : 8, \"rangeBegin\" : 120, \"rangeEnd\" : 999.99, \"value\" : 17.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed110663ccbbc4\" } }] }] }, { \"active\" : true, \"growthPlanCode\" : 2, \"planName\" : \"Plano Natura - Líder de Negócio\", \"leaderLevelCode\" : 9, \"leaderLevelName\" : \"Líder Ouro\", \"parameterRowType\" : 28, \"parameterColumnType\" : 424, \"_id\" : { \"$oid\" : \"654ebd9a56ed116596ccbbb8\" }, \"columns\" : [{ \"column\" : 1, \"rangeBegin\" : 0, \"rangeEnd\" : 999, \"_id\" : { \"$oid\" : \"654ebd9a56ed114c8fccbbb9\" }, \"rows\" : [{ \"row\" : 1, \"rangeBegin\" : 0, \"rangeEnd\" : 89.99, \"value\" : 6, \"_id\" : { \"$oid\" : \"654ebd9a56ed119feaccbbc1\" } }, { \"row\" : 2, \"rangeBegin\" : 90, \"rangeEnd\" : 94.99, \"value\" : 7, \"_id\" : { \"$oid\" : \"654ebd9a56ed11d321ccbbc0\" } }, { \"row\" : 3, \"rangeBegin\" : 95, \"rangeEnd\" : 99.99, \"value\" : 8, \"_id\" : { \"$oid\" : \"654ebd9a56ed111444ccbbbf\" } }, { \"row\" : 4, \"rangeBegin\" : 100, \"rangeEnd\" : 104.99, \"value\" : 11.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed1171f2ccbbbe\" } }, { \"row\" : 5, \"rangeBegin\" : 105, \"rangeEnd\" : 109.99, \"value\" : 14.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed11960bccbbbd\" } }, { \"row\" : 6, \"rangeBegin\" : 110, \"rangeEnd\" : 114.99, \"value\" : 15.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed11cd3fccbbbc\" } }, { \"row\" : 7, \"rangeBegin\" : 115, \"rangeEnd\" : 119.99, \"value\" : 17.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed117962ccbbbb\" } }, { \"row\" : 8, \"rangeBegin\" : 120, \"rangeEnd\" : 999.99, \"value\" : 19.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed111e53ccbbba\" } }] }] }, { \"active\" : true, \"growthPlanCode\" : 2, \"planName\" : \"Plano Natura - Líder de Negócio\", \"leaderLevelCode\" : 10, \"leaderLevelName\" : \"Líder Diamante\", \"parameterRowType\" : 28, \"parameterColumnType\" : 424, \"_id\" : { \"$oid\" : \"654ebd9a56ed111edbccbbae\" }, \"columns\" : [{ \"column\" : 1, \"rangeBegin\" : 0, \"rangeEnd\" : 999, \"_id\" : { \"$oid\" : \"654ebd9a56ed1137feccbbaf\" }, \"rows\" : [{ \"row\" : 1, \"rangeBegin\" : 0, \"rangeEnd\" : 89.99, \"value\" : 6.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed115da8ccbbb7\" } }, { \"row\" : 2, \"rangeBegin\" : 90, \"rangeEnd\" : 94.99, \"value\" : 7.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed11bba8ccbbb6\" } }, { \"row\" : 3, \"rangeBegin\" : 95, \"rangeEnd\" : 99.99, \"value\" : 8.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed112144ccbbb5\" } }, { \"row\" : 4, \"rangeBegin\" : 100, \"rangeEnd\" : 104.99, \"value\" : 13, \"_id\" : { \"$oid\" : \"654ebd9a56ed11f48eccbbb4\" } }, { \"row\" : 5, \"rangeBegin\" : 105, \"rangeEnd\" : 109.99, \"value\" : 16, \"_id\" : { \"$oid\" : \"654ebd9a56ed115d3accbbb3\" } }, { \"row\" : 6, \"rangeBegin\" : 110, \"rangeEnd\" : 114.99, \"value\" : 17, \"_id\" : { \"$oid\" : \"654ebd9a56ed115a4dccbbb2\" } }, { \"row\" : 7, \"rangeBegin\" : 115, \"rangeEnd\" : 119.99, \"value\" : 19.5, \"_id\" : { \"$oid\" : \"654ebd9a56ed113fabccbbb1\" } }, { \"row\" : 8, \"rangeBegin\" : 120, \"rangeEnd\" : 999.99, \"value\" : 22, \"_id\" : { \"$oid\" : \"654ebd9a56ed1110f7ccbbb0\" } }] }] }], \"updated\" : { \"$date\" : 1699659162297 }, \"__v\" : 0 }",
         "publish_date": "2024-03-27T18:53:58.652Z",
         "process_date": "2024-03-27T18:53:58.652Z",
         "group_leader_code": 158883969,
         "group_leader_name": "KELBIA DA SILVA MANZAN",
     }))
-    # json_credentials = json.loads(os.environ['CREDENTIALS'])
     json_credentials = json.loads(json.dumps(credential))
     credentials = Credentials(**json_credentials)
     tables = ["reward_summary_groups_v2",
-              "payment_sap"]  ## os.environ['TABLES'].replace('"', '').replace('[', '').replace(']', '').split(',')
+              "payment_sap"]
     connection_config = ConnectionConfig(credentials, tables)
     connection = ORMInstance(connection_config)
 
     for table in tables:
         result = connection.insert(json_data, table, True)
         result.add_callbacks(callback=lambda x: print(f"Inserted {json_data} into {table}"),
                              errback=lambda x: print(f"Failed to insert {json_data} into {table}"))
```

