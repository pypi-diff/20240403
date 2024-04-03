# Comparing `tmp/apollo-orm-2.1.5.tar.gz` & `tmp/apollo-orm-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-orm-2.1.5.tar", last modified: Wed Apr  3 01:16:19 2024, max compression
+gzip compressed data, was "apollo-orm-2.1.6.tar", last modified: Wed Apr  3 20:52:37 2024, max compression
```

## Comparing `apollo-orm-2.1.5.tar` & `apollo-orm-2.1.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.522697 apollo-orm-2.1.5/
--rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.5/LICENSE
--rw-rw-rw-   0        0        0     3273 2024-04-03 01:16:19.521698 apollo-orm-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.492804 apollo-orm-2.1.5/apollo_orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.5/apollo_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.495693 apollo-orm-2.1.5/apollo_orm/domains/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.5/apollo_orm/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.496693 apollo-orm-2.1.5/apollo_orm/domains/models/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.5/apollo_orm/domains/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.497692 apollo-orm-2.1.5/apollo_orm/domains/models/entities/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.498693 apollo-orm-2.1.5/apollo_orm/domains/models/entities/column/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/column/__init__.py
--rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/column/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.499693 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/
--rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.500694 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
--rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.501693 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/result_list/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
--rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.503693 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/result_process/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.504693 apollo-orm-2.1.5/apollo_orm/domains/models/entities/connection_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/connection_config/__init__.py
--rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/connection_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.506693 apollo-orm-2.1.5/apollo_orm/domains/models/entities/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/credentials/__init__.py
--rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/credentials/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.508693 apollo-orm-2.1.5/apollo_orm/domains/models/entities/table_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/table_config/__init__.py
--rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.5/apollo_orm/domains/models/entities/table_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.509698 apollo-orm-2.1.5/apollo_orm/orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.5/apollo_orm/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.511698 apollo-orm-2.1.5/apollo_orm/orm/abstracts/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.5/apollo_orm/orm/abstracts/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.5/apollo_orm/orm/abstracts/icredential.py
--rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.5/apollo_orm/orm/abstracts/idatabase.py
--rw-rw-rw-   0        0        0    21090 2024-04-03 01:14:52.000000 apollo-orm-2.1.5/apollo_orm/orm/core.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.514698 apollo-orm-2.1.5/apollo_orm/orm/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.5/apollo_orm/orm/credentials/__init__.py
--rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.5/apollo_orm/orm/credentials/credential_service.py
--rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.5/apollo_orm/orm/credentials/json_credential_service.py
--rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.5/apollo_orm/orm/credentials/secrets_manager_credential_service.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.515698 apollo-orm-2.1.5/apollo_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.5/apollo_orm/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.516697 apollo-orm-2.1.5/apollo_orm/utils/exceptions/
--rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.5/apollo_orm/utils/exceptions/CommonBaseException.py
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.5/apollo_orm/utils/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.518699 apollo-orm-2.1.5/apollo_orm/utils/logger/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.5/apollo_orm/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.5/apollo_orm/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.520697 apollo-orm-2.1.5/apollo_orm.egg-info/
--rw-rw-rw-   0        0        0     3273 2024-04-03 01:16:19.000000 apollo-orm-2.1.5/apollo_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2024-04-03 01:16:19.000000 apollo-orm-2.1.5/apollo_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 01:16:19.000000 apollo-orm-2.1.5/apollo_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 01:16:19.000000 apollo-orm-2.1.5/apollo_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-04-03 01:16:05.000000 apollo-orm-2.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 01:16:19.522697 apollo-orm-2.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 01:16:19.519698 apollo-orm-2.1.5/tests/
--rw-rw-rw-   0        0        0    13742 2024-04-03 01:14:10.000000 apollo-orm-2.1.5/tests/test_full_process.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.051840 apollo-orm-2.1.6/
+-rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3273 2024-04-03 20:52:37.050838 apollo-orm-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.014682 apollo-orm-2.1.6/apollo_orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.6/apollo_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.018833 apollo-orm-2.1.6/apollo_orm/domains/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.6/apollo_orm/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.019832 apollo-orm-2.1.6/apollo_orm/domains/models/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.6/apollo_orm/domains/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.019832 apollo-orm-2.1.6/apollo_orm/domains/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.021965 apollo-orm-2.1.6/apollo_orm/domains/models/entities/column/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/column/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/column/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.023085 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/
+-rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.024111 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.026149 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_list/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
+-rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.028602 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_process/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.029608 apollo-orm-2.1.6/apollo_orm/domains/models/entities/connection_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/connection_config/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/connection_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.031609 apollo-orm-2.1.6/apollo_orm/domains/models/entities/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/credentials/__init__.py
+-rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/credentials/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.033973 apollo-orm-2.1.6/apollo_orm/domains/models/entities/table_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/table_config/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.6/apollo_orm/domains/models/entities/table_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.035006 apollo-orm-2.1.6/apollo_orm/orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.6/apollo_orm/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.038012 apollo-orm-2.1.6/apollo_orm/orm/abstracts/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.6/apollo_orm/orm/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.6/apollo_orm/orm/abstracts/icredential.py
+-rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.6/apollo_orm/orm/abstracts/idatabase.py
+-rw-rw-rw-   0        0        0    22239 2024-04-03 20:52:18.000000 apollo-orm-2.1.6/apollo_orm/orm/core.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.042335 apollo-orm-2.1.6/apollo_orm/orm/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.6/apollo_orm/orm/credentials/__init__.py
+-rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.6/apollo_orm/orm/credentials/credential_service.py
+-rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.6/apollo_orm/orm/credentials/json_credential_service.py
+-rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.6/apollo_orm/orm/credentials/secrets_manager_credential_service.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.043733 apollo-orm-2.1.6/apollo_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.6/apollo_orm/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.045754 apollo-orm-2.1.6/apollo_orm/utils/exceptions/
+-rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.6/apollo_orm/utils/exceptions/CommonBaseException.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.6/apollo_orm/utils/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.047837 apollo-orm-2.1.6/apollo_orm/utils/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.6/apollo_orm/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.6/apollo_orm/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.049838 apollo-orm-2.1.6/apollo_orm.egg-info/
+-rw-rw-rw-   0        0        0     3273 2024-04-03 20:52:36.000000 apollo-orm-2.1.6/apollo_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2024-04-03 20:52:36.000000 apollo-orm-2.1.6/apollo_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 20:52:36.000000 apollo-orm-2.1.6/apollo_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 20:52:36.000000 apollo-orm-2.1.6/apollo_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-03 20:52:08.000000 apollo-orm-2.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 20:52:37.051840 apollo-orm-2.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 20:52:37.048839 apollo-orm-2.1.6/tests/
+-rw-rw-rw-   0        0        0    13742 2024-04-03 01:14:10.000000 apollo-orm-2.1.6/tests/test_full_process.py
```

### Comparing `apollo-orm-2.1.5/LICENSE` & `apollo-orm-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/PKG-INFO` & `apollo-orm-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.5
+Version: 2.1.6
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.5/README.md` & `apollo-orm-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py` & `apollo-orm-2.1.6/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/domains/models/entities/connection_config/entity.py` & `apollo-orm-2.1.6/apollo_orm/domains/models/entities/connection_config/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/domains/models/entities/credentials/entity.py` & `apollo-orm-2.1.6/apollo_orm/domains/models/entities/credentials/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/orm/abstracts/idatabase.py` & `apollo-orm-2.1.6/apollo_orm/orm/abstracts/idatabase.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/orm/core.py` & `apollo-orm-2.1.6/apollo_orm/orm/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import hashlib
 import json
 import re
