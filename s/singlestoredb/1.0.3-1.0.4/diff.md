# Comparing `tmp/singlestoredb-1.0.3.tar.gz` & `tmp/singlestoredb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-1.0.3.tar", last modified: Tue Apr  2 21:29:31 2024, max compression
+gzip compressed data, was "singlestoredb-1.0.4.tar", last modified: Wed Apr  3 17:43:03 2024, max compression
```

## Comparing `singlestoredb-1.0.3.tar` & `singlestoredb-1.0.4.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   151339 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/accel.c
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb/alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44227 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    36712 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb/functions/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/arrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21938 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/mmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/rowdat_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18338 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/fusion/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handlers/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handlers/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/billing_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51907 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (127)    64746 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.189015 singlestoredb-1.0.3/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.189015 singlestoredb-1.0.3/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.189015 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.189015 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/empty.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/singlestoredb/tests/ext_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/ext_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test2.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    50741 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37347 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_ext_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47693 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_ext_func_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_udf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/mogrify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   151339 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/accel.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44227 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36712 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb/functions/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/arrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21938 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/mmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/rowdat_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18338 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/fusion/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handlers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handlers/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/billing_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59380 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64746 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.690379 singlestoredb-1.0.4/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.690379 singlestoredb-1.0.4/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.690379 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.690379 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/empty.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/singlestoredb/tests/ext_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/ext_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test2.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    50741 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37347 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_ext_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47693 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_ext_func_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_udf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/mogrify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-1.0.3/LICENSE` & `singlestoredb-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/PKG-INFO` & `singlestoredb-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.0.3
+Version: 1.0.4
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.0.3/README.md` & `singlestoredb-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/accel.c` & `singlestoredb-1.0.4/accel.c`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/setup.cfg` & `singlestoredb-1.0.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 1.0.3
+version = 1.0.4
 description = Interface to the SingleStoreDB database and workspace management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
```

### Comparing `singlestoredb-1.0.3/setup.py` & `singlestoredb-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/__init__.py` & `singlestoredb-1.0.4/singlestoredb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 from typing import Any
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
```

### Comparing `singlestoredb-1.0.3/singlestoredb/alchemy/__init__.py` & `singlestoredb-1.0.4/singlestoredb/alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/auth.py` & `singlestoredb-1.0.4/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/config.py` & `singlestoredb-1.0.4/singlestoredb/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/connection.py` & `singlestoredb-1.0.4/singlestoredb/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/converters.py` & `singlestoredb-1.0.4/singlestoredb/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/exceptions.py` & `singlestoredb-1.0.4/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/functions/decorator.py` & `singlestoredb-1.0.4/singlestoredb/functions/decorator.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/functions/dtypes.py` & `singlestoredb-1.0.4/singlestoredb/functions/dtypes.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/functions/ext/arrow.py` & `singlestoredb-1.0.4/singlestoredb/functions/ext/arrow.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/functions/ext/asgi.py` & `singlestoredb-1.0.4/singlestoredb/functions/ext/asgi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/functions/ext/json.py` & `singlestoredb-1.0.4/singlestoredb/functions/ext/json.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/functions/ext/mmap.py` & `singlestoredb-1.0.4/singlestoredb/functions/ext/mmap.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/functions/ext/rowdat_1.py` & `singlestoredb-1.0.4/singlestoredb/functions/ext/rowdat_1.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/functions/signature.py` & `singlestoredb-1.0.4/singlestoredb/functions/signature.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/fusion/graphql.py` & `singlestoredb-1.0.4/singlestoredb/fusion/graphql.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/fusion/handler.py` & `singlestoredb-1.0.4/singlestoredb/fusion/handler.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/fusion/handlers/stage.py` & `singlestoredb-1.0.4/singlestoredb/fusion/handlers/stage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/fusion/handlers/utils.py` & `singlestoredb-1.0.4/singlestoredb/fusion/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/fusion/handlers/workspace.py` & `singlestoredb-1.0.4/singlestoredb/fusion/handlers/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/fusion/registry.py` & `singlestoredb-1.0.4/singlestoredb/fusion/registry.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/fusion/result.py` & `singlestoredb-1.0.4/singlestoredb/fusion/result.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/http/__init__.py` & `singlestoredb-1.0.4/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/http/connection.py` & `singlestoredb-1.0.4/singlestoredb/http/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/management/billing_usage.py` & `singlestoredb-1.0.4/singlestoredb/management/billing_usage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/management/cluster.py` & `singlestoredb-1.0.4/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/management/manager.py` & `singlestoredb-1.0.4/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/management/organization.py` & `singlestoredb-1.0.4/singlestoredb/management/organization.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/management/region.py` & `singlestoredb-1.0.4/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/management/utils.py` & `singlestoredb-1.0.4/singlestoredb/management/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import re
 import sys
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
+from typing import Mapping
 from typing import Optional
 from typing import SupportsIndex
 from typing import TypeVar
 from typing import Union
 from urllib.parse import urlparse
 
 import jwt
