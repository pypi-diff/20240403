# Comparing `tmp/pg_database_utils-0.9.0.tar.gz` & `tmp/pg_database_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_database_utils-0.9.0.tar", max compression
+gzip compressed data, was "pg_database_utils-1.0.0.tar", max compression
```

## Comparing `pg_database_utils-0.9.0.tar` & `pg_database_utils-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1505 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/LICENSE
--rw-r--r--   0        0        0     7462 2023-10-29 02:53:21.450385 pg_database_utils-0.9.0/README.md
--rw-r--r--   0        0        0        0 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/__init__.py
--rw-r--r--   0        0        0    12349 2023-10-29 01:57:23.166669 pg_database_utils-0.9.0/pg_database/conf.py
--rw-r--r--   0        0        0    24406 2023-10-28 20:49:44.334156 pg_database_utils-0.9.0/pg_database/schema.py
--rw-r--r--   0        0        0    23326 2023-10-28 20:49:53.946208 pg_database_utils-0.9.0/pg_database/sql.py
--rw-r--r--   0        0        0        0 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/__init__.py
--rw-r--r--   0        0        0      156 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/custom_databases.json
--rw-r--r--   0        0        0      587 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/custom_databases.py
--rw-r--r--   0        0        0       86 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/invalid_config.json
--rw-r--r--   0        0        0      220 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/invalid_settings.py
--rw-r--r--   0        0        0       39 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/missing_django_db.json
--rw-r--r--   0        0        0      787 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/missing_django_db.py
--rw-r--r--   0        0        0        0 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/not.json
--rw-r--r--   0        0        0       35 2020-09-18 17:58:19.000000 pg_database_utils-0.9.0/pg_database/tests/not_settings.py
--rw-r--r--   0        0        0      928 2023-10-29 02:49:06.041801 pg_database_utils-0.9.0/pg_database/tests/settings.py
--rw-r--r--   0        0        0      287 2023-10-29 02:53:21.450643 pg_database_utils-0.9.0/pg_database/tests/test_config.json
--rw-r--r--   0        0        0    87523 2023-10-29 02:53:21.451190 pg_database_utils-0.9.0/pg_database/tests/tests.py
--rw-r--r--   0        0        0     3933 2021-01-24 18:50:28.220993 pg_database_utils-0.9.0/pg_database/types.py
--rw-r--r--   0        0        0     4601 2021-01-24 18:50:28.221321 pg_database_utils-0.9.0/pg_database/validation.py
--rw-r--r--   0        0        0      839 2023-10-29 02:55:17.067387 pg_database_utils-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8391 1970-01-01 00:00:00.000000 pg_database_utils-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7462 2023-10-29 02:53:21.450385 pg_database_utils-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/__init__.py
+-rw-r--r--   0        0        0    12449 2024-04-03 18:22:30.988616 pg_database_utils-1.0.0/pg_database/conf.py
+-rw-r--r--   0        0        0    24406 2023-10-28 20:49:44.334156 pg_database_utils-1.0.0/pg_database/schema.py
+-rw-r--r--   0        0        0    23326 2023-10-28 20:49:53.946208 pg_database_utils-1.0.0/pg_database/sql.py
+-rw-r--r--   0        0        0        0 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/__init__.py
+-rw-r--r--   0        0        0      156 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/custom_databases.json
+-rw-r--r--   0        0        0      587 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/custom_databases.py
+-rw-r--r--   0        0        0       86 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/invalid_config.json
+-rw-r--r--   0        0        0      220 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/invalid_settings.py
+-rw-r--r--   0        0        0       39 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/missing_django_db.json
+-rw-r--r--   0        0        0      787 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/missing_django_db.py
+-rw-r--r--   0        0        0        0 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/not.json
+-rw-r--r--   0        0        0       35 2020-09-18 17:58:19.000000 pg_database_utils-1.0.0/pg_database/tests/not_settings.py
+-rw-r--r--   0        0        0      928 2023-10-29 02:49:06.041801 pg_database_utils-1.0.0/pg_database/tests/settings.py
+-rw-r--r--   0        0        0      287 2023-10-29 02:53:21.450643 pg_database_utils-1.0.0/pg_database/tests/test_config.json
+-rw-r--r--   0        0        0    87523 2023-10-29 02:53:21.451190 pg_database_utils-1.0.0/pg_database/tests/tests.py
+-rw-r--r--   0        0        0     3933 2021-01-24 18:50:28.220993 pg_database_utils-1.0.0/pg_database/types.py
+-rw-r--r--   0        0        0     4601 2021-01-24 18:50:28.221321 pg_database_utils-1.0.0/pg_database/validation.py
+-rw-r--r--   0        0        0      839 2024-04-03 18:24:03.995123 pg_database_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8442 1970-01-01 00:00:00.000000 pg_database_utils-1.0.0/PKG-INFO
```

### Comparing `pg_database_utils-0.9.0/LICENSE` & `pg_database_utils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/README.md` & `pg_database_utils-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pg_database/conf.py` & `pg_database_utils-1.0.0/pg_database/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,18 @@
             )
         elif not django_databases:
             logger.debug("Using provided database configuration")
 
         elif not self._database_config or self._database_config.get("django-db-key") != DEFAULT_DJANGO_DB:
             logger.debug("Applying Django database configuration")
 
