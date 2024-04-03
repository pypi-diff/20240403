# Comparing `tmp/apollo-orm-2.1.6.tar.gz` & `tmp/apollo-orm-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-orm-2.1.6.tar", last modified: Wed Apr  3 20:52:37 2024, max compression
+gzip compressed data, was "apollo-orm-2.1.7.tar", last modified: Wed Apr  3 21:42:55 2024, max compression
```

## Comparing `apollo-orm-2.1.6.tar` & `apollo-orm-2.1.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.051840 apollo-orm-2.1.6/
--rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.6/LICENSE
--rw-rw-rw-   0        0        0     3273 2024-04-03 20:52:37.050838 apollo-orm-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.014682 apollo-orm-2.1.6/apollo_orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.6/apollo_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.018833 apollo-orm-2.1.6/apollo_orm/domains/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.6/apollo_orm/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.019832 apollo-orm-2.1.6/apollo_orm/domains/models/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.6/apollo_orm/domains/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.019832 apollo-orm-2.1.6/apollo_orm/domains/models/entities/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.021965 apollo-orm-2.1.6/apollo_orm/domains/models/entities/column/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/column/__init__.py
--rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/column/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.023085 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/
--rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.024111 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
--rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.026149 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_list/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
--rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.028602 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_process/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.029608 apollo-orm-2.1.6/apollo_orm/domains/models/entities/connection_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/connection_config/__init__.py
--rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/connection_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.031609 apollo-orm-2.1.6/apollo_orm/domains/models/entities/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/credentials/__init__.py
--rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/credentials/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.033973 apollo-orm-2.1.6/apollo_orm/domains/models/entities/table_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/table_config/__init__.py
--rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/table_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.035006 apollo-orm-2.1.6/apollo_orm/orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.6/apollo_orm/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.038012 apollo-orm-2.1.6/apollo_orm/orm/abstracts/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.6/apollo_orm/orm/abstracts/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.6/apollo_orm/orm/abstracts/icredential.py
--rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.6/apollo_orm/orm/abstracts/idatabase.py
--rw-rw-rw-   0        0        0    22239 2024-04-03 20:52:18.000000 apollo-orm-2.1.6/apollo_orm/orm/core.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.042335 apollo-orm-2.1.6/apollo_orm/orm/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.6/apollo_orm/orm/credentials/__init__.py
--rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.6/apollo_orm/orm/credentials/credential_service.py
--rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.6/apollo_orm/orm/credentials/json_credential_service.py
--rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.6/apollo_orm/orm/credentials/secrets_manager_credential_service.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.043733 apollo-orm-2.1.6/apollo_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.6/apollo_orm/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.045754 apollo-orm-2.1.6/apollo_orm/utils/exceptions/
--rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.6/apollo_orm/utils/exceptions/CommonBaseException.py
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.6/apollo_orm/utils/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.047837 apollo-orm-2.1.6/apollo_orm/utils/logger/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.6/apollo_orm/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.6/apollo_orm/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.049838 apollo-orm-2.1.6/apollo_orm.egg-info/
--rw-rw-rw-   0        0        0     3273 2024-04-03 20:52:36.000000 apollo-orm-2.1.6/apollo_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2024-04-03 20:52:36.000000 apollo-orm-2.1.6/apollo_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 20:52:36.000000 apollo-orm-2.1.6/apollo_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 20:52:36.000000 apollo-orm-2.1.6/apollo_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-04-03 20:52:08.000000 apollo-orm-2.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 20:52:37.051840 apollo-orm-2.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.048839 apollo-orm-2.1.6/tests/
--rw-rw-rw-   0        0        0    13742 2024-04-03 01:14:10.000000 apollo-orm-2.1.6/tests/test_full_process.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.125789 apollo-orm-2.1.7/
+-rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3273 2024-04-03 21:42:55.125789 apollo-orm-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.095649 apollo-orm-2.1.7/apollo_orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.7/apollo_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.098646 apollo-orm-2.1.7/apollo_orm/domains/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.7/apollo_orm/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.099649 apollo-orm-2.1.7/apollo_orm/domains/models/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.7/apollo_orm/domains/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.100645 apollo-orm-2.1.7/apollo_orm/domains/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.101647 apollo-orm-2.1.7/apollo_orm/domains/models/entities/column/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/column/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/column/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.102650 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/
+-rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.104647 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.105645 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/result_list/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
+-rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.107651 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/result_process/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.109645 apollo-orm-2.1.7/apollo_orm/domains/models/entities/connection_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/connection_config/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/connection_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.110650 apollo-orm-2.1.7/apollo_orm/domains/models/entities/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/credentials/__init__.py
+-rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/credentials/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.112650 apollo-orm-2.1.7/apollo_orm/domains/models/entities/table_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/table_config/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.7/apollo_orm/domains/models/entities/table_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.113657 apollo-orm-2.1.7/apollo_orm/orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.7/apollo_orm/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.115654 apollo-orm-2.1.7/apollo_orm/orm/abstracts/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.7/apollo_orm/orm/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.7/apollo_orm/orm/abstracts/icredential.py
+-rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.7/apollo_orm/orm/abstracts/idatabase.py
+-rw-rw-rw-   0        0        0    22925 2024-04-03 21:41:46.000000 apollo-orm-2.1.7/apollo_orm/orm/core.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.118651 apollo-orm-2.1.7/apollo_orm/orm/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.7/apollo_orm/orm/credentials/__init__.py
+-rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.7/apollo_orm/orm/credentials/credential_service.py
+-rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.7/apollo_orm/orm/credentials/json_credential_service.py
+-rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.7/apollo_orm/orm/credentials/secrets_manager_credential_service.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.120114 apollo-orm-2.1.7/apollo_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.7/apollo_orm/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.122150 apollo-orm-2.1.7/apollo_orm/utils/exceptions/
+-rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.7/apollo_orm/utils/exceptions/CommonBaseException.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.7/apollo_orm/utils/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.123276 apollo-orm-2.1.7/apollo_orm/utils/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.7/apollo_orm/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.7/apollo_orm/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.124791 apollo-orm-2.1.7/apollo_orm.egg-info/
+-rw-rw-rw-   0        0        0     3273 2024-04-03 21:42:55.000000 apollo-orm-2.1.7/apollo_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2024-04-03 21:42:55.000000 apollo-orm-2.1.7/apollo_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 21:42:55.000000 apollo-orm-2.1.7/apollo_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 21:42:55.000000 apollo-orm-2.1.7/apollo_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-03 21:42:47.000000 apollo-orm-2.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 21:42:55.125789 apollo-orm-2.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 21:42:55.123782 apollo-orm-2.1.7/tests/
+-rw-rw-rw-   0        0        0    13794 2024-04-03 21:42:11.000000 apollo-orm-2.1.7/tests/test_full_process.py
```

### Comparing `apollo-orm-2.1.6/LICENSE` & `apollo-orm-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/PKG-INFO` & `apollo-orm-2.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.6
+Version: 2.1.7
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.6/README.md` & `apollo-orm-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py` & `apollo-orm-2.1.7/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/domains/models/entities/connection_config/entity.py` & `apollo-orm-2.1.7/apollo_orm/domains/models/entities/connection_config/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/domains/models/entities/credentials/entity.py` & `apollo-orm-2.1.7/apollo_orm/domains/models/entities/credentials/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/orm/abstracts/idatabase.py` & `apollo-orm-2.1.7/apollo_orm/orm/abstracts/idatabase.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/orm/core.py` & `apollo-orm-2.1.7/apollo_orm/orm/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import re
 import uuid
 from datetime import datetime, date
 
 from typing import Dict, Optional, List, Any
 