@@ -278,7 +279,36 @@
     """Convert camel-case to snake-case."""
     if s is None:
         return None
     out = re.sub(r'([A-Z]+)', r'_\1', s).lower()
     if out and out[0] == '_':
         return out[1:]
     return out
+
+
+def snake_to_camel_dict(
+    s: Optional[Mapping[str, Any]],
+    cap_first: bool = False,
+) -> Optional[Dict[str, Any]]:
+    """Convert snake-case keys to camel-case keys."""
+    if s is None:
+        return None
+    out = {}
+    for k, v in s.items():
+        if isinstance(s, Mapping):
+            out[str(snake_to_camel(k))] = snake_to_camel_dict(v, cap_first=cap_first)
+        else:
+            out[str(snake_to_camel(k))] = v
+    return out
+
+
+def camel_to_snake_dict(s: Optional[Mapping[str, Any]]) -> Optional[Dict[str, Any]]:
+    """Convert camel-case keys to snake-case keys."""
+    if s is None:
+        return None
+    out = {}
+    for k, v in s.items():
+        if isinstance(s, Mapping):
+            out[str(camel_to_snake(k))] = camel_to_snake_dict(v)
+        else:
+            out[str(camel_to_snake(k))] = v
+    return out
```

### Comparing `singlestoredb-1.0.3/singlestoredb/management/workspace.py` & `singlestoredb-1.0.4/singlestoredb/management/workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 from __future__ import annotations
 
 import datetime
 import glob
 import io
 import os
 import re
-import socket
 import time
+from collections.abc import Mapping
 from typing import Any
 from typing import BinaryIO
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import TextIO
 from typing import Union
 
 from .. import connection
 from ..exceptions import ManagementError
 from .billing_usage import BillingUsageItem
 from .manager import Manager
 from .organization import Organization
 from .region import Region
+from .utils import camel_to_snake_dict
 from .utils import from_datetime
 from .utils import NamedList
 from .utils import PathLike
 from .utils import snake_to_camel
+from .utils import snake_to_camel_dict
 from .utils import to_datetime
 from .utils import ttl_property
 from .utils import vars_to_str
 
 
 def get_secret(name: str) -> str:
     """Get a secret from the organization."""
@@ -930,14 +932,20 @@
         workspace_id: str,
         workspace_group: Union[str, 'WorkspaceGroup'],
         size: str,
         state: str,
         created_at: Union[str, datetime.datetime],
         terminated_at: Optional[Union[str, datetime.datetime]] = None,
         endpoint: Optional[str] = None,
+        auto_suspend: Optional[Dict[str, Any]] = None,
+        cache_config: Optional[int] = None,
+        deployment_type: Optional[str] = None,
+        resume_attachments: Optional[Dict[str, Any]] = None,
+        scaling_progress: Optional[int] = None,
+        last_resumed_at: Optional[str] = None,
     ):
         #: Name of the workspace
         self.name = name
 
         #: Unique ID of the workspace
         self.id = workspace_id
 
@@ -959,14 +967,32 @@
 
         #: Timestamp of when the workspace was terminated
         self.terminated_at = to_datetime(terminated_at)
 
         #: Hostname (or IP address) of the workspace database server
         self.endpoint = endpoint
 