-import threading
 import uuid
-from asyncio import Semaphore
 from datetime import datetime, date
 
 from typing import Dict, Optional, List, Any
 
 from cassandra.auth import PlainTextAuthProvider
 from cassandra.cluster import Cluster, Session, NoHostAvailable, ExecutionProfile, ResultSet, ResponseFuture, \
     EXEC_PROFILE_DEFAULT
 from cassandra.concurrent import execute_concurrent_with_args
 from cassandra.connection import ConnectionException
-from cassandra.policies import RoundRobinPolicy, DCAwareRoundRobinPolicy, TokenAwarePolicy, HostDistance, RetryPolicy, \
-    ExponentialReconnectionPolicy
+from cassandra.policies import RoundRobinPolicy, DCAwareRoundRobinPolicy, TokenAwarePolicy, RetryPolicy, \
+    ExponentialReconnectionPolicy, ConstantSpeculativeExecutionPolicy
 from cassandra.query import PreparedStatement
 from apollo_orm.domains.models.entities.column.entity import Column
 from apollo_orm.domains.models.entities.concurrent.pre_processed_insert.entity import PreProcessedInsertData
 from apollo_orm.domains.models.entities.concurrent.result_list.entity import ResultList
 from apollo_orm.domains.models.entities.concurrent.result_process.entity import ResultProcess
 from apollo_orm.domains.models.entities.connection_config.entity import ConnectionConfig
 from apollo_orm.domains.models.entities.table_config.entity import TableConfig