+from cassandra import ConsistencyLevel
 from cassandra.auth import PlainTextAuthProvider
 from cassandra.cluster import Cluster, Session, NoHostAvailable, ExecutionProfile, ResultSet, ResponseFuture, \
     EXEC_PROFILE_DEFAULT
 from cassandra.concurrent import execute_concurrent_with_args
 from cassandra.connection import ConnectionException
 from cassandra.policies import RoundRobinPolicy, DCAwareRoundRobinPolicy, TokenAwarePolicy, RetryPolicy, \
     ExponentialReconnectionPolicy, ConstantSpeculativeExecutionPolicy
@@ -129,37 +130,53 @@
 
     def on_request_error(self, query, consistency, error, retry_num):
         if retry_num < self.MAX_RETRY_ATTEMPTS:
             return self.RETRY
         return self.RETHROW
 
 
+def get_consistency_level(consistency: str) -> int:
+    ConsistencyLevel.name_to_value = {
+        'ANY': ConsistencyLevel.ANY,
+        'ONE': ConsistencyLevel.ONE,
+        'TWO': ConsistencyLevel.TWO,
+        'THREE': ConsistencyLevel.THREE,
+        'QUORUM': ConsistencyLevel.QUORUM,
+        'ALL': ConsistencyLevel.ALL,
+        'LOCAL_QUORUM': ConsistencyLevel.LOCAL_QUORUM,
+        'EACH_QUORUM': ConsistencyLevel.EACH_QUORUM,
+        'SERIAL': ConsistencyLevel.SERIAL,
+        'LOCAL_SERIAL': ConsistencyLevel.LOCAL_SERIAL,
+        'LOCAL_ONE': ConsistencyLevel.LOCAL_ONE
+    }
+    return ConsistencyLevel.name_to_value[consistency]
+
+
 class ORMInstance(IDatabaseService):
     log = Logger("ORMInstance")
 
     def __init__(self,
                  connection_config: ConnectionConfig,
                  attempts: int = 5,
-                 client_timeout: int = 20.0,
-                 consistency_level: Optional[str] = None
+                 consistency_level: str = "LOCAL_ONE",
+                 client_timeout: int = 20.0
                  ):