+        #: Current auto-suspend settings
+        self.auto_suspend = camel_to_snake_dict(auto_suspend)
+
+        #: Multiplier for the persistent cache
+        self.cache_config = cache_config
+
+        #: Deployment type of the workspace
+        self.deployment_type = deployment_type
+
+        #: Database attachments
+        self.resume_attachments = camel_to_snake_dict(resume_attachments)
+
+        #: Current progress percentage for scaling the workspace
+        self.scaling_progress = scaling_progress
+
+        #: Timestamp when workspace was last resumed
+        self.last_resumed_at = to_datetime(last_resumed_at)
+
         self._manager: Optional[WorkspaceManager] = None
 
     def __str__(self) -> str:
         """Return string representation."""
         return vars_to_str(self)
 
     def __repr__(self) -> str:
@@ -987,32 +1013,84 @@
 
         Returns
         -------
         :class:`Workspace`
 
         """
         out = cls(
-            name=obj['name'], workspace_id=obj['workspaceID'],
+            name=obj['name'],
+            workspace_id=obj['workspaceID'],
             workspace_group=obj['workspaceGroupID'],
-            size=obj.get('size', 'Unknown'), state=obj['state'],
-            created_at=obj['createdAt'], terminated_at=obj.get('terminatedAt'),
+            size=obj.get('size', 'Unknown'),
+            state=obj['state'],
+            created_at=obj['createdAt'],
+            terminated_at=obj.get('terminatedAt'),
             endpoint=obj.get('endpoint'),
+            auto_suspend=obj.get('autoSuspend'),
+            cache_config=obj.get('cacheConfig'),
+            deployment_type=obj.get('deploymentType'),
+            last_resumed_at=obj.get('lastResumedAt'),
+            resume_attachments=obj.get('resumeAttachments'),
+            scaling_progress=obj.get('scalingProgress'),
         )
         out._manager = manager
         return out
 
+    def update(
+        self,
+        auto_suspend: Optional[Dict[str, Any]] = None,
+        cache_config: Optional[int] = None,
+        deployment_type: Optional[str] = None,
+        size: Optional[str] = None,
+    ) -> None:
+        """
+        Update the workspace definition.
+
+        Parameters
+        ----------
+        auto_suspend : Dict[str, Any], optional
+            Auto-suspend mode for the workspace: IDLE, SCHEDULED, DISABLED
+        cache_config : int, optional
+            Specifies the multiplier for the persistent cache associated
+            with the workspace. If specified, it enables the cache configuration
+            multiplier. It can have one of the following values: 1, 2, or 4.
+        deployment_type : str, optional
+            The deployment type that will be applied to all the workspaces
+            within the group
+        size : str, optional
+            Size of the workspace (in workspace size notation), such as "S-1".
+
+        """
+        if self._manager is None:
+            raise ManagementError(
+                msg='No workspace manager is associated with this object.',
+            )
+        data = {
+            k: v for k, v in dict(
+                autoSuspend=snake_to_camel_dict(auto_suspend),
+                cacheConfig=cache_config,
+                deploymentType=deployment_type,
+                size=size,
+            ).items() if v is not None
+        }
+        self._manager._patch(f'workspaces/{self.id}', json=data)
+        self.refresh()
+
     def refresh(self) -> Workspace:
         """Update the object to the current state."""
         if self._manager is None:
             raise ManagementError(
                 msg='No workspace manager is associated with this object.',
             )
         new_obj = self._manager.get_workspace(self.id)
         for name, value in vars(new_obj).items():
-            setattr(self, name, value)
+            if isinstance(value, Mapping):
+                setattr(self, name, snake_to_camel_dict(value))
+            else:
+                setattr(self, name, value)
         return self
 
     def terminate(
         self,
         wait_on_terminated: bool = False,
         wait_interval: int = 10,
         wait_timeout: int = 600,
@@ -1107,23 +1185,26 @@
                 self._manager.get_workspace(self.id),
                 'Suspended', interval=wait_interval, timeout=wait_timeout,
             )
             self.refresh()
 
     def resume(
         self,
+        disable_auto_suspend: bool = False,
         wait_on_resumed: bool = False,
         wait_interval: int = 20,
         wait_timeout: int = 600,
     ) -> None:
         """
         Resume the workspace.
 
         Parameters
         ----------