@@ -104,30 +102,62 @@
                           _parse_to_cassandra_type(hashed_columns[column.hash_id], column.type))
 
 
 def _filter_kind(columns: List[Column], kind: str) -> list[Column]:
     return [column for column in columns if column.kind == kind]
 
 
+class ORMRetryPolicy(RetryPolicy):
+    def __init__(self, max_retry_attempts: int = 5):
+        self.MAX_RETRY_ATTEMPTS = max_retry_attempts
+
+    def on_read_timeout(self, query, consistency, required_responses, received_responses, data_retrieved, retry_num):
+        if retry_num < self.MAX_RETRY_ATTEMPTS and received_responses >= required_responses and not data_retrieved:
+            return self.RETRY, consistency
+        return self.RETHROW, None
+
+    def on_write_timeout(self, query, consistency, write_type, required_responses, received_responses, retry_num):
+        if retry_num < self.MAX_RETRY_ATTEMPTS and (
+                (write_type == "BATCH_LOG" and received_responses >= required_responses) or (
+                write_type != "BATCH_LOG" and received_responses > 0)):
+            return self.RETRY
+        return self.RETHROW
+
+    def on_unavailable(self, query, consistency, required_replicas, alive_replicas, retry_num):
+        if retry_num < self.MAX_RETRY_ATTEMPTS and alive_replicas < required_replicas:
+            return self.RETRY
+        return self.RETHROW
+
+    def on_request_error(self, query, consistency, error, retry_num):
+        if retry_num < self.MAX_RETRY_ATTEMPTS:
+            return self.RETRY
+        return self.RETHROW
+
+
 class ORMInstance(IDatabaseService):
     log = Logger("ORMInstance")
 
     def __init__(self,
                  connection_config: ConnectionConfig,
                  attempts: int = 5,
-                 client_timeout: int = 20.0
+                 client_timeout: int = 20.0,
+                 consistency_level: Optional[str] = None
                  ):
         self._in_process = []
-        self._semaphore: Optional[Semaphore] = None
+        self._speculative_execution_policy = ConstantSpeculativeExecutionPolicy(
+            delay=0.5, max_attempts=attempts)
         self._policy = DCAwareRoundRobinPolicy(
             connection_config.credential.datacenter) if connection_config.credential.datacenter else RoundRobinPolicy()
         self._load_balancing_policy = TokenAwarePolicy(self._policy)
         self._execution_profile = ExecutionProfile(load_balancing_policy=self._load_balancing_policy,
                                                    request_timeout=client_timeout,
-                                                   retry_policy=RetryPolicy())
+                                                   retry_policy=ORMRetryPolicy(attempts),
+                                                   consistency_level=consistency_level,
+                                                   speculative_execution_policy=self._speculative_execution_policy
+                                                   )
         self._connection_config = connection_config
         self._attempts = attempts
         self._table_config: Optional[List[TableConfig]] = None
         self._prepared_statements: Dict[str, PreparedStatement] = {}
         self.cluster: Optional[Cluster] = None
         self.session: Optional[Session] = None
         self.connect()