-        self._in_process = []
+        self._attempts = attempts
         self._speculative_execution_policy = ConstantSpeculativeExecutionPolicy(
-            delay=0.5, max_attempts=attempts)
+            delay=0.1, max_attempts=attempts)
         self._policy = DCAwareRoundRobinPolicy(
             connection_config.credential.datacenter) if connection_config.credential.datacenter else RoundRobinPolicy()
         self._load_balancing_policy = TokenAwarePolicy(self._policy)
         self._execution_profile = ExecutionProfile(load_balancing_policy=self._load_balancing_policy,
                                                    request_timeout=client_timeout,
+                                                   consistency_level=get_consistency_level(consistency_level),
                                                    retry_policy=ORMRetryPolicy(attempts),
-                                                   consistency_level=consistency_level,
                                                    speculative_execution_policy=self._speculative_execution_policy
                                                    )
         self._connection_config = connection_config
-        self._attempts = attempts
         self._table_config: Optional[List[TableConfig]] = None
         self._prepared_statements: Dict[str, PreparedStatement] = {}
         self.cluster: Optional[Cluster] = None
         self.session: Optional[Session] = None
         self.connect()
 
     def connect(self,
```

### Comparing `apollo-orm-2.1.6/apollo_orm/orm/credentials/credential_service.py` & `apollo-orm-2.1.7/apollo_orm/orm/credentials/credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/orm/credentials/json_credential_service.py` & `apollo-orm-2.1.7/apollo_orm/orm/credentials/json_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/orm/credentials/secrets_manager_credential_service.py` & `apollo-orm-2.1.7/apollo_orm/orm/credentials/secrets_manager_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/utils/exceptions/CommonBaseException.py` & `apollo-orm-2.1.7/apollo_orm/utils/exceptions/CommonBaseException.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm/utils/logger/logger.py` & `apollo-orm-2.1.7/apollo_orm/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/apollo_orm.egg-info/PKG-INFO` & `apollo-orm-2.1.7/apollo_orm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.6
+Version: 2.1.7
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.6/apollo_orm.egg-info/SOURCES.txt` & `apollo-orm-2.1.7/apollo_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.6/pyproject.toml` & `apollo-orm-2.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apollo-orm"
-version = "2.1.6"
+version = "2.1.7"
 authors = [
     { name="Danilo Rodrigues", email="daniloarodrigues@outlook.com" },
 ]
 description = "ORM Cassandra/Scylla Stable Version (2.x.x)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `apollo-orm-2.1.6/tests/test_full_process.py` & `apollo-orm-2.1.7/tests/test_full_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         "group_leader_name": "KELBIA DA SILVA MANZAN",
     }))
     json_credentials = json.loads(json.dumps(credential))
     credentials = Credentials(**json_credentials)
     tables = ["reward_summary_groups_v2",
               "payment_sap"]
     connection_config = ConnectionConfig(credentials, tables)
-    connection = ORMInstance(connection_config)
+    connection = ORMInstance(connection_config=connection_config, consistency_level="LOCAL_QUORUM")
 
     for table in tables:
         result = connection.insert(json_data, table, True)
         result.add_callbacks(callback=lambda x: print(f"Inserted {json_data} into {table}"),
                              errback=lambda x: print(f"Failed to insert {json_data} into {table}"))
         sleep(1)
         select = connection.select(json_data, table)
```