+        disable_auto_suspend : bool, optional
+            Should auto-suspend be disabled?
         wait_on_resumed : bool, optional
             Wait for the workspace to go into 'Resumed' or 'Active' mode before returning
         wait_interval : int, optional
             Number of seconds between each server check
         wait_timeout : int, optional
             Total number of seconds to check server before giving up
 
@@ -1133,15 +1214,18 @@
             If timeout is reached
 
         """
         if self._manager is None:
             raise ManagementError(
                 msg='No workspace manager is associated with this object.',
             )
-        self._manager._post(f'workspaces/{self.id}/resume')
+        self._manager._post(
+            f'workspaces/{self.id}/resume',
+            json=dict(disableAutoSuspend=disable_auto_suspend),
+        )
         if wait_on_resumed:
             self._manager._wait_on_state(
                 self._manager.get_workspace(self.id),
                 ['Resumed', 'Active'], interval=wait_interval, timeout=wait_timeout,
             )
             self.refresh()
 
@@ -1166,14 +1250,15 @@
 
     def __init__(
         self, name: str, id: str,
         created_at: Union[str, datetime.datetime],
         region: Optional[Region],
         firewall_ranges: List[str],
         terminated_at: Optional[Union[str, datetime.datetime]],
+        allow_all_traffic: Optional[bool],
     ):
         #: Name of the workspace group
         self.name = name
 
         #: Unique ID of the workspace group
         self.id = id
 
@@ -1185,14 +1270,17 @@
 
         #: List of allowed incoming IP addresses / ranges
         self.firewall_ranges = firewall_ranges
 
         #: Timestamp of when the workspace group was terminated
         self.terminated_at = to_datetime(terminated_at)
 
+        #: Should all traffic be allowed?
+        self.allow_all_traffic = allow_all_traffic
+
         self._manager: Optional[WorkspaceManager] = None
 
     def __str__(self) -> str:
         """Return string representation."""
         return vars_to_str(self)
 
     def __repr__(self) -> str:
@@ -1225,14 +1313,15 @@
         out = cls(
             name=obj['name'],
             id=obj['workspaceGroupID'],
             created_at=obj['createdAt'],
             region=region,
             firewall_ranges=obj.get('firewallRanges', []),
             terminated_at=obj.get('terminatedAt'),
+            allow_all_traffic=obj.get('allowAllTraffic'),
         )
         out._manager = manager
         return out
 
     @property
     def organization(self) -> Organization:
         if self._manager is None:
@@ -1256,43 +1345,67 @@
         """Update the object to the current state."""
         if self._manager is None:
             raise ManagementError(
                 msg='No workspace manager is associated with this object.',
             )
         new_obj = self._manager.get_workspace_group(self.id)
         for name, value in vars(new_obj).items():
-            setattr(self, name, value)
+            if isinstance(value, Mapping):
+                setattr(self, name, camel_to_snake_dict(value))
+            else:
+                setattr(self, name, value)
         return self
 
     def update(
-        self, name: Optional[str] = None,
-        admin_password: Optional[str] = None,
+        self,
+        name: Optional[str] = None,
         firewall_ranges: Optional[List[str]] = None,
+        admin_password: Optional[str] = None,
+        expires_at: Optional[str] = None,
+        allow_all_traffic: Optional[bool] = None,
+        update_window: Optional[Dict[str, int]] = None,
     ) -> None:
         """
         Update the workspace group definition.
 
         Parameters
         ----------
         name : str, optional