@@ -149,15 +179,14 @@
                     auth_provider=auth_provider,
                     protocol_version=protocol_version,
                     execution_profiles={EXEC_PROFILE_DEFAULT: self._execution_profile},
                     reconnection_policy=ExponentialReconnectionPolicy(base_delay=1.0, max_delay=60.0,
                                                                       max_attempts=self._attempts)
                 )
                 self.session = self.cluster.connect()
-                self._semaphore = threading.Semaphore(self._get_number_of_requests())
                 self._scan_tables()
                 self.log.info(f"Connected to {self._connection_config.credential.hosts}")
                 return
             except ConnectionException as e:
                 error_message = str(e) if str(e) else "Unknown error"
         raise ApolloORMException(f"Failed to connect after {self._attempts} attempts - {error_message}")
 
@@ -316,19 +345,15 @@
             -> Optional[ResponseFuture]:
         values = [filtered_columns[column.hash_id].value for column in
                   sorted(filtered_columns.values(), key=lambda x: x.name)]
         if exec_async:
             return self._execute_async_query(prepared_statement, values)
         self._execute_query(prepared_statement, values)
 
-    def release_semaphore(self):
-        self._semaphore.release()
-
     def _execute_async_query(self, statement: PreparedStatement, values: List[Any]) -> ResponseFuture:
-        self._semaphore.acquire()
         statement.is_idempotent = True
         self.log.info(f"Executing query: {statement.query_string} with values: {values}")
         try:
             return self.session.execute_async(statement, values)
         except (NoHostAvailable, ConnectionException) as e:
             self.log.error(f"Connection error: {e}. Reconnecting...")
             self.reconnect()
@@ -383,12 +408,7 @@
         self._prepared_statements[hashed_name] = self.session.prepare(statement)
 
     def _prepare_delete(self, hashed_name: str, columns: List[Column], keyspace: str, table_name: str,
                         dict_columns: Optional[Dict[str, Column]] = None) -> None:
         values = _generate_pre_statement_labels(columns)
         statement = f"delete from {keyspace}.{table_name} where {' and '.join(values.values())}"
         self._prepared_statements[hashed_name] = self.session.prepare(statement)
-
-    def _get_number_of_requests(self) -> int:
-        request_per_connection = self.cluster.get_max_requests_per_connection(host_distance=HostDistance.LOCAL)
-        max_connections = self.cluster.get_core_connections_per_host(host_distance=HostDistance.LOCAL)
-        return request_per_connection * max_connections * 0.95
```

### Comparing `apollo-orm-2.1.5/apollo_orm/orm/credentials/credential_service.py` & `apollo-orm-2.1.6/apollo_orm/orm/credentials/credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/orm/credentials/json_credential_service.py` & `apollo-orm-2.1.6/apollo_orm/orm/credentials/json_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/orm/credentials/secrets_manager_credential_service.py` & `apollo-orm-2.1.6/apollo_orm/orm/credentials/secrets_manager_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/utils/exceptions/CommonBaseException.py` & `apollo-orm-2.1.6/apollo_orm/utils/exceptions/CommonBaseException.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm/utils/logger/logger.py` & `apollo-orm-2.1.6/apollo_orm/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/apollo_orm.egg-info/PKG-INFO` & `apollo-orm-2.1.6/apollo_orm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.5
+Version: 2.1.6
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.5/apollo_orm.egg-info/SOURCES.txt` & `apollo-orm-2.1.6/apollo_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.5/pyproject.toml` & `apollo-orm-2.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apollo-orm"
-version = "2.1.5"
+version = "2.1.6"
 authors = [
     { name="Danilo Rodrigues", email="daniloarodrigues@outlook.com" },
 ]
 description = "ORM Cassandra/Scylla Stable Version (2.x.x)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `apollo-orm-2.1.5/tests/test_full_process.py` & `apollo-orm-2.1.6/tests/test_full_process.py`

 * *Files identical despite different names*