+            from django.db import connections
+
+            django_databases = connections.settings
+
             django_db_key = self._database_config.get("django-db-key") or "default"
             if django_db_key not in django_databases:
                 raise EnvironmentError(f'No Django database configured for: "{django_db_key}"')
 
             django_database = {}.fromkeys(("ENGINE", "HOST", "PORT", "NAME", "USER", "PASSWORD"))
             django_database.update(django_databases[django_db_key])
```

### Comparing `pg_database_utils-0.9.0/pg_database/schema.py` & `pg_database_utils-1.0.0/pg_database/schema.py`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pg_database/sql.py` & `pg_database_utils-1.0.0/pg_database/sql.py`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pg_database/tests/custom_databases.py` & `pg_database_utils-1.0.0/pg_database/tests/custom_databases.py`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pg_database/tests/missing_django_db.py` & `pg_database_utils-1.0.0/pg_database/tests/missing_django_db.py`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pg_database/tests/settings.py` & `pg_database_utils-1.0.0/pg_database/tests/settings.py`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pg_database/tests/tests.py` & `pg_database_utils-1.0.0/pg_database/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pg_database/types.py` & `pg_database_utils-1.0.0/pg_database/types.py`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pg_database/validation.py` & `pg_database_utils-1.0.0/pg_database/validation.py`

 * *Files identical despite different names*

### Comparing `pg_database_utils-0.9.0/pyproject.toml` & `pg_database_utils-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pg-database-utils"
-version = "0.9.0"
+version = "1.0.0"
 description = "A suite of utilities for PostgreSQL database queries and operations built on sqlalchemy"
 authors = ["dharvey-consbio <dani.harvey@consbio.org>"]
 keywords = ["postgres", "postgresql", "utils", "utilities", "pg_database", "pg_database_utils", "sqlalchemy"]
 readme = "README.md"
 homepage = "https://github.com/consbio/pg-database-utils/"
 repository = "https://github.com/consbio/pg-database-utils/"
 license = "BSD"
```

### Comparing `pg_database_utils-0.9.0/PKG-INFO` & `pg_database_utils-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pg-database-utils
-Version: 0.9.0
+Version: 1.0.0
 Summary: A suite of utilities for PostgreSQL database queries and operations built on sqlalchemy
 Home-page: https://github.com/consbio/pg-database-utils/
 License: BSD
 Keywords: postgres,postgresql,utils,utilities,pg_database,pg_database_utils,sqlalchemy
 Author: dharvey-consbio
 Author-email: dani.harvey@consbio.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: GeoAlchemy2
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.7.7,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.4.49,<2.0.0)
 Project-URL: Repository, https://github.com/consbio/pg-database-utils/
 Description-Content-Type: text/markdown
```