-            Workspace group name
-        admim_password : str, optional
-            Admin password for the workspace group
-        firewall_ranges : Sequence[str], optional
-            List of allowed incoming IP addresses
+            Name of the workspace group
+        firewall_ranges : list[str], optional
+            List of allowed CIDR ranges. An empty list indicates that all
+            inbound requests are allowed.
+        admin_password : str, optional
+            Admin password for the workspace group. If no password is supplied,
+            a password will be generated and retured in the response.
+        expires_at : str, optional
+            The timestamp of when the workspace group will expire.
+            If the expiration time is not specified,
+            the workspace group will have no expiration time.
+            At expiration, the workspace group is terminated and all the data is lost.
+            Expiration time can be specified as a timestamp or duration.
+            Example: "2021-01-02T15:04:05Z07:00", "2021-01-02", "3h30m"
+        allow_all_traffic : bool, optional
+            Allow all traffic to the workspace group
+        update_window : Dict[str, int], optional
+            Specify the day and hour of an update window: dict(day=0-6, hour=0-23)
 
         """
         if self._manager is None:
             raise ManagementError(
                 msg='No workspace manager is associated with this object.',
             )
         data = {
             k: v for k, v in dict(
-                name=name, adminPassword=admin_password,
+                name=name,
                 firewallRanges=firewall_ranges,
+                adminPassword=admin_password,
+                expiresAt=expires_at,
+                allowAllTraffic=allow_all_traffic,
+                updateWindow=snake_to_camel_dict(update_window),
             ).items() if v is not None
         }
         self._manager._patch(f'workspaceGroups/{self.id}', json=data)
         self.refresh()
 
     def terminate(
         self, force: bool = False,
@@ -1334,57 +1447,72 @@
                     raise ManagementError(
                         msg='Exceeded waiting time for WorkspaceGroup to terminate',
                     )
                 time.sleep(wait_interval)
                 wait_timeout -= wait_interval
 
     def create_workspace(
-        self, name: str, size: Optional[str] = None,
-        wait_on_active: bool = False, wait_interval: int = 10,
-        wait_timeout: int = 600, add_endpoint_to_firewall_ranges: bool = True,
+        self,
+        name: str,
+        size: Optional[str] = None,
+        auto_suspend: Optional[Dict[str, Any]] = None,
+        cache_config: Optional[int] = None,
+        enable_kai: Optional[bool] = None,
+        wait_on_active: bool = False,
+        wait_interval: int = 10,
+        wait_timeout: int = 600,
     ) -> Workspace:
         """
         Create a new workspace.
 
         Parameters
         ----------
         name : str
             Name of the workspace
         size : str, optional
             Workspace size in workspace size notation (S-00, S-1, etc.)
+        auto_suspend : Dict[str, Any], optional
+            Auto suspend settings for the workspace. If this field is not
+            provided, no settings will be enabled.
+        cache_config : int, optional
+            Specifies the multiplier for the persistent cache associated
+            with the workspace. If specified, it enables the cache configuration
+            multiplier. It can have one of the following values: 1, 2, or 4.
+        enable_kai : bool, optional
+            Whether to create a SingleStore Kai-enabled workspace
         wait_on_active : bool, optional
             Wait for the workspace to be active before returning
         wait_timeout : int, optional
             Maximum number of seconds to wait before raising an exception
             if wait=True
         wait_interval : int, optional
             Number of seconds between each polling interval
-        add_endpoint_to_firewall_ranges : bool, optional
-            Should the workspace endpoint be added to the workspace group
-            firewall ranges?
 
         Returns
         -------
         :class:`Workspace`
 
         """
         if self._manager is None:
             raise ManagementError(
                 msg='No workspace manager is associated with this object.',
             )
 
         out = self._manager.create_workspace(
-            name=name, workspace_group=self, size=size, wait_on_active=wait_on_active,
-            wait_interval=wait_interval, wait_timeout=wait_timeout,
+            name=name,
+            workspace_group=self,
+            size=size,
+            auto_suspend=snake_to_camel_dict(auto_suspend),
+            cache_config=cache_config,
+            enable_kai=enable_kai,
+            wait_on_active=wait_on_active,
+            wait_interval=wait_interval,
+            wait_timeout=wait_timeout,
         )
 
-        if add_endpoint_to_firewall_ranges and out.endpoint is not None:
-            ip_address = '{}/32'.format(socket.gethostbyname(out.endpoint))
-            self.update(firewall_ranges=self.firewall_ranges+[ip_address])
-
         return out
 
     @property
     def workspaces(self) -> NamedList[Workspace]:
         """Return a list of available workspaces."""
         if self._manager is None:
             raise ManagementError(
@@ -1521,17 +1649,23 @@
     @ttl_property(datetime.timedelta(hours=1))
     def regions(self) -> NamedList[Region]:
         """Return a list of available regions."""
         res = self._get('regions')
         return NamedList([Region.from_dict(item, self) for item in res.json()])
 
     def create_workspace_group(
-        self, name: str, region: Union[str, Region],
-        firewall_ranges: List[str], admin_password: Optional[str] = None,
+        self,
+        name: str,
+        region: Union[str, Region],
+        firewall_ranges: List[str],
+        admin_password: Optional[str] = None,
+        backup_bucket_kms_key_id: Optional[str] = None,
+        data_bucket_kms_key_id: Optional[str] = None,
         expires_at: Optional[str] = None,
+        smart_dr: Optional[bool] = None,
         allow_all_traffic: Optional[bool] = None,
         update_window: Optional[Dict[str, int]] = None,
     ) -> WorkspaceGroup:
         """
         Create a new workspace group.
 
         Parameters
@@ -1542,21 +1676,36 @@
             ID of the region where the workspace group should be created
         firewall_ranges : list[str]
             List of allowed CIDR ranges. An empty list indicates that all
             inbound requests are allowed.
         admin_password : str, optional
             Admin password for the workspace group. If no password is supplied,
             a password will be generated and retured in the response.
+        backup_bucket_kms_key_id : str, optional
+            Specifies the KMS key ID associated with the backup bucket.
+            If specified, enables Customer-Managed Encryption Keys (CMEK)
+            encryption for the backup bucket of the workspace group.
+            This feature is only supported in workspace groups deployed in AWS.
+        data_bucket_kms_key_id : str, optional
+            Specifies the KMS key ID associated with the data bucket.
+            If specified, enables Customer-Managed Encryption Keys (CMEK)
+            encryption for the data bucket and Amazon Elastic Block Store
+            (EBS) volumes of the workspace group. This feature is only supported
+            in workspace groups deployed in AWS.
         expires_at : str, optional
             The timestamp of when the workspace group will expire.
             If the expiration time is not specified,
             the workspace group will have no expiration time.
             At expiration, the workspace group is terminated and all the data is lost.
             Expiration time can be specified as a timestamp or duration.
             Example: "2021-01-02T15:04:05Z07:00", "2021-01-02", "3h30m"
+        smart_dr : bool, optional
+            Enables Smart Disaster Recovery (SmartDR) for the workspace group.
+            SmartDR is a disaster recovery solution that ensures seamless and
+            continuous replication of data from the primary region to a secondary region
         allow_all_traffic : bool, optional
             Allow all traffic to the workspace group
         update_window : Dict[str, int], optional
             Specify the day and hour of an update window: dict(day=0-6, hour=0-23)
 
         Returns
         -------
@@ -1565,38 +1714,57 @@
         """
         if isinstance(region, Region):
             region = region.id
         res = self._post(
             'workspaceGroups', json=dict(
                 name=name, regionID=region,
                 adminPassword=admin_password,
+                backupBucketKMSKeyID=backup_bucket_kms_key_id,
+                dataBucketKMSKeyID=data_bucket_kms_key_id,
                 firewallRanges=firewall_ranges or [],
                 expiresAt=expires_at,
+                smartDR=smart_dr,
                 allowAllTraffic=allow_all_traffic,
-                updateWindow=update_window,
+                updateWindow=snake_to_camel_dict(update_window),
             ),
         )
         return self.get_workspace_group(res.json()['workspaceGroupID'])
 
     def create_workspace(
-        self, name: str, workspace_group: Union[str, WorkspaceGroup],
-        size: Optional[str] = None, wait_on_active: bool = False,
-        wait_interval: int = 10, wait_timeout: int = 600,
+        self,
+        name: str,
+        workspace_group: Union[str, WorkspaceGroup],
+        size: Optional[str] = None,
+        auto_suspend: Optional[Dict[str, Any]] = None,
+        cache_config: Optional[int] = None,
+        enable_kai: Optional[bool] = None,
+        wait_on_active: bool = False,
+        wait_interval: int = 10,
+        wait_timeout: int = 600,
     ) -> Workspace:
         """
         Create a new workspace.
 
         Parameters
         ----------
         name : str
             Name of the workspace
         workspace_group : str or WorkspaceGroup
             The workspace ID of the workspace
         size : str, optional
             Workspace size in workspace size notation (S-00, S-1, etc.)
+        auto_suspend : Dict[str, Any], optional
+            Auto suspend settings for the workspace. If this field is not
+            provided, no settings will be enabled.
+        cache_config : int, optional
+            Specifies the multiplier for the persistent cache associated
+            with the workspace. If specified, it enables the cache configuration
+            multiplier. It can have one of the following values: 1, 2, or 4.
+        enable_kai : bool, optional
+            Whether to create a SingleStore Kai-enabled workspace
         wait_on_active : bool, optional
             Wait for the workspace to be active before returning
         wait_timeout : int, optional
             Maximum number of seconds to wait before raising an exception
             if wait=True
         wait_interval : int, optional
             Number of seconds between each polling interval
@@ -1606,22 +1774,28 @@
         :class:`Workspace`
 
         """
         if isinstance(workspace_group, WorkspaceGroup):
             workspace_group = workspace_group.id
         res = self._post(
             'workspaces', json=dict(
-                name=name, workspaceGroupID=workspace_group,
+                name=name,
+                workspaceGroupID=workspace_group,
                 size=size,
+                autoSuspend=snake_to_camel_dict(auto_suspend),
+                cacheConfig=cache_config,
+                enableKai=enable_kai,
             ),
         )
         out = self.get_workspace(res.json()['workspaceID'])
         if wait_on_active:
             out = self._wait_on_state(
-                out, 'Active', interval=wait_interval,
+                out,
+                'Active',
+                interval=wait_interval,
                 timeout=wait_timeout,
             )
         return out
 
     def get_workspace_group(self, id: str) -> WorkspaceGroup:
         """
         Retrieve a workspace group definition.
```

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/__init__.py` & `singlestoredb-1.0.4/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/_auth.py` & `singlestoredb-1.0.4/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/charset.py` & `singlestoredb-1.0.4/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/connection.py` & `singlestoredb-1.0.4/singlestoredb/mysql/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-1.0.4/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-1.0.4/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/constants/CR.py` & `singlestoredb-1.0.4/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/constants/ER.py` & `singlestoredb-1.0.4/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/converters.py` & `singlestoredb-1.0.4/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/cursors.py` & `singlestoredb-1.0.4/singlestoredb/mysql/cursors.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/err.py` & `singlestoredb-1.0.4/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/optionfile.py` & `singlestoredb-1.0.4/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/protocol.py` & `singlestoredb-1.0.4/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/base.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/pytest.py` & `singlestoredb-1.0.4/singlestoredb/pytest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/ext_funcs/__init__.py` & `singlestoredb-1.0.4/singlestoredb/tests/ext_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test.sql` & `singlestoredb-1.0.4/singlestoredb/tests/test.sql`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_basics.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_config.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_connection.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_dbapi.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_exceptions.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_ext_func.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_ext_func.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_ext_func_data.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_ext_func_data.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_fusion.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_http.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_management.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_plugin.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_results.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_types.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_udf.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/test_xdict.py` & `singlestoredb-1.0.4/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/tests/utils.py` & `singlestoredb-1.0.4/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/types.py` & `singlestoredb-1.0.4/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/utils/config.py` & `singlestoredb-1.0.4/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/utils/convert_rows.py` & `singlestoredb-1.0.4/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/utils/mogrify.py` & `singlestoredb-1.0.4/singlestoredb/utils/mogrify.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/utils/results.py` & `singlestoredb-1.0.4/singlestoredb/utils/results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb/utils/xdict.py` & `singlestoredb-1.0.4/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.3/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-1.0.4/singlestoredb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.0.3
+Version: 1.0.4
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.0.3/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-1.0.4/singlestoredb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

