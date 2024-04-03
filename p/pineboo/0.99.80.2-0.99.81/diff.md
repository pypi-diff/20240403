# Comparing `tmp/pineboo-0.99.80.2.tar.gz` & `tmp/pineboo-0.99.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pineboo-0.99.80.2.tar", last modified: Mon Jan  8 11:17:22 2024, max compression
+gzip compressed data, was "pineboo-0.99.81.tar", last modified: Wed Apr  3 08:18:28 2024, max compression
```

## Comparing `pineboo-0.99.80.2.tar` & `pineboo-0.99.81.tar`

### file list

```diff
@@ -1,736 +1,736 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1078 2019-07-27 10:21:43.000000 pineboo-0.99.80.2/LICENSE.mit
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5892 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4639 2023-10-17 07:14:02.000000 pineboo-0.99.80.2/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.043134 pineboo-0.99.80.2/pineboo.egg-info/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5892 2024-01-08 11:17:21.000000 pineboo-0.99.80.2/pineboo.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28782 2024-01-08 11:17:22.000000 pineboo-0.99.80.2/pineboo.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2024-01-08 11:17:21.000000 pineboo-0.99.80.2/pineboo.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      386 2024-01-08 11:17:21.000000 pineboo-0.99.80.2/pineboo.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      584 2024-01-08 11:17:21.000000 pineboo-0.99.80.2/pineboo.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2024-01-08 11:17:21.000000 pineboo-0.99.80.2/pineboo.egg-info/top_level.txt
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.043134 pineboo-0.99.80.2/pineboolib/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      179 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.043134 pineboo-0.99.80.2/pineboolib/application/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1612 2024-01-08 11:16:40.000000 pineboo-0.99.80.2/pineboolib/application/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.043134 pineboo-0.99.80.2/pineboolib/application/acls/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       20 2019-09-08 08:23:19.000000 pineboo-0.99.80.2/pineboolib/application/acls/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9234 2023-11-15 10:12:11.000000 pineboo-0.99.80.2/pineboolib/application/acls/pnaccesscontrol.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7410 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/acls/pnaccesscontrolfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9987 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/application/acls/pnaccesscontrollists.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1554 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/acls/pnboolflagstate.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.043134 pineboo-0.99.80.2/pineboolib/application/acls/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      269 2020-08-26 10:35:25.000000 pineboo-0.99.80.2/pineboolib/application/acls/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24548 2023-08-17 09:18:35.000000 pineboo-0.99.80.2/pineboolib/application/acls/tests/test_acls.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      970 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/acls/tests/test_pnaccesscontrol.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9011 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/connections.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.043134 pineboo-0.99.80.2/pineboolib/application/database/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      210 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/database/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.043134 pineboo-0.99.80.2/pineboolib/application/database/orm/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       43 2020-05-06 20:13:13.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5019 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/alembic_tools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    38146 2023-10-16 09:53:27.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/basemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6346 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/dummy_cursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1083 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/dummy_signal.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-06-24 11:26:48.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11925 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_basemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2499 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_bytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4086 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_consistency.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3575 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_dummycursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3980 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_query_orm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3395 2023-12-20 10:51:37.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_relationships.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5463 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_sessions.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4744 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_signals.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2509 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_thread_session.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1689 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1080 2020-10-15 10:56:54.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_view.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11303 2023-11-20 09:19:51.000000 pineboo-0.99.80.2/pineboolib/application/database/orm/utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8356 2023-10-04 10:16:55.000000 pineboo-0.99.80.2/pineboolib/application/database/pnbuffer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20954 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/pnconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17308 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/pnconnectionmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    40438 2023-11-15 10:12:11.000000 pineboo-0.99.80.2/pineboolib/application/database/pncursortablemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2020-06-29 10:01:24.000000 pineboo-0.99.80.2/pineboolib/application/database/pngroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2020-01-10 07:21:12.000000 pineboo-0.99.80.2/pineboolib/application/database/pnparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1340 2021-03-09 11:41:24.000000 pineboo-0.99.80.2/pineboolib/application/database/pnsignals.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   123413 2023-11-16 08:49:18.000000 pineboo-0.99.80.2/pineboolib/application/database/pnsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5770 2023-04-18 17:17:33.000000 pineboo-0.99.80.2/pineboolib/application/database/pnsqldriversmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    30622 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/application/database/pnsqlquery.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/database/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-12-02 11:03:25.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5985 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnbuffer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9972 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4011 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnconnection_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8048 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pncursortablemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      413 2019-08-28 09:29:35.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pngroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      600 2019-08-28 09:29:35.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    43087 2023-09-20 09:16:19.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1170 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnsqldriversmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28220 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3475 2023-10-04 10:16:36.000000 pineboo-0.99.80.2/pineboolib/application/database/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16052 2023-10-16 09:39:59.000000 pineboo-0.99.80.2/pineboolib/application/database/utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1475 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/file.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11533 2023-11-20 09:19:51.000000 pineboo-0.99.80.2/pineboolib/application/load_script.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/metadata/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      166 2019-07-30 14:11:28.000000 pineboo-0.99.80.2/pineboolib/application/metadata/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4940 2023-11-15 10:12:11.000000 pineboo-0.99.80.2/pineboolib/application/metadata/pnaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2345 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/metadata/pncompoundkeymetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    33256 2023-11-15 10:12:11.000000 pineboo-0.99.80.2/pineboolib/application/metadata/pnfieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7344 2023-11-15 10:12:11.000000 pineboo-0.99.80.2/pineboolib/application/metadata/pnrelationmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25988 2024-01-07 09:10:01.000000 pineboo-0.99.80.2/pineboolib/application/metadata/pntablemetadata.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/metadata/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-03 08:33:48.000000 pineboo-0.99.80.2/pineboolib/application/metadata/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1217 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pnaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2311 2020-02-05 09:39:18.000000 pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16131 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pnfieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4190 2021-08-23 10:27:07.000000 pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pnrelationmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7571 2024-01-08 11:13:46.000000 pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pntablemetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2862 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/module.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4141 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/moduleactions.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       47 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/modules_tree.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      122 2019-07-31 07:36:22.000000 pineboo-0.99.80.2/pineboolib/application/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10703 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/packager/pnpackager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1947 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/packager/pnunpacker.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/packager/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-01-21 10:44:31.000000 pineboo-0.99.80.2/pineboolib/application/packager/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1763 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/packager/tests/test_pnpackager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1519 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/packager/tests/test_pnunpaker.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       70 2019-07-29 14:08:13.000000 pineboo-0.99.80.2/pineboolib/application/parsers/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       56 2020-04-23 09:34:52.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15166 2023-11-20 09:19:51.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/kparsertools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44121 2023-11-20 09:19:51.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/kut2fpdf.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      291 2020-04-23 09:34:52.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10581 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       50 2020-04-23 09:34:52.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14321 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/pnmtdparser.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5416 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-04-23 09:34:52.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1884 2023-12-20 10:52:15.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      168 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      587 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/flex.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31605 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/flscriptparse.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3400 2020-04-23 09:34:52.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/lextab.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28374 2023-05-17 09:53:26.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/postparse.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8675 2023-05-01 18:19:35.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/pyconvert.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    94792 2023-11-15 10:12:11.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/pytnyzer.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      502 2020-04-23 09:34:52.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17353 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6174 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/token_rules.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/parser_ui/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      101 2020-04-23 09:34:52.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_ui/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50214 2023-10-16 10:19:24.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_ui/qt3ui.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/parsers/parser_ui/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       33 2020-04-23 09:34:52.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_ui/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    34853 2023-08-17 07:11:55.000000 pineboo-0.99.80.2/pineboolib/application/pnapplication.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      371 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/pncore.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6780 2023-08-17 08:09:49.000000 pineboo-0.99.80.2/pineboolib/application/process.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    26571 2023-09-19 10:18:34.000000 pineboo-0.99.80.2/pineboolib/application/projectmodule.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3677 2023-09-05 10:16:39.000000 pineboo-0.99.80.2/pineboolib/application/proxy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6901 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/qsadictmodules.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/qsatypes/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-08-01 20:49:12.000000 pineboo-0.99.80.2/pineboolib/application/qsatypes/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7972 2023-12-20 09:42:37.000000 pineboo-0.99.80.2/pineboolib/application/qsatypes/date.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20102 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/qsatypes/sysbasetype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/qsatypes/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-06 06:55:22.000000 pineboo-0.99.80.2/pineboolib/application/qsatypes/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1882 2023-12-20 14:51:09.000000 pineboo-0.99.80.2/pineboolib/application/qsatypes/tests/test_date.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5455 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/qsatypes/tests/test_sysbasetype.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3461 2021-03-29 11:28:24.000000 pineboo-0.99.80.2/pineboolib/application/safeqsa.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/signatures/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-12-25 17:46:05.000000 pineboo-0.99.80.2/pineboolib/application/signatures/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6413 2023-10-16 09:40:58.000000 pineboo-0.99.80.2/pineboolib/application/signatures/pdf_digest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9054 2024-01-02 09:55:33.000000 pineboo-0.99.80.2/pineboolib/application/signatures/pdf_qr.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/signatures/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      286 2021-01-18 11:51:09.000000 pineboo-0.99.80.2/pineboolib/application/signatures/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3440 2024-01-02 10:01:45.000000 pineboo-0.99.80.2/pineboolib/application/signatures/tests/test_signatures.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9484 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/signatures/xml_digest.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/staticloader/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-10-04 20:53:14.000000 pineboo-0.99.80.2/pineboolib/application/staticloader/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14931 2023-09-05 11:00:22.000000 pineboo-0.99.80.2/pineboolib/application/staticloader/pnmodulesstaticloader.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/staticloader/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      289 2020-09-07 08:35:55.000000 pineboo-0.99.80.2/pineboolib/application/staticloader/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2491 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/staticloader/tests/test_static_loader.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/staticloader/ui/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-08-17 12:14:19.000000 pineboo-0.99.80.2/pineboolib/application/staticloader/ui/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7299 2020-03-10 09:40:23.000000 pineboo-0.99.80.2/pineboolib/application/staticloader/ui/static_loader.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      287 2019-10-09 06:29:09.000000 pineboo-0.99.80.2/pineboolib/application/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2020-06-10 19:38:58.000000 pineboo-0.99.80.2/pineboolib/application/tests/test_application.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1350 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/tests/test_load_script.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1309 2020-09-21 07:02:30.000000 pineboo-0.99.80.2/pineboolib/application/tests/test_process.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1259 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/tests/test_projectmodule.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2020-09-04 08:27:19.000000 pineboo-0.99.80.2/pineboolib/application/tests/test_proxy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16925 2023-04-07 15:43:24.000000 pineboo-0.99.80.2/pineboolib/application/tests/test_types.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1319 2020-09-07 08:35:55.000000 pineboo-0.99.80.2/pineboolib/application/tests/test_xmlaction.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/translator/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-04-05 08:54:23.000000 pineboo-0.99.80.2/pineboolib/application/translator/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5429 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/translator/pntranslator.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.047134 pineboo-0.99.80.2/pineboolib/application/translator/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       34 2020-12-01 12:01:44.000000 pineboo-0.99.80.2/pineboolib/application/translator/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      802 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/translator/test/test_pntranslator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    21647 2023-07-27 08:57:49.000000 pineboo-0.99.80.2/pineboolib/application/types.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.051134 pineboo-0.99.80.2/pineboolib/application/utils/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      182 2019-07-31 08:47:54.000000 pineboo-0.99.80.2/pineboolib/application/utils/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1548 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/utils/check_dependencies.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2245 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/utils/convert_flaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/utils/date_conversion.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6101 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/utils/flfiles_dir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1120 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/utils/geometry.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1949 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/utils/mobilemode.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2450 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/application/utils/modules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1625 2023-12-20 10:52:04.000000 pineboo-0.99.80.2/pineboolib/application/utils/path.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4727 2020-11-25 10:48:38.000000 pineboo-0.99.80.2/pineboolib/application/utils/service.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    23217 2023-11-20 09:30:14.000000 pineboo-0.99.80.2/pineboolib/application/utils/sql_tools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1307 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/application/utils/xpm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15050 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/application/xmlaction.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.051134 pineboo-0.99.80.2/pineboolib/core/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      268 2021-03-29 11:28:24.000000 pineboo-0.99.80.2/pineboolib/core/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8761 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/core/decorators.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      746 2020-10-16 07:17:25.000000 pineboo-0.99.80.2/pineboolib/core/exceptions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.051134 pineboo-0.99.80.2/pineboolib/core/fonts/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-0.99.80.2/pineboolib/core/fonts/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.051134 pineboo-0.99.80.2/pineboolib/core/fonts/noto_sans/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-03-09 09:55:39.000000 pineboo-0.99.80.2/pineboolib/core/fonts/noto_sans/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2577 2023-12-20 10:52:30.000000 pineboo-0.99.80.2/pineboolib/core/garbage_collector.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.051134 pineboo-0.99.80.2/pineboolib/core/images/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-0.99.80.2/pineboolib/core/images/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.067134 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      960 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Pi-symbol.svg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)  1464366 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi.psd
--rw-rw-r--   0 aulla     (1000) aulla     (1000)  9487782 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi2.xcf
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   476635 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50853 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi2_256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   147180 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi2_512.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50737 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi_1024.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi_256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29321 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi_512.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-09-17 09:33:15.000000 pineboo-0.99.80.2/pineboolib/core/images/icono_pi/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.075133 pineboo-0.99.80.2/pineboolib/core/images/icons/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/__init__.py
--rwxrwxr-x   0 aulla     (1000) aulla     (1000)      892 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/about.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1230 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/aboutqt.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      853 2019-10-01 07:14:24.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/cancel.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/consola.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      669 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/date.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2199 2019-09-30 08:28:48.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/delete.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2562 2019-10-01 07:14:24.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2069 2019-09-30 08:28:48.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/edit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2237 2020-01-15 08:29:51.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/edit_file.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2020-01-15 08:29:51.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/edit_file_xml.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      934 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/estilo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      870 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/exit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/flfielddb.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      691 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/fltable-clean.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/fltable-data.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/fltable-filter.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      727 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/fltable-odf.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      459 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/folder.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      615 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/folder_update.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      563 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/font.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-bottom.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-first.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-home.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-jump.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-last.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-next.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-previous.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-top.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/go-up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      601 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-add.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1624 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-bold.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-cancel.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1682 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-clear.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      723 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-copy.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-cut.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2049 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-delete.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2104 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-find-and-replace.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1636 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-find.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1256 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-fullscreen.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-back-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-back-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-forward-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-forward-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-bottom.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-first-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-first-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-last-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-last-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-top.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-home.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-indent-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-indent-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1338 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-italic.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-jump-to-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-jump-to-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-justify-center.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      517 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-justify-fill.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      515 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-justify-left.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-justify-right.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-forward-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-forward-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-next-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-next-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      481 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-pause.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1028 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-play-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-previous-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-previous-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1266 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-record.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-rewind-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-rewind-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-stop.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1008 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-new.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-open.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1027 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-paste.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1719 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-print-preview.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1013 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-print.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1115 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-properties.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1502 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-redo-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-refresh.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      317 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-remove.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1837 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-save-as.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1971 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-save.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      631 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-select-all.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-stop.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1445 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-strikethrough.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-underline.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1601 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-undo-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-unindent-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-unindent-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      911 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/help_index.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1854 2019-09-30 08:28:48.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/insert.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      711 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/lock.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      579 2019-10-01 07:14:24.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/ok.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1997 2019-09-30 08:28:48.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/paste.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-128.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      857 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-16.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1406 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-24.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1941 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-32.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2991 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-48.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3482 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-57.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3243 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-64.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-72.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19949 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-128.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1216 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-16.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1720 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-24.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    52103 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2568 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-32.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4552 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-48.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7028 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-64.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17588 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-09-30 08:28:48.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/print.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      885 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/reload.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22869 2022-07-06 21:01:18.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/signed_stamp.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1930 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_ebcomportamiento.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1571 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flareas.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2952 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_fldumpdb.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1133 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flgroups.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1871 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flloadmod.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2404 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flloadmodpkg.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1335 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flmodules.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2010 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flmrproper.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2334 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flreinit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2771 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flreloadbatch.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flreloadlast.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2194 2019-10-02 12:19:59.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flusers.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    35029 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/terminal.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      638 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/unlock.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2635 2019-10-01 07:14:24.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2019-09-30 08:28:48.000000 pineboo-0.99.80.2/pineboolib/core/images/icons/zoom.png
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.079133 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-09-17 09:33:15.000000 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    72306 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/dbadmin240.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   187209 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/dbadmin480.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    71281 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/quick240.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   185547 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/quick480.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       52 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/readme
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    66162 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/splash.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   109093 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/core/images/splashscreen/splash.svg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1174 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/core/message_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4334 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/core/settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      426 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/core/system.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.079133 pineboo-0.99.80.2/pineboolib/core/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-09-21 07:02:47.000000 pineboo-0.99.80.2/pineboolib/core/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1215 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/core/test/test_settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      211 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/core/translate.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.079133 pineboo-0.99.80.2/pineboolib/core/utils/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      114 2019-07-28 13:56:09.000000 pineboo-0.99.80.2/pineboolib/core/utils/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3200 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/core/utils/check_dependencies.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3160 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/core/utils/logging.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      540 2019-07-28 13:56:09.000000 pineboo-0.99.80.2/pineboolib/core/utils/singleton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3720 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/core/utils/struct.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.079133 pineboo-0.99.80.2/pineboolib/core/utils/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       46 2019-08-04 20:13:49.000000 pineboo-0.99.80.2/pineboolib/core/utils/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2331 2020-03-09 12:29:25.000000 pineboo-0.99.80.2/pineboolib/core/utils/tests/test_utils_base.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1819 2020-09-21 06:32:29.000000 pineboo-0.99.80.2/pineboolib/core/utils/tests/test_version.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16422 2023-11-20 09:19:51.000000 pineboo-0.99.80.2/pineboolib/core/utils/utils_base.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4686 2021-03-08 21:10:30.000000 pineboo-0.99.80.2/pineboolib/core/utils/version.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/fllegacy/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      111 2019-07-31 21:01:09.000000 pineboo-0.99.80.2/pineboolib/fllegacy/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       77 2019-07-31 16:14:18.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      349 2019-11-28 09:34:37.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqboolflagstate.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      580 2020-11-10 11:32:00.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqformdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1011 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13443 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqods.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6876 2023-08-17 08:08:02.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      521 2020-03-09 11:54:38.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2019-07-31 20:16:08.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsettings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      337 2019-11-18 12:56:58.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqshttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsignalmapper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      241 2019-07-31 20:16:08.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsmtpclient.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1531 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18185 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      273 2019-11-28 09:34:37.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      255 2019-07-31 20:16:08.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      734 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqssproject.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      343 2020-09-14 10:30:41.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqutil.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-29 15:57:47.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1322 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1201 2020-12-01 12:01:57.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1907 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      554 2020-04-21 15:32:44.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1194 2020-08-07 17:51:40.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      953 2020-02-11 09:11:31.000000 pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      358 2019-09-19 09:51:37.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      171 2020-04-02 16:10:18.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flapplication.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      470 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flcheckbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12410 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flcodbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29392 2023-08-17 09:13:19.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fldatatable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fldateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2384 2023-08-17 07:43:27.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fldoublevalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2020-08-24 08:14:25.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flfastcgi.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   143432 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31681 2023-08-17 07:18:28.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flformdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    35199 2023-11-16 08:49:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flformrecorddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14278 2023-08-16 10:42:25.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flformsearchdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      185 2019-08-01 06:59:07.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flgroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1412 2023-08-17 08:33:39.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flintvalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fljasperengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      103 2020-08-19 14:34:59.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fljasperviewer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5795 2023-08-17 09:13:18.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fllineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3962 2023-08-17 08:30:02.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fllistviewitem.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    52920 2023-10-17 07:18:36.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29028 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flmanagermodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4432 2023-08-17 08:36:14.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flnetwork.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      196 2019-08-17 07:43:18.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4375 2023-08-17 09:13:18.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flpixmapview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3702 2020-08-24 09:53:53.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flposprinter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13936 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flreportengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22351 2023-11-20 09:19:51.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flreportviewer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      403 2019-11-14 09:39:09.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flscripteditor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5223 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flserialport.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1620 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flsettings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13515 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flsmtpclient.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      895 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flspinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      267 2020-03-05 11:36:30.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flsqlconnections.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2019-08-17 07:43:18.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2019-08-17 07:43:18.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fltable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   108699 2023-11-15 11:07:06.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      875 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fltimeedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1147 2023-08-17 08:31:41.000000 pineboo-0.99.80.2/pineboolib/fllegacy/fluintvalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    41266 2023-11-20 09:19:51.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1876 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flvar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      549 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      315 2019-08-13 07:00:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/flworkspace.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/fllegacy/forms/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    48049 2020-12-24 07:51:30.000000 pineboo-0.99.80.2/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       67 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/forms/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67557 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/fllegacy/systype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/fllegacy/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2019-12-02 11:03:25.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1455 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flcodbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1664 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_fldatatable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      991 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_fldateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8854 2023-08-16 09:53:04.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      939 2020-09-21 06:32:29.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flform.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2286 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flformrecorddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3065 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flformsearch.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2288 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      902 2020-12-22 09:37:36.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flreportengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12452 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8666 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1592 2020-09-01 07:21:14.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-09-01 07:21:14.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_smtp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8560 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_systype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/interfaces/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      331 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/interfaces/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      172 2019-07-31 18:05:01.000000 pineboo-0.99.80.2/pineboolib/interfaces/cursoraccessmode.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      228 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/interfaces/dgi_schema.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10877 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/interfaces/iconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5925 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/interfaces/ifieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2999 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/interfaces/imainwindow.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5542 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/interfaces/imanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      166 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/interfaces/isession.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    23002 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/interfaces/isqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50195 2023-10-04 10:16:22.000000 pineboo-0.99.80.2/pineboolib/interfaces/isqldriver.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3292 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/interfaces/itablemetadata.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/loader/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       92 2019-08-04 07:50:46.000000 pineboo-0.99.80.2/pineboolib/loader/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/loader/connection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1546 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/loader/dgi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/loader/dlgconnect/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      104 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/loader/dlgconnect/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      716 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/loader/dlgconnect/conn_dialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15893 2023-08-17 09:07:52.000000 pineboo-0.99.80.2/pineboolib/loader/dlgconnect/dlgconnect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24027 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/loader/dlgconnect/dlgconnect.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/loader/dlgconnect/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       57 2020-12-02 18:09:30.000000 pineboo-0.99.80.2/pineboolib/loader/dlgconnect/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2544 2020-11-09 16:02:09.000000 pineboo-0.99.80.2/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2870 2023-04-20 16:01:15.000000 pineboo-0.99.80.2/pineboolib/loader/init_project.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18643 2023-10-16 10:12:36.000000 pineboo-0.99.80.2/pineboolib/loader/main.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5952 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/loader/options.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1337 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/loader/preload.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17570 2023-10-16 08:53:07.000000 pineboo-0.99.80.2/pineboolib/loader/projectconfig.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/loader/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      477 2019-08-05 15:23:25.000000 pineboo-0.99.80.2/pineboolib/loader/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2495 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/loader/tests/test_connection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      827 2021-03-08 11:35:13.000000 pineboo-0.99.80.2/pineboolib/loader/tests/test_main.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/loader/tests/test_projectconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3682 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/loader/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/plugins/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       23 2019-08-18 15:38:56.000000 pineboo-0.99.80.2/pineboolib/plugins/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/plugins/custom_widgets/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      282 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/custom_widgets/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/custom_widgets/flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/custom_widgets/fltable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/custom_widgets/fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/custom_widgets/pncore.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/plugins/dgi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       19 2019-08-18 15:38:56.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_fcgi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-08-18 15:38:56.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_fcgi/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2848 2020-03-24 12:23:10.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-18 15:38:56.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2019-08-18 15:38:56.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-08-18 15:38:56.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2045 2023-08-16 10:03:48.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9496 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2189 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1483 2023-08-16 10:04:21.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      604 2020-04-02 16:10:18.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4643 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5507 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_schema.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.083133 pineboo-0.99.80.2/pineboolib/plugins/mainform/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      177 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       78 2019-07-30 09:20:57.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    56326 2023-08-16 10:28:14.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/eneboo.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4184 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/mainform.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-11-04 08:30:07.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5084 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       82 2019-07-30 09:20:57.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50084 2023-08-17 09:13:21.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1500 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      280 2019-11-04 08:30:07.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3263 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/plugins/sql/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-18 13:55:56.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      483 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/flmysql_innodb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12048 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/flmysql_myisam.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11801 2023-09-15 14:57:55.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/flpymssql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      825 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/flpyodbc.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13364 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/flqpsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11334 2023-10-17 07:17:48.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/flsqlite.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       31 2020-09-17 10:11:16.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2172 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flmysql_innodb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2958 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flmysql_myisam.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2861 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flpymssql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flpyodbc.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4517 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flsqlite.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2095 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_qpsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9177 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_stress.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2019-07-27 10:21:43.000000 pineboo-0.99.80.2/pineboolib/py.typed
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/q3widgets/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       94 2019-09-27 15:43:59.000000 pineboo-0.99.80.2/pineboolib/q3widgets/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1761 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/checkbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      142 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/combobox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1398 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/dateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3877 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/dialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1634 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/filedialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      511 2023-08-17 08:14:17.000000 pineboo-0.99.80.2/pineboolib/q3widgets/groupbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      118 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/line.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1061 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/lineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3582 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/q3widgets/messagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2758 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/numberedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      443 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/picture.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      134 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/pixmap.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1109 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      907 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1541 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qbytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      774 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qcheckbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2271 2023-08-17 09:13:18.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qcombobox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qdataview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2262 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qdateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      147 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qdatetime.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1663 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qdialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      237 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      316 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qeventloop.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1138 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qframe.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3414 2023-08-17 09:13:18.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qgroupbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      656 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qhboxlayout.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qhbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17373 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qhttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      231 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qiconset.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2088 2023-08-17 08:34:53.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qlabel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      144 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qlayoutwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1099 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qline.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1767 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qlineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5749 2023-08-17 09:13:18.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qlistview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      173 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qlistviewwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      445 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qmainwindow.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      137 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qmenu.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qmessagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1783 2023-08-17 09:08:20.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qobject.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qpopupmenu.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3175 2023-08-17 09:13:18.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qpushbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1975 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qradiobutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      149 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qspinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12827 2023-08-17 09:11:08.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qtable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1770 2023-08-17 08:35:39.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qtabwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2050 2023-08-17 09:13:16.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qtextedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      492 2023-08-17 08:36:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qtextstream.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      926 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qtimeedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      404 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qtoolbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2255 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qtoolbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      654 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qvboxlayout.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qvbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1231 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/qwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      184 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/radiobutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/rect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/size.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/spinbox.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/q3widgets/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      278 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      470 2019-12-19 10:11:59.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_dateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1411 2020-12-02 18:08:18.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_messagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qbytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2637 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qhttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      719 2019-09-27 15:43:59.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qpushbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1163 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qradiobuttons.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1131 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qtabwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1046 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qtextstream.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      532 2020-09-21 08:32:33.000000 pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_spinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/textedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/q3widgets/timeedit.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.087133 pineboo-0.99.80.2/pineboolib/qsa/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       95 2019-08-02 07:28:39.000000 pineboo-0.99.80.2/pineboolib/qsa/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6015 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/qsa/decorators.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1321 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/qsa/emptyscript.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7500 2023-08-17 07:22:45.000000 pineboo-0.99.80.2/pineboolib/qsa/formdbwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2035 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/qsa/input.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1439 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/qsa/object_class.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11935 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/qsa/pncontrolsfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8401 2023-05-11 11:47:21.000000 pineboo-0.99.80.2/pineboolib/qsa/qsa.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pineboolib/qsa/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      496 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/qsa/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      744 2020-06-22 11:35:54.000000 pineboo-0.99.80.2/pineboolib/qsa/tests/test_class.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4169 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/qsa/tests/test_classes.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17795 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/qsa/tests/test_knownbugs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6514 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/qsa/tests/test_orm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1563 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/qsa/tests/test_query_values.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1716 2023-05-01 18:19:33.000000 pineboo-0.99.80.2/pineboolib/qsa/tests/test_require.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7948 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/qsa/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20641 2023-11-20 09:19:51.000000 pineboo-0.99.80.2/pineboolib/qsa/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pineboolib/system_module/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/system_module/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pineboolib/system_module/forms/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9153 2019-09-30 08:28:05.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/FLWidgetMasterTable.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28933 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/ebcomportamiento.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1368 2019-10-01 07:14:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/flareas.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2994 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/flfiles.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8007 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/flgroups.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16760 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/flmodulos.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3150 2020-07-06 10:29:58.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/fltest.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1214 2019-10-01 07:14:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/flusers.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8877 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/master.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10189 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/master_copy.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9932 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/master_print.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11619 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/master_print_copy.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11760 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/forms/sys.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pineboolib/system_module/models/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2020-04-27 09:01:43.000000 pineboo-0.99.80.2/pineboolib/system_module/models/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1466 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flareas_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3206 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flfiles_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1238 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flgroups_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/fllarge_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1313 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flmetadata_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3321 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flmodules_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1292 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flseqs_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1007 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flserial_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1023 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flsettings_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2369 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/fltest2_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1769 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/models/fltest3_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1859 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/fltest4_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2296 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/models/fltest5_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2659 2020-10-13 15:24:00.000000 pineboo-0.99.80.2/pineboolib/system_module/models/fltest_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3548 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flupdates_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1450 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flusers_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1718 2020-07-16 10:23:10.000000 pineboo-0.99.80.2/pineboolib/system_module/models/flvar_model.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pineboolib/system_module/queries/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-09-17 09:33:15.000000 pineboo-0.99.80.2/pineboolib/system_module/queries/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      636 2020-10-15 10:53:48.000000 pineboo-0.99.80.2/pineboolib/system_module/queries/fltest2.qry
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pineboolib/system_module/scripts/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15257 2023-10-16 09:52:50.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/ebcomportamiento.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      234 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/fldumpdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      859 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flfiles.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flloadmod.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      246 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flloadmodpkg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      427 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flmasterareas.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20707 2023-08-16 10:02:26.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flmodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flmrproper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      238 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flreinit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3958 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flreloadbatch.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6037 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/flreloadlast.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/fltest6.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4414 2023-12-20 10:58:37.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/sys.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-03-26 18:29:13.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1104 2020-09-17 09:48:31.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1783 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flfiles.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2020-09-09 10:25:36.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4232 2023-07-17 11:03:23.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flmodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      843 2020-09-09 10:25:36.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flmrproper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      851 2020-09-09 10:25:36.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flreinit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4322 2023-07-17 11:02:35.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_reload_last.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1564 2019-09-26 11:40:44.000000 pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_sys.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2411 2020-12-05 19:13:31.000000 pineboo-0.99.80.2/pineboolib/system_module/sys.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6505 2019-08-23 10:35:06.000000 pineboo-0.99.80.2/pineboolib/system_module/sys.xpm
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pineboolib/system_module/translations/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-09-17 09:33:15.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-01-08 11:17:16.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/sys.ca.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-01-08 11:17:18.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/sys.de.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-01-08 11:17:15.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/sys.en.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    68139 2024-01-08 11:17:15.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/sys.es.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-01-08 11:17:18.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/sys.fr.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-01-08 11:17:19.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/sys.gl.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-01-08 11:17:20.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/sys.it.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-01-08 11:17:21.000000 pineboo-0.99.80.2/pineboolib/system_module/translations/sys.pt.ts
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/pymodules/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2020-11-25 08:02:11.000000 pineboo-0.99.80.2/pymodules/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      283 2024-01-08 11:17:22.091133 pineboo-0.99.80.2/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4087 2023-10-17 07:12:42.000000 pineboo-0.99.80.2/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1078 2019-07-27 10:21:43.000000 pineboo-0.99.81/LICENSE.mit
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7059 2024-04-03 08:18:28.112735 pineboo-0.99.81/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4639 2023-10-17 07:14:02.000000 pineboo-0.99.81/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/pineboo.egg-info/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7059 2024-04-03 08:18:28.000000 pineboo-0.99.81/pineboo.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28782 2024-04-03 08:18:28.000000 pineboo-0.99.81/pineboo.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2024-04-03 08:18:28.000000 pineboo-0.99.81/pineboo.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      386 2024-04-03 08:18:28.000000 pineboo-0.99.81/pineboo.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      584 2024-04-03 08:18:28.000000 pineboo-0.99.81/pineboo.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2024-04-03 08:18:28.000000 pineboo-0.99.81/pineboo.egg-info/top_level.txt
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      179 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1610 2024-04-03 08:15:45.000000 pineboo-0.99.81/pineboolib/application/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/acls/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       20 2019-09-08 08:23:19.000000 pineboo-0.99.81/pineboolib/application/acls/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9234 2023-11-15 10:12:11.000000 pineboo-0.99.81/pineboolib/application/acls/pnaccesscontrol.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7410 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/acls/pnaccesscontrolfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9987 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/application/acls/pnaccesscontrollists.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1554 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/acls/pnboolflagstate.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/acls/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      269 2020-08-26 10:35:25.000000 pineboo-0.99.81/pineboolib/application/acls/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24548 2023-08-17 09:18:35.000000 pineboo-0.99.81/pineboolib/application/acls/tests/test_acls.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      970 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/acls/tests/test_pnaccesscontrol.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9011 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/connections.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/database/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      210 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/database/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/database/orm/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       43 2020-05-06 20:13:13.000000 pineboo-0.99.81/pineboolib/application/database/orm/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5019 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/database/orm/alembic_tools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    38146 2023-10-16 09:53:27.000000 pineboo-0.99.81/pineboolib/application/database/orm/basemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6346 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/database/orm/dummy_cursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1083 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/database/orm/dummy_signal.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/database/orm/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-06-24 11:26:48.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11925 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_basemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2499 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_bytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4086 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_consistency.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3575 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_dummycursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3980 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_query_orm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3395 2023-12-20 10:51:37.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_relationships.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5463 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_sessions.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4744 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_signals.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2509 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_thread_session.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1689 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1080 2020-10-15 10:56:54.000000 pineboo-0.99.81/pineboolib/application/database/orm/tests/test_view.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11303 2023-11-20 09:19:51.000000 pineboo-0.99.81/pineboolib/application/database/orm/utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8356 2023-10-04 10:16:55.000000 pineboo-0.99.81/pineboolib/application/database/pnbuffer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20954 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/pnconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17308 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/pnconnectionmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    40438 2023-11-15 10:12:11.000000 pineboo-0.99.81/pineboolib/application/database/pncursortablemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2020-06-29 10:01:24.000000 pineboo-0.99.81/pineboolib/application/database/pngroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2020-01-10 07:21:12.000000 pineboo-0.99.81/pineboolib/application/database/pnparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1340 2021-03-09 11:41:24.000000 pineboo-0.99.81/pineboolib/application/database/pnsignals.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   123561 2024-04-03 07:34:55.000000 pineboo-0.99.81/pineboolib/application/database/pnsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5770 2023-04-18 17:17:33.000000 pineboo-0.99.81/pineboolib/application/database/pnsqldriversmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    30622 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/application/database/pnsqlquery.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/database/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-12-02 11:03:25.000000 pineboo-0.99.81/pineboolib/application/database/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5985 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pnbuffer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9972 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pnconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4011 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pnconnection_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8048 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pncursortablemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      413 2019-08-28 09:29:35.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pngroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      600 2019-08-28 09:29:35.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pnparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44587 2024-04-03 08:14:34.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pnsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1170 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pnsqldriversmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28220 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_pnsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3475 2023-10-04 10:16:36.000000 pineboo-0.99.81/pineboolib/application/database/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16052 2023-10-16 09:39:59.000000 pineboo-0.99.81/pineboolib/application/database/utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1475 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/file.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11533 2023-11-20 09:19:51.000000 pineboo-0.99.81/pineboolib/application/load_script.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/metadata/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      166 2019-07-30 14:11:28.000000 pineboo-0.99.81/pineboolib/application/metadata/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4940 2023-11-15 10:12:11.000000 pineboo-0.99.81/pineboolib/application/metadata/pnaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2345 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/metadata/pncompoundkeymetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    33256 2023-11-15 10:12:11.000000 pineboo-0.99.81/pineboolib/application/metadata/pnfieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7344 2023-11-15 10:12:11.000000 pineboo-0.99.81/pineboolib/application/metadata/pnrelationmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26029 2024-01-08 11:54:33.000000 pineboo-0.99.81/pineboolib/application/metadata/pntablemetadata.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/metadata/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-03 08:33:48.000000 pineboo-0.99.81/pineboolib/application/metadata/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1217 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/metadata/tests/test_pnaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2311 2020-02-05 09:39:18.000000 pineboo-0.99.81/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16131 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/metadata/tests/test_pnfieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4190 2021-08-23 10:27:07.000000 pineboo-0.99.81/pineboolib/application/metadata/tests/test_pnrelationmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7571 2024-01-08 11:13:46.000000 pineboo-0.99.81/pineboolib/application/metadata/tests/test_pntablemetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2862 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/module.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4141 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/moduleactions.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       47 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/modules_tree.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.072735 pineboo-0.99.81/pineboolib/application/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      122 2019-07-31 07:36:22.000000 pineboo-0.99.81/pineboolib/application/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10703 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/packager/pnpackager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1947 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/packager/pnunpacker.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/packager/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-01-21 10:44:31.000000 pineboo-0.99.81/pineboolib/application/packager/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1763 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/packager/tests/test_pnpackager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1519 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/packager/tests/test_pnunpaker.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       70 2019-07-29 14:08:13.000000 pineboo-0.99.81/pineboolib/application/parsers/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/parser_kut/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       56 2020-04-23 09:34:52.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_kut/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15166 2023-11-20 09:19:51.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_kut/kparsertools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44121 2023-11-20 09:19:51.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_kut/kut2fpdf.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/parser_kut/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      291 2020-04-23 09:34:52.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_kut/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10581 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       50 2020-04-23 09:34:52.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14321 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/pnmtdparser.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5416 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-04-23 09:34:52.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1884 2023-12-20 10:52:15.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      168 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      587 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/flex.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31605 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/flscriptparse.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3400 2020-04-23 09:34:52.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/lextab.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28374 2023-05-17 09:53:26.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/postparse.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8675 2023-05-01 18:19:35.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/pyconvert.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    94792 2023-11-15 10:12:11.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/pytnyzer.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      502 2020-04-23 09:34:52.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17353 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6174 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/token_rules.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/parser_ui/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      101 2020-04-23 09:34:52.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_ui/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50214 2023-10-16 10:19:24.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_ui/qt3ui.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/parsers/parser_ui/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       33 2020-04-23 09:34:52.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_ui/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    34853 2023-08-17 07:11:55.000000 pineboo-0.99.81/pineboolib/application/pnapplication.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      371 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/pncore.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6780 2023-08-17 08:09:49.000000 pineboo-0.99.81/pineboolib/application/process.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26571 2023-09-19 10:18:34.000000 pineboo-0.99.81/pineboolib/application/projectmodule.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3677 2023-09-05 10:16:39.000000 pineboo-0.99.81/pineboolib/application/proxy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6901 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/qsadictmodules.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/qsatypes/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-08-01 20:49:12.000000 pineboo-0.99.81/pineboolib/application/qsatypes/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7972 2023-12-20 09:42:37.000000 pineboo-0.99.81/pineboolib/application/qsatypes/date.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20102 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/qsatypes/sysbasetype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/qsatypes/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-06 06:55:22.000000 pineboo-0.99.81/pineboolib/application/qsatypes/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1882 2023-12-20 14:51:09.000000 pineboo-0.99.81/pineboolib/application/qsatypes/tests/test_date.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5455 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/qsatypes/tests/test_sysbasetype.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3461 2021-03-29 11:28:24.000000 pineboo-0.99.81/pineboolib/application/safeqsa.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/signatures/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-12-25 17:46:05.000000 pineboo-0.99.81/pineboolib/application/signatures/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6413 2023-10-16 09:40:58.000000 pineboo-0.99.81/pineboolib/application/signatures/pdf_digest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9054 2024-01-02 09:55:33.000000 pineboo-0.99.81/pineboolib/application/signatures/pdf_qr.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/signatures/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      286 2021-01-18 11:51:09.000000 pineboo-0.99.81/pineboolib/application/signatures/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3440 2024-01-02 10:01:45.000000 pineboo-0.99.81/pineboolib/application/signatures/tests/test_signatures.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9484 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/signatures/xml_digest.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/staticloader/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-10-04 20:53:14.000000 pineboo-0.99.81/pineboolib/application/staticloader/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14931 2023-09-05 11:00:22.000000 pineboo-0.99.81/pineboolib/application/staticloader/pnmodulesstaticloader.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/staticloader/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      289 2020-09-07 08:35:55.000000 pineboo-0.99.81/pineboolib/application/staticloader/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2491 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/staticloader/tests/test_static_loader.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/staticloader/ui/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-08-17 12:14:19.000000 pineboo-0.99.81/pineboolib/application/staticloader/ui/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7299 2020-03-10 09:40:23.000000 pineboo-0.99.81/pineboolib/application/staticloader/ui/static_loader.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      287 2019-10-09 06:29:09.000000 pineboo-0.99.81/pineboolib/application/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2020-06-10 19:38:58.000000 pineboo-0.99.81/pineboolib/application/tests/test_application.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1350 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/tests/test_load_script.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1309 2020-09-21 07:02:30.000000 pineboo-0.99.81/pineboolib/application/tests/test_process.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1259 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/tests/test_projectmodule.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2020-09-04 08:27:19.000000 pineboo-0.99.81/pineboolib/application/tests/test_proxy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16925 2023-04-07 15:43:24.000000 pineboo-0.99.81/pineboolib/application/tests/test_types.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1319 2020-09-07 08:35:55.000000 pineboo-0.99.81/pineboolib/application/tests/test_xmlaction.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/translator/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-04-05 08:54:23.000000 pineboo-0.99.81/pineboolib/application/translator/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5429 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/translator/pntranslator.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/translator/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       34 2020-12-01 12:01:44.000000 pineboo-0.99.81/pineboolib/application/translator/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      802 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/translator/test/test_pntranslator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    21647 2023-07-27 08:57:49.000000 pineboo-0.99.81/pineboolib/application/types.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/application/utils/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      182 2019-07-31 08:47:54.000000 pineboo-0.99.81/pineboolib/application/utils/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1548 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/utils/check_dependencies.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2245 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/utils/convert_flaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/utils/date_conversion.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6101 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/utils/flfiles_dir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1120 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/utils/geometry.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1949 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/utils/mobilemode.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2450 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/application/utils/modules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1625 2023-12-20 10:52:04.000000 pineboo-0.99.81/pineboolib/application/utils/path.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4727 2020-11-25 10:48:38.000000 pineboo-0.99.81/pineboolib/application/utils/service.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    23217 2023-11-20 09:30:14.000000 pineboo-0.99.81/pineboolib/application/utils/sql_tools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1307 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/application/utils/xpm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15050 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/application/xmlaction.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/core/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      268 2021-03-29 11:28:24.000000 pineboo-0.99.81/pineboolib/core/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8761 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/core/decorators.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      746 2020-10-16 07:17:25.000000 pineboo-0.99.81/pineboolib/core/exceptions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/core/fonts/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-0.99.81/pineboolib/core/fonts/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/core/fonts/noto_sans/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-03-09 09:55:39.000000 pineboo-0.99.81/pineboolib/core/fonts/noto_sans/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2577 2023-12-20 10:52:30.000000 pineboo-0.99.81/pineboolib/core/garbage_collector.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.076735 pineboo-0.99.81/pineboolib/core/images/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-0.99.81/pineboolib/core/images/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.088735 pineboo-0.99.81/pineboolib/core/images/icono_pi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      960 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Pi-symbol.svg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)  1464366 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi.psd
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)  9487782 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi2.xcf
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   476635 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50853 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi2_256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   147180 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi2_512.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50737 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi_1024.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi_256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29321 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi_512.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-09-17 09:33:15.000000 pineboo-0.99.81/pineboolib/core/images/icono_pi/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.096735 pineboo-0.99.81/pineboolib/core/images/icons/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-0.99.81/pineboolib/core/images/icons/__init__.py
+-rwxrwxr-x   0 aulla     (1000) aulla     (1000)      892 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/about.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1230 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/aboutqt.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      853 2019-10-01 07:14:24.000000 pineboo-0.99.81/pineboolib/core/images/icons/cancel.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/consola.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      669 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/date.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2199 2019-09-30 08:28:48.000000 pineboo-0.99.81/pineboolib/core/images/icons/delete.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2562 2019-10-01 07:14:24.000000 pineboo-0.99.81/pineboolib/core/images/icons/down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2069 2019-09-30 08:28:48.000000 pineboo-0.99.81/pineboolib/core/images/icons/edit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2237 2020-01-15 08:29:51.000000 pineboo-0.99.81/pineboolib/core/images/icons/edit_file.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2020-01-15 08:29:51.000000 pineboo-0.99.81/pineboolib/core/images/icons/edit_file_xml.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      934 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/estilo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      870 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/exit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/flfielddb.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      691 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/fltable-clean.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/fltable-data.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/fltable-filter.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      727 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/fltable-odf.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      459 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/folder.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      615 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/folder_update.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      563 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/font.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-bottom.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-first.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-home.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-jump.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-last.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-next.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-previous.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-top.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/go-up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      601 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-add.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1624 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-bold.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-cancel.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1682 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-clear.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      723 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-copy.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-cut.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2049 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-delete.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2104 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-find-and-replace.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1636 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-find.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1256 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-fullscreen.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-back-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-back-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-forward-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-forward-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-bottom.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-first-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-first-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-last-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-last-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-top.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-home.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-indent-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-indent-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1338 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-italic.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-jump-to-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-jump-to-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-justify-center.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      517 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-justify-fill.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      515 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-justify-left.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-justify-right.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-forward-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-forward-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-next-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-next-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      481 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-pause.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1028 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-play-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-previous-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-previous-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1266 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-record.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-rewind-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-rewind-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-stop.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1008 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-new.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-open.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1027 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-paste.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1719 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-print-preview.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1013 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-print.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1115 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-properties.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1502 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-redo-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-refresh.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      317 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-remove.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1837 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-save-as.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1971 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-save.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      631 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-select-all.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-stop.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1445 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-strikethrough.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-underline.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1601 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-undo-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-unindent-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/gtk-unindent-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      911 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/help_index.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1854 2019-09-30 08:28:48.000000 pineboo-0.99.81/pineboolib/core/images/icons/insert.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      711 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/lock.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      579 2019-10-01 07:14:24.000000 pineboo-0.99.81/pineboolib/core/images/icons/ok.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1997 2019-09-30 08:28:48.000000 pineboo-0.99.81/pineboolib/core/images/icons/paste.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-128.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      857 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-16.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1406 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-24.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1941 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-32.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2991 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-48.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3482 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-57.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3243 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-64.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-72.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19949 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-128.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1216 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-16.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1720 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-24.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    52103 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2568 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-32.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4552 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-48.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7028 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-64.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17588 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-09-30 08:28:48.000000 pineboo-0.99.81/pineboolib/core/images/icons/print.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      885 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/reload.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22869 2022-07-06 21:01:18.000000 pineboo-0.99.81/pineboolib/core/images/icons/signed_stamp.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1930 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_ebcomportamiento.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1571 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flareas.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2952 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_fldumpdb.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1133 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flgroups.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1871 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flloadmod.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2404 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flloadmodpkg.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1335 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flmodules.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2010 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flmrproper.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2334 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flreinit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2771 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flreloadbatch.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flreloadlast.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2194 2019-10-02 12:19:59.000000 pineboo-0.99.81/pineboolib/core/images/icons/sys_flusers.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    35029 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/terminal.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      638 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/icons/unlock.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2635 2019-10-01 07:14:24.000000 pineboo-0.99.81/pineboolib/core/images/icons/up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2019-09-30 08:28:48.000000 pineboo-0.99.81/pineboolib/core/images/icons/zoom.png
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.096735 pineboo-0.99.81/pineboolib/core/images/splashscreen/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-09-17 09:33:15.000000 pineboo-0.99.81/pineboolib/core/images/splashscreen/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    72306 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/splashscreen/dbadmin240.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   187209 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/splashscreen/dbadmin480.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    71281 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/splashscreen/quick240.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   185547 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/splashscreen/quick480.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       52 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/splashscreen/readme
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    66162 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/splashscreen/splash.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   109093 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/core/images/splashscreen/splash.svg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1174 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/core/message_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4334 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/core/settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      426 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/core/system.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.096735 pineboo-0.99.81/pineboolib/core/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-09-21 07:02:47.000000 pineboo-0.99.81/pineboolib/core/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1215 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/core/test/test_settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      211 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/core/translate.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.096735 pineboo-0.99.81/pineboolib/core/utils/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      114 2019-07-28 13:56:09.000000 pineboo-0.99.81/pineboolib/core/utils/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3200 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/core/utils/check_dependencies.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3160 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/core/utils/logging.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      540 2019-07-28 13:56:09.000000 pineboo-0.99.81/pineboolib/core/utils/singleton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3720 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/core/utils/struct.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.096735 pineboo-0.99.81/pineboolib/core/utils/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       46 2019-08-04 20:13:49.000000 pineboo-0.99.81/pineboolib/core/utils/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2331 2020-03-09 12:29:25.000000 pineboo-0.99.81/pineboolib/core/utils/tests/test_utils_base.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1819 2020-09-21 06:32:29.000000 pineboo-0.99.81/pineboolib/core/utils/tests/test_version.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16422 2023-11-20 09:19:51.000000 pineboo-0.99.81/pineboolib/core/utils/utils_base.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4686 2021-03-08 21:10:30.000000 pineboo-0.99.81/pineboolib/core/utils/version.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.100735 pineboo-0.99.81/pineboolib/fllegacy/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      111 2019-07-31 21:01:09.000000 pineboo-0.99.81/pineboolib/fllegacy/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.100735 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       77 2019-07-31 16:14:18.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      349 2019-11-28 09:34:37.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqboolflagstate.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      580 2020-11-10 11:32:00.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqformdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1011 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13443 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqods.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6876 2023-08-17 08:08:02.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      521 2020-03-09 11:54:38.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2019-07-31 20:16:08.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsettings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      337 2019-11-18 12:56:58.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqshttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsignalmapper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      241 2019-07-31 20:16:08.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsmtpclient.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1531 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18185 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      273 2019-11-28 09:34:37.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      255 2019-07-31 20:16:08.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      734 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqssproject.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      343 2020-09-14 10:30:41.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqutil.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.100735 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-29 15:57:47.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1322 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1201 2020-12-01 12:01:57.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1907 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      554 2020-04-21 15:32:44.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1194 2020-08-07 17:51:40.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      953 2020-02-11 09:11:31.000000 pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      358 2019-09-19 09:51:37.000000 pineboo-0.99.81/pineboolib/fllegacy/flaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      171 2020-04-02 16:10:18.000000 pineboo-0.99.81/pineboolib/fllegacy/flapplication.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      470 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/fllegacy/flcheckbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12410 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/fllegacy/flcodbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29392 2023-08-17 09:13:19.000000 pineboo-0.99.81/pineboolib/fllegacy/fldatatable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/fldateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2384 2023-08-17 07:43:27.000000 pineboo-0.99.81/pineboolib/fllegacy/fldoublevalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2020-08-24 08:14:25.000000 pineboo-0.99.81/pineboolib/fllegacy/flfastcgi.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   143432 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/fllegacy/flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31681 2023-08-17 07:18:28.000000 pineboo-0.99.81/pineboolib/fllegacy/flformdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    35199 2023-11-16 08:49:24.000000 pineboo-0.99.81/pineboolib/fllegacy/flformrecorddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14278 2023-08-16 10:42:25.000000 pineboo-0.99.81/pineboolib/fllegacy/flformsearchdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      185 2019-08-01 06:59:07.000000 pineboo-0.99.81/pineboolib/fllegacy/flgroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1412 2023-08-17 08:33:39.000000 pineboo-0.99.81/pineboolib/fllegacy/flintvalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/fljasperengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      103 2020-08-19 14:34:59.000000 pineboo-0.99.81/pineboolib/fllegacy/fljasperviewer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5795 2023-08-17 09:13:18.000000 pineboo-0.99.81/pineboolib/fllegacy/fllineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3962 2023-08-17 08:30:02.000000 pineboo-0.99.81/pineboolib/fllegacy/fllistviewitem.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    52920 2023-10-17 07:18:36.000000 pineboo-0.99.81/pineboolib/fllegacy/flmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29028 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/fllegacy/flmanagermodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4432 2023-08-17 08:36:14.000000 pineboo-0.99.81/pineboolib/fllegacy/flnetwork.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      196 2019-08-17 07:43:18.000000 pineboo-0.99.81/pineboolib/fllegacy/flparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4375 2023-08-17 09:13:18.000000 pineboo-0.99.81/pineboolib/fllegacy/flpixmapview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3702 2020-08-24 09:53:53.000000 pineboo-0.99.81/pineboolib/fllegacy/flposprinter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13936 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/fllegacy/flreportengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22351 2023-11-20 09:19:51.000000 pineboo-0.99.81/pineboolib/fllegacy/flreportviewer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      403 2019-11-14 09:39:09.000000 pineboo-0.99.81/pineboolib/fllegacy/flscripteditor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5223 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/fllegacy/flserialport.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1620 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/flsettings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13515 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/flsmtpclient.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      895 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/flspinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      267 2020-03-05 11:36:30.000000 pineboo-0.99.81/pineboolib/fllegacy/flsqlconnections.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2019-08-17 07:43:18.000000 pineboo-0.99.81/pineboolib/fllegacy/flsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2019-08-17 07:43:18.000000 pineboo-0.99.81/pineboolib/fllegacy/flsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/fltable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   108699 2023-11-15 11:07:06.000000 pineboo-0.99.81/pineboolib/fllegacy/fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      875 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/fltimeedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1147 2023-08-17 08:31:41.000000 pineboo-0.99.81/pineboolib/fllegacy/fluintvalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    41266 2023-11-20 09:19:51.000000 pineboo-0.99.81/pineboolib/fllegacy/flutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1876 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/fllegacy/flvar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      549 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/flwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      315 2019-08-13 07:00:24.000000 pineboo-0.99.81/pineboolib/fllegacy/flworkspace.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.100735 pineboo-0.99.81/pineboolib/fllegacy/forms/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    48049 2020-12-24 07:51:30.000000 pineboo-0.99.81/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       67 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/forms/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67557 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/fllegacy/systype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.100735 pineboo-0.99.81/pineboolib/fllegacy/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2019-12-02 11:03:25.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1455 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_flcodbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1664 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_fldatatable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      991 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_fldateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8854 2023-08-16 09:53:04.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      939 2020-09-21 06:32:29.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_flform.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2286 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_flformrecorddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3065 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_flformsearch.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2288 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_flmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      902 2020-12-22 09:37:36.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_flreportengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12452 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8666 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_flutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1592 2020-09-01 07:21:14.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-09-01 07:21:14.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_smtp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8560 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/fllegacy/tests/test_systype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.100735 pineboo-0.99.81/pineboolib/interfaces/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      331 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/interfaces/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      172 2019-07-31 18:05:01.000000 pineboo-0.99.81/pineboolib/interfaces/cursoraccessmode.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      228 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/interfaces/dgi_schema.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10877 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/interfaces/iconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5925 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/interfaces/ifieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2999 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/interfaces/imainwindow.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5542 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/interfaces/imanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      166 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/interfaces/isession.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    23002 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/interfaces/isqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50195 2023-10-04 10:16:22.000000 pineboo-0.99.81/pineboolib/interfaces/isqldriver.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3292 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/interfaces/itablemetadata.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.100735 pineboo-0.99.81/pineboolib/loader/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       92 2019-08-04 07:50:46.000000 pineboo-0.99.81/pineboolib/loader/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/loader/connection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1546 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/loader/dgi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/loader/dlgconnect/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      104 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/loader/dlgconnect/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      716 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/loader/dlgconnect/conn_dialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15893 2023-08-17 09:07:52.000000 pineboo-0.99.81/pineboolib/loader/dlgconnect/dlgconnect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24027 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/loader/dlgconnect/dlgconnect.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/loader/dlgconnect/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       57 2020-12-02 18:09:30.000000 pineboo-0.99.81/pineboolib/loader/dlgconnect/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2544 2020-11-09 16:02:09.000000 pineboo-0.99.81/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2870 2023-04-20 16:01:15.000000 pineboo-0.99.81/pineboolib/loader/init_project.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18643 2023-10-16 10:12:36.000000 pineboo-0.99.81/pineboolib/loader/main.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5952 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/loader/options.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1337 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/loader/preload.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17570 2023-10-16 08:53:07.000000 pineboo-0.99.81/pineboolib/loader/projectconfig.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/loader/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      477 2019-08-05 15:23:25.000000 pineboo-0.99.81/pineboolib/loader/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2495 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/loader/tests/test_connection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      827 2021-03-08 11:35:13.000000 pineboo-0.99.81/pineboolib/loader/tests/test_main.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/loader/tests/test_projectconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3682 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/loader/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       23 2019-08-18 15:38:56.000000 pineboo-0.99.81/pineboolib/plugins/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/custom_widgets/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      282 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/custom_widgets/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/custom_widgets/flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/custom_widgets/fltable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/custom_widgets/fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/custom_widgets/pncore.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/dgi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       19 2019-08-18 15:38:56.000000 pineboo-0.99.81/pineboolib/plugins/dgi/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_fcgi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-08-18 15:38:56.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_fcgi/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2848 2020-03-24 12:23:10.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-18 15:38:56.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2019-08-18 15:38:56.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-08-18 15:38:56.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2045 2023-08-16 10:03:48.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9496 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2189 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1483 2023-08-16 10:04:21.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      604 2020-04-02 16:10:18.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4643 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5507 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/dgi/dgi_schema.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/mainform/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      177 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/mainform/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       78 2019-07-30 09:20:57.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    56326 2023-08-16 10:28:14.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/eneboo.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4184 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/mainform.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-11-04 08:30:07.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5084 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       82 2019-07-30 09:20:57.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50084 2023-08-17 09:13:21.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1500 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      280 2019-11-04 08:30:07.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3263 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/sql/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-18 13:55:56.000000 pineboo-0.99.81/pineboolib/plugins/sql/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      483 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/flmysql_innodb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12048 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/plugins/sql/flmysql_myisam.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11801 2023-09-15 14:57:55.000000 pineboo-0.99.81/pineboolib/plugins/sql/flpymssql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      825 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/flpyodbc.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13364 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/plugins/sql/flqpsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11334 2023-10-17 07:17:48.000000 pineboo-0.99.81/pineboolib/plugins/sql/flsqlite.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.104735 pineboo-0.99.81/pineboolib/plugins/sql/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       31 2020-09-17 10:11:16.000000 pineboo-0.99.81/pineboolib/plugins/sql/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2172 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flmysql_innodb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2958 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flmysql_myisam.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2861 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flpymssql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flpyodbc.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4517 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flsqlite.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2095 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/tests/test_qpsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9177 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/plugins/sql/tests/test_stress.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2019-07-27 10:21:43.000000 pineboo-0.99.81/pineboolib/py.typed
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.108735 pineboo-0.99.81/pineboolib/q3widgets/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       94 2019-09-27 15:43:59.000000 pineboo-0.99.81/pineboolib/q3widgets/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1761 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/checkbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      142 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/combobox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1398 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/dateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3877 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/dialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1634 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/filedialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      511 2023-08-17 08:14:17.000000 pineboo-0.99.81/pineboolib/q3widgets/groupbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      118 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/line.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1061 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/lineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3582 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/q3widgets/messagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2758 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/numberedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      443 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/picture.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      134 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/pixmap.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1109 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      907 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/q3widgets/qbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1541 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qbytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      774 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qcheckbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2271 2023-08-17 09:13:18.000000 pineboo-0.99.81/pineboolib/q3widgets/qcombobox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qdataview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2262 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qdateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      147 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qdatetime.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1663 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qdialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      237 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      316 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qeventloop.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1138 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qframe.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3414 2023-08-17 09:13:18.000000 pineboo-0.99.81/pineboolib/q3widgets/qgroupbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      656 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qhboxlayout.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qhbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17373 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/q3widgets/qhttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      231 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qiconset.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2088 2023-08-17 08:34:53.000000 pineboo-0.99.81/pineboolib/q3widgets/qlabel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      144 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qlayoutwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1099 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qline.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1767 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qlineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5749 2023-08-17 09:13:18.000000 pineboo-0.99.81/pineboolib/q3widgets/qlistview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      173 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qlistviewwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      445 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qmainwindow.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      137 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qmenu.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qmessagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1783 2023-08-17 09:08:20.000000 pineboo-0.99.81/pineboolib/q3widgets/qobject.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qpopupmenu.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3175 2023-08-17 09:13:18.000000 pineboo-0.99.81/pineboolib/q3widgets/qpushbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1975 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qradiobutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      149 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qspinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12827 2023-08-17 09:11:08.000000 pineboo-0.99.81/pineboolib/q3widgets/qtable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1770 2023-08-17 08:35:39.000000 pineboo-0.99.81/pineboolib/q3widgets/qtabwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2050 2023-08-17 09:13:16.000000 pineboo-0.99.81/pineboolib/q3widgets/qtextedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      492 2023-08-17 08:36:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qtextstream.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      926 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qtimeedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      404 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qtoolbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2255 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qtoolbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      654 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qvboxlayout.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qvbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1231 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/qwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      184 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/radiobutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/rect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/size.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/spinbox.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.108735 pineboo-0.99.81/pineboolib/q3widgets/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      278 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      470 2019-12-19 10:11:59.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_dateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1411 2020-12-02 18:08:18.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_messagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_qbytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2637 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_qhttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      719 2019-09-27 15:43:59.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_qpushbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1163 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_qradiobuttons.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1131 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_qtabwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1046 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_qtextstream.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      532 2020-09-21 08:32:33.000000 pineboo-0.99.81/pineboolib/q3widgets/tests/test_spinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/textedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/q3widgets/timeedit.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.108735 pineboo-0.99.81/pineboolib/qsa/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       95 2019-08-02 07:28:39.000000 pineboo-0.99.81/pineboolib/qsa/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6015 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/qsa/decorators.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1321 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/qsa/emptyscript.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7500 2023-08-17 07:22:45.000000 pineboo-0.99.81/pineboolib/qsa/formdbwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2035 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/qsa/input.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1439 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/qsa/object_class.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11935 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/qsa/pncontrolsfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8401 2023-05-11 11:47:21.000000 pineboo-0.99.81/pineboolib/qsa/qsa.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.108735 pineboo-0.99.81/pineboolib/qsa/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      496 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/qsa/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      744 2020-06-22 11:35:54.000000 pineboo-0.99.81/pineboolib/qsa/tests/test_class.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4169 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/qsa/tests/test_classes.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17795 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/qsa/tests/test_knownbugs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6514 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/qsa/tests/test_orm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1563 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/qsa/tests/test_query_values.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1716 2023-05-01 18:19:33.000000 pineboo-0.99.81/pineboolib/qsa/tests/test_require.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7948 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/qsa/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20641 2023-11-20 09:19:51.000000 pineboo-0.99.81/pineboolib/qsa/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.108735 pineboo-0.99.81/pineboolib/system_module/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/system_module/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/pineboolib/system_module/forms/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9153 2019-09-30 08:28:05.000000 pineboo-0.99.81/pineboolib/system_module/forms/FLWidgetMasterTable.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-0.99.81/pineboolib/system_module/forms/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28933 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/ebcomportamiento.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1368 2019-10-01 07:14:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/flareas.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2994 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/flfiles.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8007 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/flgroups.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16760 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/flmodulos.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3150 2020-07-06 10:29:58.000000 pineboo-0.99.81/pineboolib/system_module/forms/fltest.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1214 2019-10-01 07:14:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/flusers.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8877 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/master.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10189 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/master_copy.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9932 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/master_print.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11619 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/master_print_copy.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11760 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/forms/sys.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/pineboolib/system_module/models/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2020-04-27 09:01:43.000000 pineboo-0.99.81/pineboolib/system_module/models/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1466 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/system_module/models/flareas_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3206 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/system_module/models/flfiles_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1238 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/flgroups_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/fllarge_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1313 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/flmetadata_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3321 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/system_module/models/flmodules_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1292 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/flseqs_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1007 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/flserial_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1023 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/flsettings_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2369 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/fltest2_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1769 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/models/fltest3_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1859 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/fltest4_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2296 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/models/fltest5_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2659 2020-10-13 15:24:00.000000 pineboo-0.99.81/pineboolib/system_module/models/fltest_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3548 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/flupdates_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1450 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/flusers_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1718 2020-07-16 10:23:10.000000 pineboo-0.99.81/pineboolib/system_module/models/flvar_model.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/pineboolib/system_module/queries/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-09-17 09:33:15.000000 pineboo-0.99.81/pineboolib/system_module/queries/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      636 2020-10-15 10:53:48.000000 pineboo-0.99.81/pineboolib/system_module/queries/fltest2.qry
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/pineboolib/system_module/scripts/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/system_module/scripts/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15257 2023-10-16 09:52:50.000000 pineboo-0.99.81/pineboolib/system_module/scripts/ebcomportamiento.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      234 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/fldumpdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      859 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flfiles.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flloadmod.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      246 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flloadmodpkg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      427 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flmasterareas.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20707 2023-08-16 10:02:26.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flmodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flmrproper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      238 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flreinit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3958 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flreloadbatch.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6037 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/system_module/scripts/flreloadlast.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-0.99.81/pineboolib/system_module/scripts/fltest6.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4414 2023-12-20 10:58:37.000000 pineboo-0.99.81/pineboolib/system_module/scripts/sys.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/pineboolib/system_module/scripts/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-03-26 18:29:13.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1104 2020-09-17 09:48:31.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1783 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flfiles.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2020-09-09 10:25:36.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4232 2023-07-17 11:03:23.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flmodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      843 2020-09-09 10:25:36.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flmrproper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      851 2020-09-09 10:25:36.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flreinit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4322 2023-07-17 11:02:35.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_reload_last.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1564 2019-09-26 11:40:44.000000 pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_sys.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2411 2020-12-05 19:13:31.000000 pineboo-0.99.81/pineboolib/system_module/sys.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6505 2019-08-23 10:35:06.000000 pineboo-0.99.81/pineboolib/system_module/sys.xpm
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/pineboolib/system_module/translations/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-09-17 09:33:15.000000 pineboo-0.99.81/pineboolib/system_module/translations/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-04-03 08:18:22.000000 pineboo-0.99.81/pineboolib/system_module/translations/sys.ca.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-04-03 08:18:23.000000 pineboo-0.99.81/pineboolib/system_module/translations/sys.de.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-04-03 08:18:21.000000 pineboo-0.99.81/pineboolib/system_module/translations/sys.en.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    68139 2024-04-03 08:18:20.000000 pineboo-0.99.81/pineboolib/system_module/translations/sys.es.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-04-03 08:18:24.000000 pineboo-0.99.81/pineboolib/system_module/translations/sys.fr.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-04-03 08:18:25.000000 pineboo-0.99.81/pineboolib/system_module/translations/sys.gl.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-04-03 08:18:26.000000 pineboo-0.99.81/pineboolib/system_module/translations/sys.it.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67947 2024-04-03 08:18:27.000000 pineboo-0.99.81/pineboolib/system_module/translations/sys.pt.ts
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2024-04-03 08:18:28.112735 pineboo-0.99.81/pymodules/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2020-11-25 08:02:11.000000 pineboo-0.99.81/pymodules/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      283 2024-04-03 08:18:28.116735 pineboo-0.99.81/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4087 2023-10-17 07:12:42.000000 pineboo-0.99.81/setup.py
```

### Comparing `pineboo-0.99.80.2/LICENSE.mit` & `pineboo-0.99.81/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/PKG-INFO` & `pineboo-0.99.81/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: pineboo
-Version: 0.99.80.2
-Summary: ERP replacement for Eneboo written in Python
-Home-page: https://github.com/deavid/pineboo
-Author: David Martínez Martí, José A. Fernández Fernández
-Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
-Keywords: erp pineboo eneboo accounting sales warehouse
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Environment :: X11 Applications :: Qt
-Classifier: Topic :: Office/Business :: Financial :: Accounting
-Classifier: Typing :: Typed
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Natural Language :: Spanish
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.mit
-
 .. image:: https://gitlab.com/aulla/pineboo/badges/master/pipeline.svg
     :target: https://gitlab.com/aulla/pineboo/commits/master
     :alt: pipeline status
 
 .. image:: https://gitlab.com/aulla/pineboo/badges/master/coverage.svg
     :target: https://gitlab.com/aulla/pineboo/commits/master
     :alt: coverage report
```

### Comparing `pineboo-0.99.80.2/pineboo.egg-info/SOURCES.txt` & `pineboo-0.99.81/pineboo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboo.egg-info/requires.txt` & `pineboo-0.99.81/pineboo.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Pillow==8.2.0
-PyQt6-Qt6==6.5.3
-PyQt6-sip==13.6.0
-PyQt6==6.5.3
-PyYAML==5.3.1
 alembic>=1.7.7
 black==23.11
 clipboard==0.0.4
 coloredlogs==14.0
 cryptography==36.0.1
 fernet==1.0.1
+fpdf2==2.4.2
 flake8==3.9.0
 flup==1.0.3
 fonttools>=4.27.1
-fpdf2==2.4.2
 keyrings.alt>=3.4.0
 lxml==4.9.3
 marshmallow>=3.19.0
 ninja==1.10.0.post1
 odfpy
 pdf2image==1.14.0
 ply==3.11
 poppler-utils
 psycopg2
+pyroma==2.6
+pyfiglet
 pyHanko[opentype]==0.20.1
 pyOpenSSL==20.0.1
-pyfiglet
 pympler
-pyroma==2.6
 python-barcode
 python-daemon
 qrcode[pil]
 sqlalchemy==1.4.49
 sqlparse==0.3.1
 twine==3.1.1
 uharfbuzz>=0.37.3
 watchdog>=0.10.2
 xades==0.2.1
 xmlsig==0.1.7
+Pillow==8.2.0
+PyYAML==5.3.1
+PyQt6==6.5.3
+PyQt6-Qt6==6.5.3
+PyQt6-sip==13.6.0
```

### Comparing `pineboo-0.99.80.2/pineboolib/application/__init__.py` & `pineboo-0.99.81/pineboolib/application/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 PROJECT = Project()
 
 SERIALIZE_LIST: Dict[int, List[str]] = {}
 FILE_CLASSES: Dict[str, str] = {}
 ID_SESSION: str = ""
 
-PINEBOO_VER = "0.99.80.2"
+PINEBOO_VER = "0.99.81"
 
 SHOW_CURSOR_EVENTS: bool = False  # Enable show pnsqlcursor actions debug.
 SHOW_CONNECTION_EVENTS: bool = False  # Enable show debug when connection is closed.
 SHOW_NESTED_WARNING: bool = False  # Enable show nested debug.
 VIRTUAL_DB: bool = True  # Enable :memory: database on pytest.
 LOG_SQL: bool = False  # Enable sqlalchemy logs.
 USE_WEBSOCKET_CHANNEL: bool = False  # Enable websockets features.
```

### Comparing `pineboo-0.99.80.2/pineboolib/application/acls/pnaccesscontrol.py` & `pineboo-0.99.81/pineboolib/application/acls/pnaccesscontrol.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/acls/pnaccesscontrolfactory.py` & `pineboo-0.99.81/pineboolib/application/acls/pnaccesscontrolfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/acls/pnaccesscontrollists.py` & `pineboo-0.99.81/pineboolib/application/acls/pnaccesscontrollists.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/acls/pnboolflagstate.py` & `pineboo-0.99.81/pineboolib/application/acls/pnboolflagstate.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/acls/tests/test_acls.py` & `pineboo-0.99.81/pineboolib/application/acls/tests/test_acls.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/acls/tests/test_pnaccesscontrol.py` & `pineboo-0.99.81/pineboolib/application/acls/tests/test_pnaccesscontrol.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/connections.py` & `pineboo-0.99.81/pineboolib/application/connections.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/alembic_tools.py` & `pineboo-0.99.81/pineboolib/application/database/orm/alembic_tools.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/basemodel.py` & `pineboo-0.99.81/pineboolib/application/database/orm/basemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/dummy_cursor.py` & `pineboo-0.99.81/pineboolib/application/database/orm/dummy_cursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/dummy_signal.py` & `pineboo-0.99.81/pineboolib/application/database/orm/dummy_signal.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_basemodel.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_bytearray.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_bytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_consistency.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_consistency.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_dummycursor.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_dummycursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_query_orm.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_query_orm.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_relationships.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_relationships.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_sessions.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_signals.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_thread_session.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_thread_session.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_utils.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/tests/test_view.py` & `pineboo-0.99.81/pineboolib/application/database/orm/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/orm/utils.py` & `pineboo-0.99.81/pineboolib/application/database/orm/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pnbuffer.py` & `pineboo-0.99.81/pineboolib/application/database/pnbuffer.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pnconnection.py` & `pineboo-0.99.81/pineboolib/application/database/pnconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pnconnectionmanager.py` & `pineboo-0.99.81/pineboolib/application/database/pnconnectionmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pncursortablemodel.py` & `pineboo-0.99.81/pineboolib/application/database/pncursortablemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pngroupbyquery.py` & `pineboo-0.99.81/pineboolib/application/database/pngroupbyquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pnparameterquery.py` & `pineboo-0.99.81/pineboolib/application/database/pnparameterquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pnsignals.py` & `pineboo-0.99.81/pineboolib/application/database/pnsignals.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pnsqlcursor.py` & `pineboo-0.99.81/pineboolib/application/database/pnsqlcursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1127,17 +1127,19 @@
                         #    "SQL linea = %s conn name = %s", qry.sql(), self.connectionName()
                         # )
                         qry.exec_()
                         if not qry.next():
                             LOGGER.warning(
                                 " msgCheckIntegrity. No se encuentra el valor en session: %s, transacción: %s, sql: %s, size: %s",
                                 qry.db().session(),
-                                qry.db().session().get_transaction()  # type: ignore [attr-defined]
-                                if not qry.db().session().in_nested_transaction()  # type: ignore [attr-defined]
-                                else qry.db().session().get_nested_transaction(),  # type: ignore [attr-defined]
+                                (
+                                    qry.db().session().get_transaction()  # type: ignore [attr-defined]
+                                    if not qry.db().session().in_nested_transaction()  # type: ignore [attr-defined]
+                                    else qry.db().session().get_nested_transaction()
+                                ),  # type: ignore [attr-defined]
                                 qry.sql(),
                                 qry.size(),
                             )
                             message += "\n%s:%s : El valor %s no existe en la tabla %s" % (
                                 self.table(),
                                 field.alias(),
                                 value,
@@ -2444,14 +2446,16 @@
             )
             return False
 
         if not self.checkIntegrity():
             log_func("CommitBuffer cancelado. Problema de integridad.")
             return False
 
+        manager = self.db().connManager().manager()
+
         field_name_check = None
         function_before_commit = (
             "beforeCommit_%s" % self.table() if self.activatedCommitActions() else ""
         )
         function_after_commit = (
             "afterCommit_%s" % self.table() if self.activatedCommitActions() else ""
         )
@@ -2593,25 +2597,26 @@
                     continue
 
                 result = self.private_cursor.buffer_.value(  # type: ignore [union-attr] # noqa: F821
                     field_name
                 )
 
                 for relation in field.relationList():
-                    cursor = PNSqlCursor(relation.foreignTable())
-                    foreign_mtd = cursor.private_cursor.metadata_
+                    foreign_mtd = manager.metadata(relation.foreignTable())
                     if foreign_mtd is None:
                         continue
+
                     foreign_field = foreign_mtd.field(relation.foreignField())
                     if foreign_field is None:
                         continue
 
                     relation_m1 = foreign_field.relationM1()
 
                     if relation_m1 and relation_m1.deleteCascade():
+                        cursor = PNSqlCursor(relation.foreignTable())
                         cursor.setForwardOnly(True)
                         cursor.select(
                             self.conn()
                             .connManager()
                             .manager()
                             .formatAssignValue(relation.foreignField(), foreign_field, result, True)
                         )
```

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pnsqldriversmanager.py` & `pineboo-0.99.81/pineboolib/application/database/pnsqldriversmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/pnsqlquery.py` & `pineboo-0.99.81/pineboolib/application/database/pnsqlquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnbuffer.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_pnbuffer.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnconnection.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_pnconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnconnection_manager.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_pnconnection_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_pncursortablemodel.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_pncursortablemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnparameterquery.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_pnparameterquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnsqlcursor.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_pnsqlcursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Test_pnsqlcursor module."""
 
 import unittest
 from pineboolib.loader.main import init_testing, finish_testing
 from pineboolib.core.utils import logging
 from pineboolib.application.database import pnsqlcursor
+from pineboolib.application.metadata import pnrelationmetadata
 from pineboolib import application
 from pineboolib.application.database.tests import fixture_path
 from pineboolib.core.utils import utils_base
 
 LOGGER = logging.get_logger("test")
 
 
@@ -213,37 +214,80 @@
         self.assertEqual(
             pass_, 4, "Solo ha borrado %s registros! %s" % (pass_, ", ".join(borrados))
         )
 
     def test_basic_3(self) -> None:
         """Delete data from a database."""
 
+        # recoger el metadata
+        metadata = application.PROJECT.conn_manager.manager().metadata("flareas")
+        # añadir relación fake
+        relation_meta = pnrelationmetadata.PNRelationMetaData(
+            "fake", "idarea", pnrelationmetadata.PNRelationMetaData.RELATION_1M
+        )
+
         cursor = pnsqlcursor.PNSqlCursor("flareas")
+
+        field = cursor.metadata().field("idarea")
+        field.addRelationMD(relation_meta)
+
+        # comprobar si el cambio es persistente
+
+        metadata_cursor = cursor.metadata()
+        relations = metadata_cursor.field("idarea").relationList()
+        found = False
+        for relation in relations:
+            if relation.foreignTable() == "fake":
+                found = True
+                break
+
+        self.assertTrue(found, "No se encuentra la relacion FAKE")
+
         cursor.setModeAccess(cursor.Insert)
         cursor.refreshBuffer()
         cursor.setValueBuffer("bloqueo", True)
         cursor.setValueBuffer("idarea", "T1")
         cursor.setValueBuffer("descripcion", "Área de prueba T1")
         self.assertTrue(cursor.commitBuffer())
 
-        cursor2 = pnsqlcursor.PNSqlCursor("flmodules")
-        cursor2.setModeAccess(cursor2.Insert)
-        cursor2.refreshBuffer()
-        cursor2.setValueBuffer("idmodulo", "M1")
-        cursor2.setValueBuffer("idarea", "T1")
-        cursor2.setValueBuffer("descripcion", "Módulo T")
-        cursor2.setValueBuffer("version", "0.0")
-        cursor2.commitBuffer()
+        cursor.select("idarea = 'T1'")
+        self.assertTrue(cursor.first())
+        cursor.setModeAccess(cursor.Del)
+        cursor.refreshBuffer()
+        self.assertTrue(cursor.commitBuffer())
 
-        cursor3 = pnsqlcursor.PNSqlCursor("flareas")
-        cursor3.select("idarea = 'T1'")
-        self.assertTrue(cursor3.first())
-        cursor3.setModeAccess(cursor3.Del)
-        cursor3.refreshBuffer()
-        self.assertFalse(cursor3.commitBuffer())
+    def test_basic_4(self) -> None:
+        """Delete with relation errors."""
+        cursor = pnsqlcursor.PNSqlCursor("flareas")
+        cursor.setModeAccess(cursor.Insert)
+        cursor.refreshBuffer()
+        cursor.setValueBuffer("bloqueo", True)
+        cursor.setValueBuffer("idarea", "T")
+        cursor.setValueBuffer("descripcion", "Área de prueba T")
+        self.assertTrue(cursor.commitBuffer())
+
+        cursor.select("idarea ='T'")
+        first_result = cursor.first()
+        self.assertEqual(first_result, True)
+        size_1 = cursor.size()
+        self.assertEqual(size_1, 1, "tiene que devolver 1 y ha devuelto %s" % size_1)
+        cursor.setForwardOnly(True)
+        cursor.setModeAccess(cursor.Del)
+        cursor.refreshBuffer()
+
+        value_idarea = cursor.valueBuffer("idarea")
+        self.assertEqual(value_idarea, "T")
+        cursor.commitBuffer()
+        cursor.refresh()
+        size_2 = cursor.size()
+        self.assertEqual(size_2, 1)
+        cursor.setForwardOnly(False)
+        cursor.refresh()
+        size_3 = cursor.size()
+        self.assertEqual(size_3, 0, "Tiene que devolver 0 y ha devuelto %s" % size_3)
 
     @classmethod
     def tearDownClass(cls) -> None:
         """Ensure test clear all data."""
         finish_testing()
 
 
@@ -755,15 +799,14 @@
     def setUpClass(cls) -> None:
         """Ensure pineboo is initialized for testing."""
         init_testing()
 
     def test_basic_relations_1(self) -> None:
         """Test basic relations 1."""
         from pineboolib.application.database import pnsqlcursor
-        from pineboolib.application.metadata import pnrelationmetadata
 
         cur_areas = pnsqlcursor.PNSqlCursor("flareas")
 
         cursor_6 = pnsqlcursor.PNSqlCursor("flareas")
         cursor_6.setModeAccess(cursor_6.Insert)
         cursor_6.refreshBuffer()
         cursor_6.setValueBuffer("bloqueo", True)
```

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnsqldriversmanager.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_pnsqldriversmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_pnsqlquery.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_pnsqlquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/tests/test_utils.py` & `pineboo-0.99.81/pineboolib/application/database/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/database/utils.py` & `pineboo-0.99.81/pineboolib/application/database/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/file.py` & `pineboo-0.99.81/pineboolib/application/file.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/load_script.py` & `pineboo-0.99.81/pineboolib/application/load_script.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/pnaction.py` & `pineboo-0.99.81/pineboolib/application/metadata/pnaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/pncompoundkeymetadata.py` & `pineboo-0.99.81/pineboolib/application/metadata/pncompoundkeymetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/pnfieldmetadata.py` & `pineboo-0.99.81/pineboolib/application/metadata/pnfieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/pnrelationmetadata.py` & `pineboo-0.99.81/pineboolib/application/metadata/pnrelationmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/pntablemetadata.py` & `pineboo-0.99.81/pineboolib/application/metadata/pntablemetadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,15 +499,15 @@
     def fieldList(self, only_names: bool = False) -> List["pnfieldmetadata.PNFieldMetaData"]:
         """
         Return a list of field definitions.
 
         @return Object with the table field deficits list
         """
 
-        return self.fieldNames() if only_names else list(self.private._fields_dict.values())
+        return self.fieldNames() if only_names else list(self.private._fields_dict.values())  # type: ignore [return-value, arg-type]
 
     def fieldListArray(self, prefix_table: bool = False) -> List[str]:
         """
         To get a string with the names of the fields separated by commas.
 
         @param prefix_table If TRUE a prefix is ​​added to each field with the name of the table; tablename.fieldname
         @return String with the names of the fields separated by commas.
```

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pnaction.py` & `pineboo-0.99.81/pineboolib/application/metadata/tests/test_pnaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py` & `pineboo-0.99.81/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pnfieldmetadata.py` & `pineboo-0.99.81/pineboolib/application/metadata/tests/test_pnfieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pnrelationmetadata.py` & `pineboo-0.99.81/pineboolib/application/metadata/tests/test_pnrelationmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/metadata/tests/test_pntablemetadata.py` & `pineboo-0.99.81/pineboolib/application/metadata/tests/test_pntablemetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/module.py` & `pineboo-0.99.81/pineboolib/application/module.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/moduleactions.py` & `pineboo-0.99.81/pineboolib/application/moduleactions.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/packager/pnpackager.py` & `pineboo-0.99.81/pineboolib/application/packager/pnpackager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/packager/pnunpacker.py` & `pineboo-0.99.81/pineboolib/application/packager/pnunpacker.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/packager/tests/test_pnpackager.py` & `pineboo-0.99.81/pineboolib/application/packager/tests/test_pnpackager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/packager/tests/test_pnunpaker.py` & `pineboo-0.99.81/pineboolib/application/packager/tests/test_pnunpaker.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/kparsertools.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_kut/kparsertools.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/kut2fpdf.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_kut/kut2fpdf.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/pnmtdparser.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/pnmtdparser.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/flex.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/flex.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/flscriptparse.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/flscriptparse.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/lextab.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/lextab.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/postparse.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/postparse.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/pyconvert.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/pyconvert.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/pytnyzer.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/pytnyzer.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_qsa/token_rules.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_qsa/token_rules.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_ui/qt3ui.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_ui/qt3ui.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py` & `pineboo-0.99.81/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/pnapplication.py` & `pineboo-0.99.81/pineboolib/application/pnapplication.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/process.py` & `pineboo-0.99.81/pineboolib/application/process.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/projectmodule.py` & `pineboo-0.99.81/pineboolib/application/projectmodule.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/proxy.py` & `pineboo-0.99.81/pineboolib/application/proxy.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/qsadictmodules.py` & `pineboo-0.99.81/pineboolib/application/qsadictmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/qsatypes/date.py` & `pineboo-0.99.81/pineboolib/application/qsatypes/date.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/qsatypes/sysbasetype.py` & `pineboo-0.99.81/pineboolib/application/qsatypes/sysbasetype.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/qsatypes/tests/test_date.py` & `pineboo-0.99.81/pineboolib/application/qsatypes/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/qsatypes/tests/test_sysbasetype.py` & `pineboo-0.99.81/pineboolib/application/qsatypes/tests/test_sysbasetype.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/safeqsa.py` & `pineboo-0.99.81/pineboolib/application/safeqsa.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/signatures/pdf_digest.py` & `pineboo-0.99.81/pineboolib/application/signatures/pdf_digest.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/signatures/pdf_qr.py` & `pineboo-0.99.81/pineboolib/application/signatures/pdf_qr.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/signatures/tests/test_signatures.py` & `pineboo-0.99.81/pineboolib/application/signatures/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/signatures/xml_digest.py` & `pineboo-0.99.81/pineboolib/application/signatures/xml_digest.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/staticloader/pnmodulesstaticloader.py` & `pineboo-0.99.81/pineboolib/application/staticloader/pnmodulesstaticloader.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/staticloader/tests/test_static_loader.py` & `pineboo-0.99.81/pineboolib/application/staticloader/tests/test_static_loader.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/staticloader/ui/static_loader.ui` & `pineboo-0.99.81/pineboolib/application/staticloader/ui/static_loader.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/tests/test_application.py` & `pineboo-0.99.81/pineboolib/application/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/tests/test_load_script.py` & `pineboo-0.99.81/pineboolib/application/tests/test_load_script.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/tests/test_process.py` & `pineboo-0.99.81/pineboolib/application/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/tests/test_projectmodule.py` & `pineboo-0.99.81/pineboolib/application/tests/test_projectmodule.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/tests/test_proxy.py` & `pineboo-0.99.81/pineboolib/application/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/tests/test_types.py` & `pineboo-0.99.81/pineboolib/application/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/tests/test_xmlaction.py` & `pineboo-0.99.81/pineboolib/application/tests/test_xmlaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/translator/pntranslator.py` & `pineboo-0.99.81/pineboolib/application/translator/pntranslator.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/translator/test/test_pntranslator.py` & `pineboo-0.99.81/pineboolib/application/translator/test/test_pntranslator.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/types.py` & `pineboo-0.99.81/pineboolib/application/types.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/check_dependencies.py` & `pineboo-0.99.81/pineboolib/application/utils/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/convert_flaction.py` & `pineboo-0.99.81/pineboolib/application/utils/convert_flaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/date_conversion.py` & `pineboo-0.99.81/pineboolib/application/utils/date_conversion.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/flfiles_dir.py` & `pineboo-0.99.81/pineboolib/application/utils/flfiles_dir.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/geometry.py` & `pineboo-0.99.81/pineboolib/application/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/mobilemode.py` & `pineboo-0.99.81/pineboolib/application/utils/mobilemode.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/modules.py` & `pineboo-0.99.81/pineboolib/application/utils/modules.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/path.py` & `pineboo-0.99.81/pineboolib/application/utils/path.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/service.py` & `pineboo-0.99.81/pineboolib/application/utils/service.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/sql_tools.py` & `pineboo-0.99.81/pineboolib/application/utils/sql_tools.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/utils/xpm.py` & `pineboo-0.99.81/pineboolib/application/utils/xpm.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/application/xmlaction.py` & `pineboo-0.99.81/pineboolib/application/xmlaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/decorators.py` & `pineboo-0.99.81/pineboolib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/exceptions.py` & `pineboo-0.99.81/pineboolib/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/garbage_collector.py` & `pineboo-0.99.81/pineboolib/core/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Pi-symbol.svg` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Pi-symbol.svg`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi.psd` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi.psd`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi2.xcf` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi2.xcf`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi2_256.png` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi2_256.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi2_512.png` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi2_512.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi_1024.png` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi_1024.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi_256.png` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi_256.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icono_pi/Symbol_pi_512.png` & `pineboo-0.99.81/pineboolib/core/images/icono_pi/Symbol_pi_512.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/about.png` & `pineboo-0.99.81/pineboolib/core/images/icons/about.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/aboutqt.png` & `pineboo-0.99.81/pineboolib/core/images/icons/aboutqt.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/cancel.png` & `pineboo-0.99.81/pineboolib/core/images/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/consola.png` & `pineboo-0.99.81/pineboolib/core/images/icons/consola.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/date.png` & `pineboo-0.99.81/pineboolib/core/images/icons/date.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/delete.png` & `pineboo-0.99.81/pineboolib/core/images/icons/delete.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/down.png` & `pineboo-0.99.81/pineboolib/core/images/icons/down.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/edit.png` & `pineboo-0.99.81/pineboolib/core/images/icons/edit.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/edit_file.png` & `pineboo-0.99.81/pineboolib/core/images/icons/edit_file.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/edit_file_xml.png` & `pineboo-0.99.81/pineboolib/core/images/icons/edit_file_xml.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/estilo.png` & `pineboo-0.99.81/pineboolib/core/images/icons/estilo.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/exit.png` & `pineboo-0.99.81/pineboolib/core/images/icons/exit.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/fltable-clean.png` & `pineboo-0.99.81/pineboolib/core/images/icons/fltable-clean.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/fltable-data.png` & `pineboo-0.99.81/pineboolib/core/images/icons/fltable-data.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/fltable-odf.png` & `pineboo-0.99.81/pineboolib/core/images/icons/fltable-odf.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/folder_update.png` & `pineboo-0.99.81/pineboolib/core/images/icons/folder_update.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/font.png` & `pineboo-0.99.81/pineboolib/core/images/icons/font.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-bottom.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-bottom.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-down.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-down.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-first.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-first.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-home.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-home.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-jump.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-jump.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-last.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-last.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-next.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-next.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-previous.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-previous.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-top.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-top.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/go-up.png` & `pineboo-0.99.81/pineboolib/core/images/icons/go-up.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-add.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-add.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-bold.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-bold.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-cancel.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-cancel.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-clear.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-clear.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-copy.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-copy.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-cut.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-cut.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-delete.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-delete.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-find-and-replace.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-find-and-replace.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-find.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-find.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-fullscreen.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-fullscreen.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-back-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-back-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-back-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-back-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-down.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-down.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-forward-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-forward-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-forward-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-forward-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-go-up.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-go-up.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-bottom.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-bottom.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-first-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-first-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-first-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-first-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-last-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-last-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-last-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-last-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-goto-top.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-goto-top.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-home.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-home.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-indent-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-indent-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-indent-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-indent-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-italic.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-italic.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-jump-to-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-jump-to-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-jump-to-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-jump-to-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-justify-center.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-justify-center.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-justify-fill.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-justify-fill.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-justify-left.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-justify-left.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-justify-right.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-justify-right.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-forward-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-forward-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-forward-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-forward-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-next-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-next-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-next-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-next-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-play-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-play-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-previous-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-previous-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-previous-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-previous-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-record.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-record.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-rewind-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-rewind-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-rewind-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-rewind-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-media-stop.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-media-stop.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-new.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-new.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-open.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-open.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-paste.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-paste.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-print-preview.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-print-preview.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-print.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-print.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-properties.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-properties.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-redo-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-redo-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-refresh.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-refresh.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-save-as.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-save-as.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-save.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-save.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-select-all.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-select-all.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-stop.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-stop.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-strikethrough.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-strikethrough.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-underline.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-underline.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-undo-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-undo-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-unindent-ltr.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-unindent-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/gtk-unindent-rtl.png` & `pineboo-0.99.81/pineboolib/core/images/icons/gtk-unindent-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/help_index.png` & `pineboo-0.99.81/pineboolib/core/images/icons/help_index.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/insert.png` & `pineboo-0.99.81/pineboolib/core/images/icons/insert.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/lock.png` & `pineboo-0.99.81/pineboolib/core/images/icons/lock.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/ok.png` & `pineboo-0.99.81/pineboolib/core/images/icons/ok.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/paste.png` & `pineboo-0.99.81/pineboolib/core/images/icons/paste.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-128.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-128.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-16.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-16.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-24.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-24.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-256.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-256.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-32.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-32.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-48.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-48.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-57.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-57.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-64.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-64.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo-72.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo-72.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo-logo.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo-logo.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-128.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-128.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-16.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-16.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-24.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-24.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-256.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-256.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-32.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-32.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-48.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-48.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo-64.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo-64.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/pineboo2-logo.png` & `pineboo-0.99.81/pineboolib/core/images/icons/pineboo2-logo.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/print.png` & `pineboo-0.99.81/pineboolib/core/images/icons/print.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/reload.png` & `pineboo-0.99.81/pineboolib/core/images/icons/reload.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/signed_stamp.png` & `pineboo-0.99.81/pineboolib/core/images/icons/signed_stamp.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_ebcomportamiento.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_ebcomportamiento.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flareas.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flareas.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_fldumpdb.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_fldumpdb.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flgroups.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flgroups.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flloadmod.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flloadmod.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flloadmodpkg.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flloadmodpkg.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flmodules.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flmodules.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flmrproper.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flmrproper.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flreinit.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flreinit.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flreloadbatch.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flreloadbatch.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flreloadlast.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flreloadlast.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/sys_flusers.png` & `pineboo-0.99.81/pineboolib/core/images/icons/sys_flusers.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/terminal.png` & `pineboo-0.99.81/pineboolib/core/images/icons/terminal.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/unlock.png` & `pineboo-0.99.81/pineboolib/core/images/icons/unlock.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/up.png` & `pineboo-0.99.81/pineboolib/core/images/icons/up.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/icons/zoom.png` & `pineboo-0.99.81/pineboolib/core/images/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/splashscreen/dbadmin240.png` & `pineboo-0.99.81/pineboolib/core/images/splashscreen/dbadmin240.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/splashscreen/dbadmin480.png` & `pineboo-0.99.81/pineboolib/core/images/splashscreen/dbadmin480.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/splashscreen/quick240.png` & `pineboo-0.99.81/pineboolib/core/images/splashscreen/quick240.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/splashscreen/quick480.png` & `pineboo-0.99.81/pineboolib/core/images/splashscreen/quick480.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/splashscreen/splash.png` & `pineboo-0.99.81/pineboolib/core/images/splashscreen/splash.png`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/images/splashscreen/splash.svg` & `pineboo-0.99.81/pineboolib/core/images/splashscreen/splash.svg`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/message_manager.py` & `pineboo-0.99.81/pineboolib/core/message_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/settings.py` & `pineboo-0.99.81/pineboolib/core/settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/test/test_settings.py` & `pineboo-0.99.81/pineboolib/core/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/utils/check_dependencies.py` & `pineboo-0.99.81/pineboolib/core/utils/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/utils/logging.py` & `pineboo-0.99.81/pineboolib/core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/utils/singleton.py` & `pineboo-0.99.81/pineboolib/core/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/utils/struct.py` & `pineboo-0.99.81/pineboolib/core/utils/struct.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/utils/tests/test_utils_base.py` & `pineboo-0.99.81/pineboolib/core/utils/tests/test_utils_base.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/utils/tests/test_version.py` & `pineboo-0.99.81/pineboolib/core/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/utils/utils_base.py` & `pineboo-0.99.81/pineboolib/core/utils/utils_base.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/core/utils/version.py` & `pineboo-0.99.81/pineboolib/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqformdb.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqformdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqods.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqods.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqs.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqs.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqsql.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/aqssproject.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/aqssproject.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py` & `pineboo-0.99.81/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flcodbar.py` & `pineboo-0.99.81/pineboolib/fllegacy/flcodbar.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fldatatable.py` & `pineboo-0.99.81/pineboolib/fllegacy/fldatatable.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fldateedit.py` & `pineboo-0.99.81/pineboolib/fllegacy/fldateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fldoublevalidator.py` & `pineboo-0.99.81/pineboolib/fllegacy/fldoublevalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flfastcgi.py` & `pineboo-0.99.81/pineboolib/fllegacy/flfastcgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flfielddb.py` & `pineboo-0.99.81/pineboolib/fllegacy/flfielddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flformdb.py` & `pineboo-0.99.81/pineboolib/fllegacy/flformdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flformrecorddb.py` & `pineboo-0.99.81/pineboolib/fllegacy/flformrecorddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flformsearchdb.py` & `pineboo-0.99.81/pineboolib/fllegacy/flformsearchdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flintvalidator.py` & `pineboo-0.99.81/pineboolib/fllegacy/flintvalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fllineedit.py` & `pineboo-0.99.81/pineboolib/fllegacy/fllineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fllistviewitem.py` & `pineboo-0.99.81/pineboolib/fllegacy/fllistviewitem.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flmanager.py` & `pineboo-0.99.81/pineboolib/fllegacy/flmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flmanagermodules.py` & `pineboo-0.99.81/pineboolib/fllegacy/flmanagermodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flnetwork.py` & `pineboo-0.99.81/pineboolib/fllegacy/flnetwork.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flpixmapview.py` & `pineboo-0.99.81/pineboolib/fllegacy/flpixmapview.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flposprinter.py` & `pineboo-0.99.81/pineboolib/fllegacy/flposprinter.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flreportengine.py` & `pineboo-0.99.81/pineboolib/fllegacy/flreportengine.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flreportviewer.py` & `pineboo-0.99.81/pineboolib/fllegacy/flreportviewer.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flserialport.py` & `pineboo-0.99.81/pineboolib/fllegacy/flserialport.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flsettings.py` & `pineboo-0.99.81/pineboolib/fllegacy/flsettings.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flsmtpclient.py` & `pineboo-0.99.81/pineboolib/fllegacy/flsmtpclient.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flspinbox.py` & `pineboo-0.99.81/pineboolib/fllegacy/flspinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fltable.py` & `pineboo-0.99.81/pineboolib/fllegacy/fltable.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fltabledb.py` & `pineboo-0.99.81/pineboolib/fllegacy/fltabledb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fltimeedit.py` & `pineboo-0.99.81/pineboolib/fllegacy/fltimeedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/fluintvalidator.py` & `pineboo-0.99.81/pineboolib/fllegacy/fluintvalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flutil.py` & `pineboo-0.99.81/pineboolib/fllegacy/flutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flvar.py` & `pineboo-0.99.81/pineboolib/fllegacy/flvar.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/flwidget.py` & `pineboo-0.99.81/pineboolib/fllegacy/flwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui` & `pineboo-0.99.81/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/systype.py` & `pineboo-0.99.81/pineboolib/fllegacy/systype.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flcodbar.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_flcodbar.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_fldatatable.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_fldatatable.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_fldateedit.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_fldateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flfielddb.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_flfielddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flform.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_flform.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flformrecorddb.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_flformrecorddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flformsearch.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_flformsearch.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flmanager.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_flmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flreportengine.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_flreportengine.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_fltabledb.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_fltabledb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_flutil.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_flutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_settings.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_smtp.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_smtp.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/fllegacy/tests/test_systype.py` & `pineboo-0.99.81/pineboolib/fllegacy/tests/test_systype.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/interfaces/iconnection.py` & `pineboo-0.99.81/pineboolib/interfaces/iconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/interfaces/ifieldmetadata.py` & `pineboo-0.99.81/pineboolib/interfaces/ifieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/interfaces/imainwindow.py` & `pineboo-0.99.81/pineboolib/interfaces/imainwindow.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/interfaces/imanager.py` & `pineboo-0.99.81/pineboolib/interfaces/imanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/interfaces/isqlcursor.py` & `pineboo-0.99.81/pineboolib/interfaces/isqlcursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/interfaces/isqldriver.py` & `pineboo-0.99.81/pineboolib/interfaces/isqldriver.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/interfaces/itablemetadata.py` & `pineboo-0.99.81/pineboolib/interfaces/itablemetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/connection.py` & `pineboo-0.99.81/pineboolib/loader/connection.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/dgi.py` & `pineboo-0.99.81/pineboolib/loader/dgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/dlgconnect/conn_dialog.py` & `pineboo-0.99.81/pineboolib/loader/dlgconnect/conn_dialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/dlgconnect/dlgconnect.py` & `pineboo-0.99.81/pineboolib/loader/dlgconnect/dlgconnect.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/dlgconnect/dlgconnect.ui` & `pineboo-0.99.81/pineboolib/loader/dlgconnect/dlgconnect.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py` & `pineboo-0.99.81/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/init_project.py` & `pineboo-0.99.81/pineboolib/loader/init_project.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/main.py` & `pineboo-0.99.81/pineboolib/loader/main.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/options.py` & `pineboo-0.99.81/pineboolib/loader/options.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/preload.py` & `pineboo-0.99.81/pineboolib/loader/preload.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/projectconfig.py` & `pineboo-0.99.81/pineboolib/loader/projectconfig.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/tests/test_connection.py` & `pineboo-0.99.81/pineboolib/loader/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/tests/test_main.py` & `pineboo-0.99.81/pineboolib/loader/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/tests/test_projectconfig.py` & `pineboo-0.99.81/pineboolib/loader/tests/test_projectconfig.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/loader/utils.py` & `pineboo-0.99.81/pineboolib/loader/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py` & `pineboo-0.99.81/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py` & `pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui` & `pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py` & `pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py` & `pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py` & `pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py` & `pineboo-0.99.81/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/dgi/dgi_schema.py` & `pineboo-0.99.81/pineboolib/plugins/dgi/dgi_schema.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/eneboo.py` & `pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/eneboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/mainform.ui` & `pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/mainform.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py` & `pineboo-0.99.81/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py` & `pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui` & `pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py` & `pineboo-0.99.81/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/flmysql_myisam.py` & `pineboo-0.99.81/pineboolib/plugins/sql/flmysql_myisam.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/flpymssql.py` & `pineboo-0.99.81/pineboolib/plugins/sql/flpymssql.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/flpyodbc.py` & `pineboo-0.99.81/pineboolib/plugins/sql/flpyodbc.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/flqpsql.py` & `pineboo-0.99.81/pineboolib/plugins/sql/flqpsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/flsqlite.py` & `pineboo-0.99.81/pineboolib/plugins/sql/flsqlite.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flmysql_innodb.py` & `pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flmysql_innodb.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flmysql_myisam.py` & `pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flmysql_myisam.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flpymssql.py` & `pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flpymssql.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flpyodbc.py` & `pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flpyodbc.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_flsqlite.py` & `pineboo-0.99.81/pineboolib/plugins/sql/tests/test_flsqlite.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_qpsql.py` & `pineboo-0.99.81/pineboolib/plugins/sql/tests/test_qpsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/plugins/sql/tests/test_stress.py` & `pineboo-0.99.81/pineboolib/plugins/sql/tests/test_stress.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/checkbox.py` & `pineboo-0.99.81/pineboolib/q3widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/dateedit.py` & `pineboo-0.99.81/pineboolib/q3widgets/dateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/dialog.py` & `pineboo-0.99.81/pineboolib/q3widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/filedialog.py` & `pineboo-0.99.81/pineboolib/q3widgets/filedialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/lineedit.py` & `pineboo-0.99.81/pineboolib/q3widgets/lineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/messagebox.py` & `pineboo-0.99.81/pineboolib/q3widgets/messagebox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/numberedit.py` & `pineboo-0.99.81/pineboolib/q3widgets/numberedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qaction.py` & `pineboo-0.99.81/pineboolib/q3widgets/qaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qbuttongroup.py` & `pineboo-0.99.81/pineboolib/q3widgets/qbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qbytearray.py` & `pineboo-0.99.81/pineboolib/q3widgets/qbytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qcheckbox.py` & `pineboo-0.99.81/pineboolib/q3widgets/qcheckbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qcombobox.py` & `pineboo-0.99.81/pineboolib/q3widgets/qcombobox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qdateedit.py` & `pineboo-0.99.81/pineboolib/q3widgets/qdateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qdialog.py` & `pineboo-0.99.81/pineboolib/q3widgets/qdialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qframe.py` & `pineboo-0.99.81/pineboolib/q3widgets/qframe.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qgroupbox.py` & `pineboo-0.99.81/pineboolib/q3widgets/qgroupbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qhboxlayout.py` & `pineboo-0.99.81/pineboolib/q3widgets/qhboxlayout.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qhttp.py` & `pineboo-0.99.81/pineboolib/q3widgets/qhttp.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qlabel.py` & `pineboo-0.99.81/pineboolib/q3widgets/qlabel.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qline.py` & `pineboo-0.99.81/pineboolib/q3widgets/qline.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qlineedit.py` & `pineboo-0.99.81/pineboolib/q3widgets/qlineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qlistview.py` & `pineboo-0.99.81/pineboolib/q3widgets/qlistview.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qobject.py` & `pineboo-0.99.81/pineboolib/q3widgets/qobject.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qpushbutton.py` & `pineboo-0.99.81/pineboolib/q3widgets/qpushbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qradiobutton.py` & `pineboo-0.99.81/pineboolib/q3widgets/qradiobutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qtable.py` & `pineboo-0.99.81/pineboolib/q3widgets/qtable.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qtabwidget.py` & `pineboo-0.99.81/pineboolib/q3widgets/qtabwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qtextedit.py` & `pineboo-0.99.81/pineboolib/q3widgets/qtextedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qtimeedit.py` & `pineboo-0.99.81/pineboolib/q3widgets/qtimeedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qtoolbutton.py` & `pineboo-0.99.81/pineboolib/q3widgets/qtoolbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qvboxlayout.py` & `pineboo-0.99.81/pineboolib/q3widgets/qvboxlayout.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/qwidget.py` & `pineboo-0.99.81/pineboolib/q3widgets/qwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/spinbox.py` & `pineboo-0.99.81/pineboolib/q3widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_messagebox.py` & `pineboo-0.99.81/pineboolib/q3widgets/tests/test_messagebox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qbytearray.py` & `pineboo-0.99.81/pineboolib/q3widgets/tests/test_qbytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qhttp.py` & `pineboo-0.99.81/pineboolib/q3widgets/tests/test_qhttp.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qpushbutton.py` & `pineboo-0.99.81/pineboolib/q3widgets/tests/test_qpushbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qradiobuttons.py` & `pineboo-0.99.81/pineboolib/q3widgets/tests/test_qradiobuttons.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qtabwidget.py` & `pineboo-0.99.81/pineboolib/q3widgets/tests/test_qtabwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_qtextstream.py` & `pineboo-0.99.81/pineboolib/q3widgets/tests/test_qtextstream.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/q3widgets/tests/test_spinbox.py` & `pineboo-0.99.81/pineboolib/q3widgets/tests/test_spinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/decorators.py` & `pineboo-0.99.81/pineboolib/qsa/decorators.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/emptyscript.py` & `pineboo-0.99.81/pineboolib/qsa/emptyscript.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/formdbwidget.py` & `pineboo-0.99.81/pineboolib/qsa/formdbwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/input.py` & `pineboo-0.99.81/pineboolib/qsa/input.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/object_class.py` & `pineboo-0.99.81/pineboolib/qsa/object_class.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/pncontrolsfactory.py` & `pineboo-0.99.81/pineboolib/qsa/pncontrolsfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/qsa.py` & `pineboo-0.99.81/pineboolib/qsa/qsa.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/tests/test_class.py` & `pineboo-0.99.81/pineboolib/qsa/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/tests/test_classes.py` & `pineboo-0.99.81/pineboolib/qsa/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/tests/test_knownbugs.py` & `pineboo-0.99.81/pineboolib/qsa/tests/test_knownbugs.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/tests/test_orm.py` & `pineboo-0.99.81/pineboolib/qsa/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/tests/test_query_values.py` & `pineboo-0.99.81/pineboolib/qsa/tests/test_query_values.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/tests/test_require.py` & `pineboo-0.99.81/pineboolib/qsa/tests/test_require.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/tests/test_utils.py` & `pineboo-0.99.81/pineboolib/qsa/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/qsa/utils.py` & `pineboo-0.99.81/pineboolib/qsa/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/FLWidgetMasterTable.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/FLWidgetMasterTable.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/ebcomportamiento.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/ebcomportamiento.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/flareas.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/flareas.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/flfiles.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/flfiles.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/flgroups.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/flgroups.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/flmodulos.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/flmodulos.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/fltest.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/fltest.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/flusers.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/flusers.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/master.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/master.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/master_copy.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/master_copy.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/master_print.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/master_print.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/master_print_copy.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/master_print_copy.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/forms/sys.ui` & `pineboo-0.99.81/pineboolib/system_module/forms/sys.ui`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flareas_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flareas_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flfiles_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flfiles_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flgroups_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flgroups_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/fllarge_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/fllarge_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flmetadata_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flmetadata_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flmodules_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flmodules_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flseqs_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flseqs_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flserial_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flserial_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flsettings_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flsettings_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/fltest2_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/fltest2_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/fltest3_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/fltest3_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/fltest4_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/fltest4_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/fltest5_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/fltest5_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/fltest_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/fltest_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flupdates_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flupdates_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flusers_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flusers_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/models/flvar_model.py` & `pineboo-0.99.81/pineboolib/system_module/models/flvar_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/queries/fltest2.qry` & `pineboo-0.99.81/pineboolib/system_module/queries/fltest2.qry`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/ebcomportamiento.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/ebcomportamiento.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/flfiles.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/flfiles.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/flloadmod.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/flloadmod.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/flmodules.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/flmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/flreloadbatch.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/flreloadbatch.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/flreloadlast.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/flreloadlast.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/sys.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/sys.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flfiles.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flfiles.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flmodules.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flmrproper.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flmrproper.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_flreinit.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_flreinit.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_reload_last.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_reload_last.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/scripts/tests/test_sys.py` & `pineboo-0.99.81/pineboolib/system_module/scripts/tests/test_sys.py`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/sys.xml` & `pineboo-0.99.81/pineboolib/system_module/sys.xml`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/sys.xpm` & `pineboo-0.99.81/pineboolib/system_module/sys.xpm`

 * *Files identical despite different names*

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.ca.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.ca.ts`

 * *Files 0% similar despite different names*

#### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.ca.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.ca.ts`

```diff
@@ -397,34 +397,97 @@
       <source>No</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Form</name>
     <message>
-      <location filename="../forms/fltest.ui" line="0"/>
-      <location filename="../forms/flmodulos.ui" line="0"/>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>Form</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Acerca de pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>iduser</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Principal</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
+
+https://github.com/deavid/pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>idgroup</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Empresas colaboradoras:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flmodulos.ui" line="0"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Librerías</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copiar al portapapeles</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Licencia</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copyright © 2012 David Martínez Martí
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the “Software”), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Cerrar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/fltest.ui" line="0"/>
       <location filename="../forms/flusers.ui" line="0"/>
-      <source>descripcion</source>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>Form</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idmodulo</source>
@@ -442,14 +505,20 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idarea</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>descripcion</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Ficheros</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>flfiles</source>
@@ -457,14 +526,24 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Log</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>iduser</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>idgroup</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>string_field</source>
@@ -496,93 +575,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>bloqueo</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Acerca de pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Principal</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
-
-https://github.com/deavid/pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Empresas colaboradoras:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Librerías</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copiar al portapapeles</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Licencia</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copyright © 2012 David Martínez Martí
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the “Software”), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Cerrar</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>MainForm</name>
     <message>
       <location filename="../../plugins/mainform/eneboo_mdi/eneboo_mdi.py" line="112"/>
       <source>Cascada</source>
       <translation type="unfinished"/>
@@ -800,15 +800,15 @@
       <source>Elegir archivo</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>PNSqlCursor</name>
     <message>
-      <location filename="../../application/database/pnsqlcursor.py" line="2352"/>
+      <location filename="../../application/database/pnsqlcursor.py" line="2354"/>
       <location filename="../../application/database/pnsqlcursor.py" line="781"/>
       <source>No hay ningún registro seleccionado</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../application/database/pnsqlcursor.py" line="793"/>
       <source>El registro activo será borrado. ¿ Está seguro ?</source>
@@ -898,14 +898,19 @@
       <location filename="../../fllegacy/tests/test_fltabledb.py" line="283"/>
       <source>Distinto de Valor</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>application</name>
+    <message>
+      <location filename="../../fllegacy/flmanager.py" line="1271"/>
+      <source>No se ha podido crear los metadatatos para la tabla %s</source>
+      <translation type="unfinished"/>
+    </message>
     <message encoding="UTF-8">
       <location filename="../../interfaces/isqldriver.py" line="360"/>
       <source>Sí</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../interfaces/isqldriver.py" line="790"/>
@@ -959,19 +964,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../plugins/sql/flqpsql.py" line="310"/>
       <source>Comprobando indices</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/flmanager.py" line="1271"/>
-      <source>No se ha podido crear los metadatatos para la tabla %s</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>ebcomportamiento</name>
     <message>
       <location filename="../forms/ebcomportamiento.ui" line="0"/>
       <source>Opciones de comportamiento</source>
       <translation type="unfinished"/>
@@ -1455,87 +1455,44 @@
       <location filename="../../fllegacy/tests/test_systype.py" line="47"/>
       <source>hola python sin group</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>scripts</name>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="19"/>
-      <source>Directorio de Módulos</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="34"/>
-      <source>Error al buscar los módulos en el directorio:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="52"/>
-      <source>Error al cargar el módulo:</source>
-      <translation type="unfinished"/>
-    </message>
     <message>
-      <location filename="../scripts/flreloadbatch.py" line="96"/>
-      <source>Aceptar</source>
+      <location filename="../../fllegacy/systype.py" line="540"/>
+      <source>Seleccionar Eneboo/Abanq Package</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
-      <location filename="../scripts/flreloadbatch.py" line="97"/>
-      <source>Cancelar</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="99"/>
-      <source>Seleccione módulos a cargar</source>
+      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
+      <source>hola python</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="23"/>
-      <source>Elegir Fichero</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flmodules.py" line="249"/>
-      <location filename="../scripts/flloadmod.py" line="31"/>
-      <source>Imposible cargar el módulo.
-Licencia del módulo no aceptada.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flloadmod.py" line="57"/>
-      <source>Este módulo depende del módulo</source>
+      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
+      <source>single</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="59"/>
-      <source>, que no está instalado.
-FacturaLUX puede fallar por esta causa.
-¿Desea continuar la carga?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="21"/>
-      <source>Módulo a cargar (*.mod)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="22"/>
-      <source>Módulo a cargar</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
+      <source>variable %s</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flreloadlast.py" line="51"/>
-      <source>Error en la carga del fichero xml .mod</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
+      <source>multiple variable %s , %s</source>
       <translation type="unfinished"/>
     </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="94"/>
-      <source>Error al crear el área:</source>
+    <message>
+      <location filename="../scripts/flreloadbatch.py" line="97"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
+      <source>Cancelar</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="66"/>
       <source>- Cargando ::</source>
       <translation type="unfinished"/>
     </message>
@@ -1581,48 +1538,91 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="238"/>
       <source>No, no acepto este acuerdo de licencia.</source>
       <translation type="unfinished"/>
     </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="31"/>
+      <location filename="../scripts/flmodules.py" line="249"/>
+      <source>Imposible cargar el módulo.
+Licencia del módulo no aceptada.</source>
+      <translation type="unfinished"/>
+    </message>
     <message>
       <location filename="../scripts/flmodules.py" line="291"/>
       <source>* Carga finalizada.</source>
       <translation type="unfinished"/>
     </message>
     <message encoding="UTF-8">
       <location filename="../scripts/flmodules.py" line="469"/>
       <source>* Exportación finalizada.</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
-      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
-      <source>single</source>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="19"/>
+      <source>Directorio de Módulos</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="34"/>
+      <source>Error al buscar los módulos en el directorio:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="52"/>
+      <source>Error al cargar el módulo:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/systype.py" line="540"/>
-      <source>Seleccionar Eneboo/Abanq Package</source>
+      <location filename="../scripts/flreloadbatch.py" line="96"/>
+      <source>Aceptar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="99"/>
+      <source>Seleccione módulos a cargar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="21"/>
+      <source>Módulo a cargar (*.mod)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="22"/>
+      <source>Módulo a cargar</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
-      <source>hola python</source>
+      <location filename="../scripts/flreloadlast.py" line="51"/>
+      <source>Error en la carga del fichero xml .mod</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="94"/>
+      <source>Error al crear el área:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
-      <source>variable %s</source>
+      <location filename="../scripts/flloadmod.py" line="23"/>
+      <source>Elegir Fichero</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="57"/>
+      <source>Este módulo depende del módulo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
-      <source>multiple variable %s , %s</source>
+      <location filename="../scripts/flloadmod.py" line="59"/>
+      <source>, que no está instalado.
+FacturaLUX puede fallar por esta causa.
+¿Desea continuar la carga?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>sys</name>
     <message>
       <location filename="../forms/sys.ui" line="0"/>
```

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.de.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.de.ts`

 * *Files 0% similar despite different names*

#### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.de.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.de.ts`

```diff
@@ -397,34 +397,97 @@
       <source>No</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Form</name>
     <message>
-      <location filename="../forms/fltest.ui" line="0"/>
-      <location filename="../forms/flmodulos.ui" line="0"/>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>Form</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Acerca de pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>iduser</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Principal</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
+
+https://github.com/deavid/pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>idgroup</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Empresas colaboradoras:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flmodulos.ui" line="0"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Librerías</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copiar al portapapeles</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Licencia</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copyright © 2012 David Martínez Martí
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the “Software”), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Cerrar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/fltest.ui" line="0"/>
       <location filename="../forms/flusers.ui" line="0"/>
-      <source>descripcion</source>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>Form</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idmodulo</source>
@@ -442,14 +505,20 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idarea</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>descripcion</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Ficheros</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>flfiles</source>
@@ -457,14 +526,24 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Log</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>iduser</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>idgroup</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>string_field</source>
@@ -496,93 +575,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>bloqueo</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Acerca de pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Principal</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
-
-https://github.com/deavid/pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Empresas colaboradoras:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Librerías</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copiar al portapapeles</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Licencia</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copyright © 2012 David Martínez Martí
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the “Software”), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Cerrar</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>MainForm</name>
     <message>
       <location filename="../../plugins/mainform/eneboo_mdi/eneboo_mdi.py" line="112"/>
       <source>Cascada</source>
       <translation type="unfinished"/>
@@ -800,15 +800,15 @@
       <source>Elegir archivo</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>PNSqlCursor</name>
     <message>
-      <location filename="../../application/database/pnsqlcursor.py" line="2352"/>
+      <location filename="../../application/database/pnsqlcursor.py" line="2354"/>
       <location filename="../../application/database/pnsqlcursor.py" line="781"/>
       <source>No hay ningún registro seleccionado</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../application/database/pnsqlcursor.py" line="793"/>
       <source>El registro activo será borrado. ¿ Está seguro ?</source>
@@ -898,14 +898,19 @@
       <location filename="../../fllegacy/tests/test_fltabledb.py" line="283"/>
       <source>Distinto de Valor</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>application</name>
+    <message>
+      <location filename="../../fllegacy/flmanager.py" line="1271"/>
+      <source>No se ha podido crear los metadatatos para la tabla %s</source>
+      <translation type="unfinished"/>
+    </message>
     <message encoding="UTF-8">
       <location filename="../../interfaces/isqldriver.py" line="360"/>
       <source>Sí</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../interfaces/isqldriver.py" line="790"/>
@@ -959,19 +964,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../plugins/sql/flqpsql.py" line="310"/>
       <source>Comprobando indices</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/flmanager.py" line="1271"/>
-      <source>No se ha podido crear los metadatatos para la tabla %s</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>ebcomportamiento</name>
     <message>
       <location filename="../forms/ebcomportamiento.ui" line="0"/>
       <source>Opciones de comportamiento</source>
       <translation type="unfinished"/>
@@ -1455,87 +1455,44 @@
       <location filename="../../fllegacy/tests/test_systype.py" line="47"/>
       <source>hola python sin group</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>scripts</name>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="19"/>
-      <source>Directorio de Módulos</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="34"/>
-      <source>Error al buscar los módulos en el directorio:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="52"/>
-      <source>Error al cargar el módulo:</source>
-      <translation type="unfinished"/>
-    </message>
     <message>
-      <location filename="../scripts/flreloadbatch.py" line="96"/>
-      <source>Aceptar</source>
+      <location filename="../../fllegacy/systype.py" line="540"/>
+      <source>Seleccionar Eneboo/Abanq Package</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
-      <location filename="../scripts/flreloadbatch.py" line="97"/>
-      <source>Cancelar</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="99"/>
-      <source>Seleccione módulos a cargar</source>
+      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
+      <source>hola python</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="23"/>
-      <source>Elegir Fichero</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flmodules.py" line="249"/>
-      <location filename="../scripts/flloadmod.py" line="31"/>
-      <source>Imposible cargar el módulo.
-Licencia del módulo no aceptada.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flloadmod.py" line="57"/>
-      <source>Este módulo depende del módulo</source>
+      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
+      <source>single</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="59"/>
-      <source>, que no está instalado.
-FacturaLUX puede fallar por esta causa.
-¿Desea continuar la carga?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="21"/>
-      <source>Módulo a cargar (*.mod)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="22"/>
-      <source>Módulo a cargar</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
+      <source>variable %s</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flreloadlast.py" line="51"/>
-      <source>Error en la carga del fichero xml .mod</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
+      <source>multiple variable %s , %s</source>
       <translation type="unfinished"/>
     </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="94"/>
-      <source>Error al crear el área:</source>
+    <message>
+      <location filename="../scripts/flreloadbatch.py" line="97"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
+      <source>Cancelar</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="66"/>
       <source>- Cargando ::</source>
       <translation type="unfinished"/>
     </message>
@@ -1581,48 +1538,91 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="238"/>
       <source>No, no acepto este acuerdo de licencia.</source>
       <translation type="unfinished"/>
     </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="31"/>
+      <location filename="../scripts/flmodules.py" line="249"/>
+      <source>Imposible cargar el módulo.
+Licencia del módulo no aceptada.</source>
+      <translation type="unfinished"/>
+    </message>
     <message>
       <location filename="../scripts/flmodules.py" line="291"/>
       <source>* Carga finalizada.</source>
       <translation type="unfinished"/>
     </message>
     <message encoding="UTF-8">
       <location filename="../scripts/flmodules.py" line="469"/>
       <source>* Exportación finalizada.</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
-      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
-      <source>single</source>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="19"/>
+      <source>Directorio de Módulos</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="34"/>
+      <source>Error al buscar los módulos en el directorio:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="52"/>
+      <source>Error al cargar el módulo:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/systype.py" line="540"/>
-      <source>Seleccionar Eneboo/Abanq Package</source>
+      <location filename="../scripts/flreloadbatch.py" line="96"/>
+      <source>Aceptar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="99"/>
+      <source>Seleccione módulos a cargar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="21"/>
+      <source>Módulo a cargar (*.mod)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="22"/>
+      <source>Módulo a cargar</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
-      <source>hola python</source>
+      <location filename="../scripts/flreloadlast.py" line="51"/>
+      <source>Error en la carga del fichero xml .mod</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="94"/>
+      <source>Error al crear el área:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
-      <source>variable %s</source>
+      <location filename="../scripts/flloadmod.py" line="23"/>
+      <source>Elegir Fichero</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="57"/>
+      <source>Este módulo depende del módulo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
-      <source>multiple variable %s , %s</source>
+      <location filename="../scripts/flloadmod.py" line="59"/>
+      <source>, que no está instalado.
+FacturaLUX puede fallar por esta causa.
+¿Desea continuar la carga?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>sys</name>
     <message>
       <location filename="../forms/sys.ui" line="0"/>
```

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.en.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.en.ts`

 * *Files 0% similar despite different names*

#### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.en.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.en.ts`

```diff
@@ -397,34 +397,97 @@
       <source>No</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Form</name>
     <message>
-      <location filename="../forms/fltest.ui" line="0"/>
-      <location filename="../forms/flmodulos.ui" line="0"/>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>Form</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Acerca de pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>iduser</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Principal</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
+
+https://github.com/deavid/pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>idgroup</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Empresas colaboradoras:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flmodulos.ui" line="0"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Librerías</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copiar al portapapeles</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Licencia</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copyright © 2012 David Martínez Martí
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the “Software”), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Cerrar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/fltest.ui" line="0"/>
       <location filename="../forms/flusers.ui" line="0"/>
-      <source>descripcion</source>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>Form</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idmodulo</source>
@@ -442,14 +505,20 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idarea</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>descripcion</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Ficheros</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>flfiles</source>
@@ -457,14 +526,24 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Log</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>iduser</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>idgroup</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>string_field</source>
@@ -496,93 +575,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>bloqueo</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Acerca de pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Principal</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
-
-https://github.com/deavid/pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Empresas colaboradoras:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Librerías</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copiar al portapapeles</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Licencia</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copyright © 2012 David Martínez Martí
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the “Software”), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Cerrar</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>MainForm</name>
     <message>
       <location filename="../../plugins/mainform/eneboo_mdi/eneboo_mdi.py" line="112"/>
       <source>Cascada</source>
       <translation type="unfinished"/>
@@ -800,15 +800,15 @@
       <source>Elegir archivo</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>PNSqlCursor</name>
     <message>
-      <location filename="../../application/database/pnsqlcursor.py" line="2352"/>
+      <location filename="../../application/database/pnsqlcursor.py" line="2354"/>
       <location filename="../../application/database/pnsqlcursor.py" line="781"/>
       <source>No hay ningún registro seleccionado</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../application/database/pnsqlcursor.py" line="793"/>
       <source>El registro activo será borrado. ¿ Está seguro ?</source>
@@ -898,14 +898,19 @@
       <location filename="../../fllegacy/tests/test_fltabledb.py" line="283"/>
       <source>Distinto de Valor</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>application</name>
+    <message>
+      <location filename="../../fllegacy/flmanager.py" line="1271"/>
+      <source>No se ha podido crear los metadatatos para la tabla %s</source>
+      <translation type="unfinished"/>
+    </message>
     <message encoding="UTF-8">
       <location filename="../../interfaces/isqldriver.py" line="360"/>
       <source>Sí</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../interfaces/isqldriver.py" line="790"/>
@@ -959,19 +964,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../plugins/sql/flqpsql.py" line="310"/>
       <source>Comprobando indices</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/flmanager.py" line="1271"/>
-      <source>No se ha podido crear los metadatatos para la tabla %s</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>ebcomportamiento</name>
     <message>
       <location filename="../forms/ebcomportamiento.ui" line="0"/>
       <source>Opciones de comportamiento</source>
       <translation type="unfinished"/>
@@ -1455,87 +1455,44 @@
       <location filename="../../fllegacy/tests/test_systype.py" line="47"/>
       <source>hola python sin group</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>scripts</name>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="19"/>
-      <source>Directorio de Módulos</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="34"/>
-      <source>Error al buscar los módulos en el directorio:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="52"/>
-      <source>Error al cargar el módulo:</source>
-      <translation type="unfinished"/>
-    </message>
     <message>
-      <location filename="../scripts/flreloadbatch.py" line="96"/>
-      <source>Aceptar</source>
+      <location filename="../../fllegacy/systype.py" line="540"/>
+      <source>Seleccionar Eneboo/Abanq Package</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
-      <location filename="../scripts/flreloadbatch.py" line="97"/>
-      <source>Cancelar</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="99"/>
-      <source>Seleccione módulos a cargar</source>
+      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
+      <source>hola python</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="23"/>
-      <source>Elegir Fichero</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flmodules.py" line="249"/>
-      <location filename="../scripts/flloadmod.py" line="31"/>
-      <source>Imposible cargar el módulo.
-Licencia del módulo no aceptada.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flloadmod.py" line="57"/>
-      <source>Este módulo depende del módulo</source>
+      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
+      <source>single</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="59"/>
-      <source>, que no está instalado.
-FacturaLUX puede fallar por esta causa.
-¿Desea continuar la carga?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="21"/>
-      <source>Módulo a cargar (*.mod)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="22"/>
-      <source>Módulo a cargar</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
+      <source>variable %s</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flreloadlast.py" line="51"/>
-      <source>Error en la carga del fichero xml .mod</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
+      <source>multiple variable %s , %s</source>
       <translation type="unfinished"/>
     </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="94"/>
-      <source>Error al crear el área:</source>
+    <message>
+      <location filename="../scripts/flreloadbatch.py" line="97"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
+      <source>Cancelar</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="66"/>
       <source>- Cargando ::</source>
       <translation type="unfinished"/>
     </message>
@@ -1581,48 +1538,91 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="238"/>
       <source>No, no acepto este acuerdo de licencia.</source>
       <translation type="unfinished"/>
     </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="31"/>
+      <location filename="../scripts/flmodules.py" line="249"/>
+      <source>Imposible cargar el módulo.
+Licencia del módulo no aceptada.</source>
+      <translation type="unfinished"/>
+    </message>
     <message>
       <location filename="../scripts/flmodules.py" line="291"/>
       <source>* Carga finalizada.</source>
       <translation type="unfinished"/>
     </message>
     <message encoding="UTF-8">
       <location filename="../scripts/flmodules.py" line="469"/>
       <source>* Exportación finalizada.</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
-      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
-      <source>single</source>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="19"/>
+      <source>Directorio de Módulos</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="34"/>
+      <source>Error al buscar los módulos en el directorio:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="52"/>
+      <source>Error al cargar el módulo:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/systype.py" line="540"/>
-      <source>Seleccionar Eneboo/Abanq Package</source>
+      <location filename="../scripts/flreloadbatch.py" line="96"/>
+      <source>Aceptar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="99"/>
+      <source>Seleccione módulos a cargar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="21"/>
+      <source>Módulo a cargar (*.mod)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="22"/>
+      <source>Módulo a cargar</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
-      <source>hola python</source>
+      <location filename="../scripts/flreloadlast.py" line="51"/>
+      <source>Error en la carga del fichero xml .mod</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="94"/>
+      <source>Error al crear el área:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
-      <source>variable %s</source>
+      <location filename="../scripts/flloadmod.py" line="23"/>
+      <source>Elegir Fichero</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="57"/>
+      <source>Este módulo depende del módulo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
-      <source>multiple variable %s , %s</source>
+      <location filename="../scripts/flloadmod.py" line="59"/>
+      <source>, que no está instalado.
+FacturaLUX puede fallar por esta causa.
+¿Desea continuar la carga?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>sys</name>
     <message>
       <location filename="../forms/sys.ui" line="0"/>
```

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.es.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.es.ts`

 * *Files 0% similar despite different names*

#### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.es.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.es.ts`

```diff
@@ -397,34 +397,97 @@
       <source>No</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Form</name>
     <message>
-      <location filename="../forms/fltest.ui" line="0"/>
-      <location filename="../forms/flmodulos.ui" line="0"/>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>Form</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Acerca de pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>iduser</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Principal</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
+
+https://github.com/deavid/pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>idgroup</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Empresas colaboradoras:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flmodulos.ui" line="0"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Librerías</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copiar al portapapeles</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Licencia</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copyright © 2012 David Martínez Martí
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the “Software”), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Cerrar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/fltest.ui" line="0"/>
       <location filename="../forms/flusers.ui" line="0"/>
-      <source>descripcion</source>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>Form</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idmodulo</source>
@@ -442,14 +505,20 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idarea</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>descripcion</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Ficheros</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>flfiles</source>
@@ -457,14 +526,24 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Log</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>iduser</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>idgroup</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>string_field</source>
@@ -496,93 +575,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>bloqueo</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Acerca de pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Principal</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
-
-https://github.com/deavid/pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Empresas colaboradoras:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Librerías</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copiar al portapapeles</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Licencia</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copyright © 2012 David Martínez Martí
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the “Software”), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Cerrar</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>MainForm</name>
     <message>
       <location filename="../../plugins/mainform/eneboo_mdi/eneboo_mdi.py" line="112"/>
       <source>Cascada</source>
       <translation type="unfinished"/>
@@ -804,15 +804,15 @@
       <source>Elegir archivo</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>PNSqlCursor</name>
     <message>
-      <location filename="../../application/database/pnsqlcursor.py" line="2352"/>
+      <location filename="../../application/database/pnsqlcursor.py" line="2354"/>
       <location filename="../../application/database/pnsqlcursor.py" line="781"/>
       <source>No hay ningún registro seleccionado</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../application/database/pnsqlcursor.py" line="793"/>
       <source>El registro activo será borrado. ¿ Está seguro ?</source>
@@ -902,14 +902,19 @@
       <location filename="../../fllegacy/tests/test_fltabledb.py" line="283"/>
       <source>Distinto de Valor</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>application</name>
+    <message>
+      <location filename="../../fllegacy/flmanager.py" line="1271"/>
+      <source>No se ha podido crear los metadatatos para la tabla %s</source>
+      <translation type="unfinished"/>
+    </message>
     <message encoding="UTF-8">
       <location filename="../../interfaces/isqldriver.py" line="360"/>
       <source>Sí</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../interfaces/isqldriver.py" line="790"/>
@@ -963,19 +968,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../plugins/sql/flqpsql.py" line="310"/>
       <source>Comprobando indices</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/flmanager.py" line="1271"/>
-      <source>No se ha podido crear los metadatatos para la tabla %s</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>ebcomportamiento</name>
     <message>
       <location filename="../forms/ebcomportamiento.ui" line="0"/>
       <source>Opciones de comportamiento</source>
       <translation type="unfinished"/>
@@ -1459,87 +1459,44 @@
       <location filename="../../fllegacy/tests/test_systype.py" line="47"/>
       <source>hola python sin group</source>
       <translation>Hola de nuevo!</translation>
     </message>
   </context>
   <context>
     <name>scripts</name>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="19"/>
-      <source>Directorio de Módulos</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="34"/>
-      <source>Error al buscar los módulos en el directorio:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="52"/>
-      <source>Error al cargar el módulo:</source>
-      <translation type="unfinished"/>
-    </message>
     <message>
-      <location filename="../scripts/flreloadbatch.py" line="96"/>
-      <source>Aceptar</source>
+      <location filename="../../fllegacy/systype.py" line="540"/>
+      <source>Seleccionar Eneboo/Abanq Package</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
-      <location filename="../scripts/flreloadbatch.py" line="97"/>
-      <source>Cancelar</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="99"/>
-      <source>Seleccione módulos a cargar</source>
-      <translation type="unfinished"/>
+      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
+      <source>hola python</source>
+      <translation>Holaaaaa</translation>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="23"/>
-      <source>Elegir Fichero</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flmodules.py" line="249"/>
-      <location filename="../scripts/flloadmod.py" line="31"/>
-      <source>Imposible cargar el módulo.
-Licencia del módulo no aceptada.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flloadmod.py" line="57"/>
-      <source>Este módulo depende del módulo</source>
-      <translation type="unfinished"/>
+      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
+      <source>single</source>
+      <translation>simple!</translation>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="59"/>
-      <source>, que no está instalado.
-FacturaLUX puede fallar por esta causa.
-¿Desea continuar la carga?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="21"/>
-      <source>Módulo a cargar (*.mod)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="22"/>
-      <source>Módulo a cargar</source>
-      <translation type="unfinished"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
+      <source>variable %s</source>
+      <translation>con variable %s!</translation>
     </message>
     <message>
-      <location filename="../scripts/flreloadlast.py" line="51"/>
-      <source>Error en la carga del fichero xml .mod</source>
-      <translation type="unfinished"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
+      <source>multiple variable %s , %s</source>
+      <translation>Test %s y %s</translation>
     </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="94"/>
-      <source>Error al crear el área:</source>
+    <message>
+      <location filename="../scripts/flreloadbatch.py" line="97"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
+      <source>Cancelar</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="66"/>
       <source>- Cargando ::</source>
       <translation type="unfinished"/>
     </message>
@@ -1585,49 +1542,92 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="238"/>
       <source>No, no acepto este acuerdo de licencia.</source>
       <translation type="unfinished"/>
     </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="31"/>
+      <location filename="../scripts/flmodules.py" line="249"/>
+      <source>Imposible cargar el módulo.
+Licencia del módulo no aceptada.</source>
+      <translation type="unfinished"/>
+    </message>
     <message>
       <location filename="../scripts/flmodules.py" line="291"/>
       <source>* Carga finalizada.</source>
       <translation type="unfinished"/>
     </message>
     <message encoding="UTF-8">
       <location filename="../scripts/flmodules.py" line="469"/>
       <source>* Exportación finalizada.</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
-      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
-      <source>single</source>
-      <translation>simple!</translation>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="19"/>
+      <source>Directorio de Módulos</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="34"/>
+      <source>Error al buscar los módulos en el directorio:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="52"/>
+      <source>Error al cargar el módulo:</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/systype.py" line="540"/>
-      <source>Seleccionar Eneboo/Abanq Package</source>
+      <location filename="../scripts/flreloadbatch.py" line="96"/>
+      <source>Aceptar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="99"/>
+      <source>Seleccione módulos a cargar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="21"/>
+      <source>Módulo a cargar (*.mod)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="22"/>
+      <source>Módulo a cargar</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
-      <source>hola python</source>
-      <translation>Holaaaaa</translation>
+      <location filename="../scripts/flreloadlast.py" line="51"/>
+      <source>Error en la carga del fichero xml .mod</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="94"/>
+      <source>Error al crear el área:</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
-      <source>variable %s</source>
-      <translation>con variable %s!</translation>
+      <location filename="../scripts/flloadmod.py" line="23"/>
+      <source>Elegir Fichero</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="57"/>
+      <source>Este módulo depende del módulo</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
-      <source>multiple variable %s , %s</source>
-      <translation>Test %s y %s</translation>
+      <location filename="../scripts/flloadmod.py" line="59"/>
+      <source>, que no está instalado.
+FacturaLUX puede fallar por esta causa.
+¿Desea continuar la carga?</source>
+      <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>sys</name>
     <message>
       <location filename="../forms/sys.ui" line="0"/>
       <source>MainWindow</source>
```

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.fr.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.fr.ts`

 * *Files 0% similar despite different names*

#### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.fr.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.fr.ts`

```diff
@@ -397,34 +397,97 @@
       <source>No</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Form</name>
     <message>
-      <location filename="../forms/fltest.ui" line="0"/>
-      <location filename="../forms/flmodulos.ui" line="0"/>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>Form</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Acerca de pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>iduser</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Principal</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
+
+https://github.com/deavid/pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>idgroup</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Empresas colaboradoras:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flmodulos.ui" line="0"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Librerías</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copiar al portapapeles</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Licencia</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copyright © 2012 David Martínez Martí
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the “Software”), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Cerrar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/fltest.ui" line="0"/>
       <location filename="../forms/flusers.ui" line="0"/>
-      <source>descripcion</source>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>Form</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idmodulo</source>
@@ -442,14 +505,20 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idarea</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>descripcion</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Ficheros</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>flfiles</source>
@@ -457,14 +526,24 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Log</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>iduser</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>idgroup</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>string_field</source>
@@ -496,93 +575,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>bloqueo</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Acerca de pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Principal</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
-
-https://github.com/deavid/pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Empresas colaboradoras:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Librerías</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copiar al portapapeles</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Licencia</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copyright © 2012 David Martínez Martí
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the “Software”), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Cerrar</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>MainForm</name>
     <message>
       <location filename="../../plugins/mainform/eneboo_mdi/eneboo_mdi.py" line="112"/>
       <source>Cascada</source>
       <translation type="unfinished"/>
@@ -800,15 +800,15 @@
       <source>Elegir archivo</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>PNSqlCursor</name>
     <message>
-      <location filename="../../application/database/pnsqlcursor.py" line="2352"/>
+      <location filename="../../application/database/pnsqlcursor.py" line="2354"/>
       <location filename="../../application/database/pnsqlcursor.py" line="781"/>
       <source>No hay ningún registro seleccionado</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../application/database/pnsqlcursor.py" line="793"/>
       <source>El registro activo será borrado. ¿ Está seguro ?</source>
@@ -898,14 +898,19 @@
       <location filename="../../fllegacy/tests/test_fltabledb.py" line="283"/>
       <source>Distinto de Valor</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>application</name>
+    <message>
+      <location filename="../../fllegacy/flmanager.py" line="1271"/>
+      <source>No se ha podido crear los metadatatos para la tabla %s</source>
+      <translation type="unfinished"/>
+    </message>
     <message encoding="UTF-8">
       <location filename="../../interfaces/isqldriver.py" line="360"/>
       <source>Sí</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../interfaces/isqldriver.py" line="790"/>
@@ -959,19 +964,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../plugins/sql/flqpsql.py" line="310"/>
       <source>Comprobando indices</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/flmanager.py" line="1271"/>
-      <source>No se ha podido crear los metadatatos para la tabla %s</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>ebcomportamiento</name>
     <message>
       <location filename="../forms/ebcomportamiento.ui" line="0"/>
       <source>Opciones de comportamiento</source>
       <translation type="unfinished"/>
@@ -1455,87 +1455,44 @@
       <location filename="../../fllegacy/tests/test_systype.py" line="47"/>
       <source>hola python sin group</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>scripts</name>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="19"/>
-      <source>Directorio de Módulos</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="34"/>
-      <source>Error al buscar los módulos en el directorio:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="52"/>
-      <source>Error al cargar el módulo:</source>
-      <translation type="unfinished"/>
-    </message>
     <message>
-      <location filename="../scripts/flreloadbatch.py" line="96"/>
-      <source>Aceptar</source>
+      <location filename="../../fllegacy/systype.py" line="540"/>
+      <source>Seleccionar Eneboo/Abanq Package</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
-      <location filename="../scripts/flreloadbatch.py" line="97"/>
-      <source>Cancelar</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="99"/>
-      <source>Seleccione módulos a cargar</source>
+      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
+      <source>hola python</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="23"/>
-      <source>Elegir Fichero</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flmodules.py" line="249"/>
-      <location filename="../scripts/flloadmod.py" line="31"/>
-      <source>Imposible cargar el módulo.
-Licencia del módulo no aceptada.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flloadmod.py" line="57"/>
-      <source>Este módulo depende del módulo</source>
+      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
+      <source>single</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="59"/>
-      <source>, que no está instalado.
-FacturaLUX puede fallar por esta causa.
-¿Desea continuar la carga?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="21"/>
-      <source>Módulo a cargar (*.mod)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="22"/>
-      <source>Módulo a cargar</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
+      <source>variable %s</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flreloadlast.py" line="51"/>
-      <source>Error en la carga del fichero xml .mod</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
+      <source>multiple variable %s , %s</source>
       <translation type="unfinished"/>
     </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="94"/>
-      <source>Error al crear el área:</source>
+    <message>
+      <location filename="../scripts/flreloadbatch.py" line="97"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
+      <source>Cancelar</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="66"/>
       <source>- Cargando ::</source>
       <translation type="unfinished"/>
     </message>
@@ -1581,48 +1538,91 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="238"/>
       <source>No, no acepto este acuerdo de licencia.</source>
       <translation type="unfinished"/>
     </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="31"/>
+      <location filename="../scripts/flmodules.py" line="249"/>
+      <source>Imposible cargar el módulo.
+Licencia del módulo no aceptada.</source>
+      <translation type="unfinished"/>
+    </message>
     <message>
       <location filename="../scripts/flmodules.py" line="291"/>
       <source>* Carga finalizada.</source>
       <translation type="unfinished"/>
     </message>
     <message encoding="UTF-8">
       <location filename="../scripts/flmodules.py" line="469"/>
       <source>* Exportación finalizada.</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
-      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
-      <source>single</source>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="19"/>
+      <source>Directorio de Módulos</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="34"/>
+      <source>Error al buscar los módulos en el directorio:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="52"/>
+      <source>Error al cargar el módulo:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/systype.py" line="540"/>
-      <source>Seleccionar Eneboo/Abanq Package</source>
+      <location filename="../scripts/flreloadbatch.py" line="96"/>
+      <source>Aceptar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="99"/>
+      <source>Seleccione módulos a cargar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="21"/>
+      <source>Módulo a cargar (*.mod)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="22"/>
+      <source>Módulo a cargar</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
-      <source>hola python</source>
+      <location filename="../scripts/flreloadlast.py" line="51"/>
+      <source>Error en la carga del fichero xml .mod</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="94"/>
+      <source>Error al crear el área:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
-      <source>variable %s</source>
+      <location filename="../scripts/flloadmod.py" line="23"/>
+      <source>Elegir Fichero</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="57"/>
+      <source>Este módulo depende del módulo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
-      <source>multiple variable %s , %s</source>
+      <location filename="../scripts/flloadmod.py" line="59"/>
+      <source>, que no está instalado.
+FacturaLUX puede fallar por esta causa.
+¿Desea continuar la carga?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>sys</name>
     <message>
       <location filename="../forms/sys.ui" line="0"/>
```

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.gl.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.gl.ts`

 * *Files 0% similar despite different names*

#### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.gl.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.gl.ts`

```diff
@@ -397,34 +397,97 @@
       <source>No</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Form</name>
     <message>
-      <location filename="../forms/fltest.ui" line="0"/>
-      <location filename="../forms/flmodulos.ui" line="0"/>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>Form</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Acerca de pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>iduser</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Principal</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
+
+https://github.com/deavid/pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>idgroup</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Empresas colaboradoras:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flmodulos.ui" line="0"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Librerías</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copiar al portapapeles</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Licencia</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copyright © 2012 David Martínez Martí
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the “Software”), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Cerrar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/fltest.ui" line="0"/>
       <location filename="../forms/flusers.ui" line="0"/>
-      <source>descripcion</source>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>Form</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idmodulo</source>
@@ -442,14 +505,20 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idarea</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>descripcion</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Ficheros</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>flfiles</source>
@@ -457,14 +526,24 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Log</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>iduser</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>idgroup</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>string_field</source>
@@ -496,93 +575,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>bloqueo</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Acerca de pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Principal</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
-
-https://github.com/deavid/pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Empresas colaboradoras:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Librerías</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copiar al portapapeles</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Licencia</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copyright © 2012 David Martínez Martí
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the “Software”), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Cerrar</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>MainForm</name>
     <message>
       <location filename="../../plugins/mainform/eneboo_mdi/eneboo_mdi.py" line="112"/>
       <source>Cascada</source>
       <translation type="unfinished"/>
@@ -800,15 +800,15 @@
       <source>Elegir archivo</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>PNSqlCursor</name>
     <message>
-      <location filename="../../application/database/pnsqlcursor.py" line="2352"/>
+      <location filename="../../application/database/pnsqlcursor.py" line="2354"/>
       <location filename="../../application/database/pnsqlcursor.py" line="781"/>
       <source>No hay ningún registro seleccionado</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../application/database/pnsqlcursor.py" line="793"/>
       <source>El registro activo será borrado. ¿ Está seguro ?</source>
@@ -898,14 +898,19 @@
       <location filename="../../fllegacy/tests/test_fltabledb.py" line="283"/>
       <source>Distinto de Valor</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>application</name>
+    <message>
+      <location filename="../../fllegacy/flmanager.py" line="1271"/>
+      <source>No se ha podido crear los metadatatos para la tabla %s</source>
+      <translation type="unfinished"/>
+    </message>
     <message encoding="UTF-8">
       <location filename="../../interfaces/isqldriver.py" line="360"/>
       <source>Sí</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../interfaces/isqldriver.py" line="790"/>
@@ -959,19 +964,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../plugins/sql/flqpsql.py" line="310"/>
       <source>Comprobando indices</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/flmanager.py" line="1271"/>
-      <source>No se ha podido crear los metadatatos para la tabla %s</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>ebcomportamiento</name>
     <message>
       <location filename="../forms/ebcomportamiento.ui" line="0"/>
       <source>Opciones de comportamiento</source>
       <translation type="unfinished"/>
@@ -1455,87 +1455,44 @@
       <location filename="../../fllegacy/tests/test_systype.py" line="47"/>
       <source>hola python sin group</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>scripts</name>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="19"/>
-      <source>Directorio de Módulos</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="34"/>
-      <source>Error al buscar los módulos en el directorio:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="52"/>
-      <source>Error al cargar el módulo:</source>
-      <translation type="unfinished"/>
-    </message>
     <message>
-      <location filename="../scripts/flreloadbatch.py" line="96"/>
-      <source>Aceptar</source>
+      <location filename="../../fllegacy/systype.py" line="540"/>
+      <source>Seleccionar Eneboo/Abanq Package</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
-      <location filename="../scripts/flreloadbatch.py" line="97"/>
-      <source>Cancelar</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="99"/>
-      <source>Seleccione módulos a cargar</source>
+      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
+      <source>hola python</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="23"/>
-      <source>Elegir Fichero</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flmodules.py" line="249"/>
-      <location filename="../scripts/flloadmod.py" line="31"/>
-      <source>Imposible cargar el módulo.
-Licencia del módulo no aceptada.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flloadmod.py" line="57"/>
-      <source>Este módulo depende del módulo</source>
+      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
+      <source>single</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="59"/>
-      <source>, que no está instalado.
-FacturaLUX puede fallar por esta causa.
-¿Desea continuar la carga?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="21"/>
-      <source>Módulo a cargar (*.mod)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="22"/>
-      <source>Módulo a cargar</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
+      <source>variable %s</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flreloadlast.py" line="51"/>
-      <source>Error en la carga del fichero xml .mod</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
+      <source>multiple variable %s , %s</source>
       <translation type="unfinished"/>
     </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="94"/>
-      <source>Error al crear el área:</source>
+    <message>
+      <location filename="../scripts/flreloadbatch.py" line="97"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
+      <source>Cancelar</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="66"/>
       <source>- Cargando ::</source>
       <translation type="unfinished"/>
     </message>
@@ -1581,48 +1538,91 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="238"/>
       <source>No, no acepto este acuerdo de licencia.</source>
       <translation type="unfinished"/>
     </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="31"/>
+      <location filename="../scripts/flmodules.py" line="249"/>
+      <source>Imposible cargar el módulo.
+Licencia del módulo no aceptada.</source>
+      <translation type="unfinished"/>
+    </message>
     <message>
       <location filename="../scripts/flmodules.py" line="291"/>
       <source>* Carga finalizada.</source>
       <translation type="unfinished"/>
     </message>
     <message encoding="UTF-8">
       <location filename="../scripts/flmodules.py" line="469"/>
       <source>* Exportación finalizada.</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
-      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
-      <source>single</source>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="19"/>
+      <source>Directorio de Módulos</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="34"/>
+      <source>Error al buscar los módulos en el directorio:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="52"/>
+      <source>Error al cargar el módulo:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/systype.py" line="540"/>
-      <source>Seleccionar Eneboo/Abanq Package</source>
+      <location filename="../scripts/flreloadbatch.py" line="96"/>
+      <source>Aceptar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="99"/>
+      <source>Seleccione módulos a cargar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="21"/>
+      <source>Módulo a cargar (*.mod)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="22"/>
+      <source>Módulo a cargar</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
-      <source>hola python</source>
+      <location filename="../scripts/flreloadlast.py" line="51"/>
+      <source>Error en la carga del fichero xml .mod</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="94"/>
+      <source>Error al crear el área:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
-      <source>variable %s</source>
+      <location filename="../scripts/flloadmod.py" line="23"/>
+      <source>Elegir Fichero</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="57"/>
+      <source>Este módulo depende del módulo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
-      <source>multiple variable %s , %s</source>
+      <location filename="../scripts/flloadmod.py" line="59"/>
+      <source>, que no está instalado.
+FacturaLUX puede fallar por esta causa.
+¿Desea continuar la carga?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>sys</name>
     <message>
       <location filename="../forms/sys.ui" line="0"/>
```

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.it.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.it.ts`

 * *Files 0% similar despite different names*

#### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.it.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.it.ts`

```diff
@@ -397,34 +397,97 @@
       <source>No</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Form</name>
     <message>
-      <location filename="../forms/fltest.ui" line="0"/>
-      <location filename="../forms/flmodulos.ui" line="0"/>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>Form</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Acerca de pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>iduser</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Principal</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
+
+https://github.com/deavid/pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>idgroup</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Empresas colaboradoras:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flmodulos.ui" line="0"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Librerías</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copiar al portapapeles</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Licencia</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copyright © 2012 David Martínez Martí
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the “Software”), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Cerrar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/fltest.ui" line="0"/>
       <location filename="../forms/flusers.ui" line="0"/>
-      <source>descripcion</source>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>Form</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idmodulo</source>
@@ -442,14 +505,20 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idarea</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>descripcion</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Ficheros</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>flfiles</source>
@@ -457,14 +526,24 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Log</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>iduser</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>idgroup</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>string_field</source>
@@ -496,93 +575,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>bloqueo</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Acerca de pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Principal</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
-
-https://github.com/deavid/pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Empresas colaboradoras:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Librerías</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copiar al portapapeles</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Licencia</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copyright © 2012 David Martínez Martí
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the “Software”), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Cerrar</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>MainForm</name>
     <message>
       <location filename="../../plugins/mainform/eneboo_mdi/eneboo_mdi.py" line="112"/>
       <source>Cascada</source>
       <translation type="unfinished"/>
@@ -800,15 +800,15 @@
       <source>Elegir archivo</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>PNSqlCursor</name>
     <message>
-      <location filename="../../application/database/pnsqlcursor.py" line="2352"/>
+      <location filename="../../application/database/pnsqlcursor.py" line="2354"/>
       <location filename="../../application/database/pnsqlcursor.py" line="781"/>
       <source>No hay ningún registro seleccionado</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../application/database/pnsqlcursor.py" line="793"/>
       <source>El registro activo será borrado. ¿ Está seguro ?</source>
@@ -898,14 +898,19 @@
       <location filename="../../fllegacy/tests/test_fltabledb.py" line="283"/>
       <source>Distinto de Valor</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>application</name>
+    <message>
+      <location filename="../../fllegacy/flmanager.py" line="1271"/>
+      <source>No se ha podido crear los metadatatos para la tabla %s</source>
+      <translation type="unfinished"/>
+    </message>
     <message encoding="UTF-8">
       <location filename="../../interfaces/isqldriver.py" line="360"/>
       <source>Sí</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../interfaces/isqldriver.py" line="790"/>
@@ -959,19 +964,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../plugins/sql/flqpsql.py" line="310"/>
       <source>Comprobando indices</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/flmanager.py" line="1271"/>
-      <source>No se ha podido crear los metadatatos para la tabla %s</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>ebcomportamiento</name>
     <message>
       <location filename="../forms/ebcomportamiento.ui" line="0"/>
       <source>Opciones de comportamiento</source>
       <translation type="unfinished"/>
@@ -1455,87 +1455,44 @@
       <location filename="../../fllegacy/tests/test_systype.py" line="47"/>
       <source>hola python sin group</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>scripts</name>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="19"/>
-      <source>Directorio de Módulos</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="34"/>
-      <source>Error al buscar los módulos en el directorio:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="52"/>
-      <source>Error al cargar el módulo:</source>
-      <translation type="unfinished"/>
-    </message>
     <message>
-      <location filename="../scripts/flreloadbatch.py" line="96"/>
-      <source>Aceptar</source>
+      <location filename="../../fllegacy/systype.py" line="540"/>
+      <source>Seleccionar Eneboo/Abanq Package</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
-      <location filename="../scripts/flreloadbatch.py" line="97"/>
-      <source>Cancelar</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="99"/>
-      <source>Seleccione módulos a cargar</source>
+      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
+      <source>hola python</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="23"/>
-      <source>Elegir Fichero</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flmodules.py" line="249"/>
-      <location filename="../scripts/flloadmod.py" line="31"/>
-      <source>Imposible cargar el módulo.
-Licencia del módulo no aceptada.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flloadmod.py" line="57"/>
-      <source>Este módulo depende del módulo</source>
+      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
+      <source>single</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="59"/>
-      <source>, que no está instalado.
-FacturaLUX puede fallar por esta causa.
-¿Desea continuar la carga?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="21"/>
-      <source>Módulo a cargar (*.mod)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="22"/>
-      <source>Módulo a cargar</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
+      <source>variable %s</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flreloadlast.py" line="51"/>
-      <source>Error en la carga del fichero xml .mod</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
+      <source>multiple variable %s , %s</source>
       <translation type="unfinished"/>
     </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="94"/>
-      <source>Error al crear el área:</source>
+    <message>
+      <location filename="../scripts/flreloadbatch.py" line="97"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
+      <source>Cancelar</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="66"/>
       <source>- Cargando ::</source>
       <translation type="unfinished"/>
     </message>
@@ -1581,48 +1538,91 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="238"/>
       <source>No, no acepto este acuerdo de licencia.</source>
       <translation type="unfinished"/>
     </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="31"/>
+      <location filename="../scripts/flmodules.py" line="249"/>
+      <source>Imposible cargar el módulo.
+Licencia del módulo no aceptada.</source>
+      <translation type="unfinished"/>
+    </message>
     <message>
       <location filename="../scripts/flmodules.py" line="291"/>
       <source>* Carga finalizada.</source>
       <translation type="unfinished"/>
     </message>
     <message encoding="UTF-8">
       <location filename="../scripts/flmodules.py" line="469"/>
       <source>* Exportación finalizada.</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
-      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
-      <source>single</source>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="19"/>
+      <source>Directorio de Módulos</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="34"/>
+      <source>Error al buscar los módulos en el directorio:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="52"/>
+      <source>Error al cargar el módulo:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/systype.py" line="540"/>
-      <source>Seleccionar Eneboo/Abanq Package</source>
+      <location filename="../scripts/flreloadbatch.py" line="96"/>
+      <source>Aceptar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="99"/>
+      <source>Seleccione módulos a cargar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="21"/>
+      <source>Módulo a cargar (*.mod)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="22"/>
+      <source>Módulo a cargar</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
-      <source>hola python</source>
+      <location filename="../scripts/flreloadlast.py" line="51"/>
+      <source>Error en la carga del fichero xml .mod</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="94"/>
+      <source>Error al crear el área:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
-      <source>variable %s</source>
+      <location filename="../scripts/flloadmod.py" line="23"/>
+      <source>Elegir Fichero</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="57"/>
+      <source>Este módulo depende del módulo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
-      <source>multiple variable %s , %s</source>
+      <location filename="../scripts/flloadmod.py" line="59"/>
+      <source>, que no está instalado.
+FacturaLUX puede fallar por esta causa.
+¿Desea continuar la carga?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>sys</name>
     <message>
       <location filename="../forms/sys.ui" line="0"/>
```

### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.pt.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.pt.ts`

 * *Files 0% similar despite different names*

#### Comparing `pineboo-0.99.80.2/pineboolib/system_module/translations/sys.pt.ts` & `pineboo-0.99.81/pineboolib/system_module/translations/sys.pt.ts`

```diff
@@ -397,34 +397,97 @@
       <source>No</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Form</name>
     <message>
-      <location filename="../forms/fltest.ui" line="0"/>
-      <location filename="../forms/flmodulos.ui" line="0"/>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>Form</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Acerca de pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>iduser</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Principal</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
+
+https://github.com/deavid/pineboo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flusers.ui" line="0"/>
-      <source>idgroup</source>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Empresas colaboradoras:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../forms/flmodulos.ui" line="0"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Librerías</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copiar al portapapeles</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Licencia</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Copyright © 2012 David Martínez Martí
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the “Software”), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
+      <source>Cerrar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/fltest.ui" line="0"/>
       <location filename="../forms/flusers.ui" line="0"/>
-      <source>descripcion</source>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>Form</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idmodulo</source>
@@ -442,14 +505,20 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>idarea</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <location filename="../forms/flmodulos.ui" line="0"/>
+      <source>descripcion</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Ficheros</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>flfiles</source>
@@ -457,14 +526,24 @@
     </message>
     <message>
       <location filename="../forms/flmodulos.ui" line="0"/>
       <source>Log</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>iduser</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../forms/flusers.ui" line="0"/>
+      <source>idgroup</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>string_field</source>
@@ -496,93 +575,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../forms/fltest.ui" line="0"/>
       <source>bloqueo</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Acerca de pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Principal</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Pineboo es un port del motor AbanQ/Eneboo a PyQt6, mantenido por la comunidad Eneboo basandose en el proyecto pineboo de: David Martínez Martí
-
-https://github.com/deavid/pineboo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Empresas colaboradoras:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>José A. Fdez Fdez (aullasistemas@gmail.com)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>YeboYebo S.L. (mail@yeboyebo.es)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Miguel J. (miguelajsmaps@gmail.com) *Documentación</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Librerías</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copiar al portapapeles</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Licencia</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Copyright © 2012 David Martínez Martí
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the “Software”), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS 
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui" line="0"/>
-      <source>Cerrar</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>MainForm</name>
     <message>
       <location filename="../../plugins/mainform/eneboo_mdi/eneboo_mdi.py" line="112"/>
       <source>Cascada</source>
       <translation type="unfinished"/>
@@ -800,15 +800,15 @@
       <source>Elegir archivo</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>PNSqlCursor</name>
     <message>
-      <location filename="../../application/database/pnsqlcursor.py" line="2352"/>
+      <location filename="../../application/database/pnsqlcursor.py" line="2354"/>
       <location filename="../../application/database/pnsqlcursor.py" line="781"/>
       <source>No hay ningún registro seleccionado</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../application/database/pnsqlcursor.py" line="793"/>
       <source>El registro activo será borrado. ¿ Está seguro ?</source>
@@ -898,14 +898,19 @@
       <location filename="../../fllegacy/tests/test_fltabledb.py" line="283"/>
       <source>Distinto de Valor</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>application</name>
+    <message>
+      <location filename="../../fllegacy/flmanager.py" line="1271"/>
+      <source>No se ha podido crear los metadatatos para la tabla %s</source>
+      <translation type="unfinished"/>
+    </message>
     <message encoding="UTF-8">
       <location filename="../../interfaces/isqldriver.py" line="360"/>
       <source>Sí</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../interfaces/isqldriver.py" line="790"/>
@@ -959,19 +964,14 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../plugins/sql/flqpsql.py" line="310"/>
       <source>Comprobando indices</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/flmanager.py" line="1271"/>
-      <source>No se ha podido crear los metadatatos para la tabla %s</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>ebcomportamiento</name>
     <message>
       <location filename="../forms/ebcomportamiento.ui" line="0"/>
       <source>Opciones de comportamiento</source>
       <translation type="unfinished"/>
@@ -1455,87 +1455,44 @@
       <location filename="../../fllegacy/tests/test_systype.py" line="47"/>
       <source>hola python sin group</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>scripts</name>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="19"/>
-      <source>Directorio de Módulos</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="34"/>
-      <source>Error al buscar los módulos en el directorio:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="52"/>
-      <source>Error al cargar el módulo:</source>
-      <translation type="unfinished"/>
-    </message>
     <message>
-      <location filename="../scripts/flreloadbatch.py" line="96"/>
-      <source>Aceptar</source>
+      <location filename="../../fllegacy/systype.py" line="540"/>
+      <source>Seleccionar Eneboo/Abanq Package</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
-      <location filename="../scripts/flreloadbatch.py" line="97"/>
-      <source>Cancelar</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadbatch.py" line="99"/>
-      <source>Seleccione módulos a cargar</source>
+      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
+      <source>hola python</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="23"/>
-      <source>Elegir Fichero</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flmodules.py" line="249"/>
-      <location filename="../scripts/flloadmod.py" line="31"/>
-      <source>Imposible cargar el módulo.
-Licencia del módulo no aceptada.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flloadmod.py" line="57"/>
-      <source>Este módulo depende del módulo</source>
+      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
+      <source>single</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flloadmod.py" line="59"/>
-      <source>, que no está instalado.
-FacturaLUX puede fallar por esta causa.
-¿Desea continuar la carga?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="21"/>
-      <source>Módulo a cargar (*.mod)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="22"/>
-      <source>Módulo a cargar</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
+      <source>variable %s</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../scripts/flreloadlast.py" line="51"/>
-      <source>Error en la carga del fichero xml .mod</source>
+      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
+      <source>multiple variable %s , %s</source>
       <translation type="unfinished"/>
     </message>
-    <message encoding="UTF-8">
-      <location filename="../scripts/flreloadlast.py" line="94"/>
-      <source>Error al crear el área:</source>
+    <message>
+      <location filename="../scripts/flreloadbatch.py" line="97"/>
+      <location filename="../../plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py" line="19"/>
+      <source>Cancelar</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="66"/>
       <source>- Cargando ::</source>
       <translation type="unfinished"/>
     </message>
@@ -1581,48 +1538,91 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../scripts/flmodules.py" line="238"/>
       <source>No, no acepto este acuerdo de licencia.</source>
       <translation type="unfinished"/>
     </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="31"/>
+      <location filename="../scripts/flmodules.py" line="249"/>
+      <source>Imposible cargar el módulo.
+Licencia del módulo no aceptada.</source>
+      <translation type="unfinished"/>
+    </message>
     <message>
       <location filename="../scripts/flmodules.py" line="291"/>
       <source>* Carga finalizada.</source>
       <translation type="unfinished"/>
     </message>
     <message encoding="UTF-8">
       <location filename="../scripts/flmodules.py" line="469"/>
       <source>* Exportación finalizada.</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="23"/>
-      <location filename="../../application/translator/test/test_pntranslator.py" line="22"/>
-      <source>single</source>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="19"/>
+      <source>Directorio de Módulos</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="34"/>
+      <source>Error al buscar los módulos en el directorio:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="52"/>
+      <source>Error al cargar el módulo:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/systype.py" line="540"/>
-      <source>Seleccionar Eneboo/Abanq Package</source>
+      <location filename="../scripts/flreloadbatch.py" line="96"/>
+      <source>Aceptar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadbatch.py" line="99"/>
+      <source>Seleccione módulos a cargar</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="21"/>
+      <source>Módulo a cargar (*.mod)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="22"/>
+      <source>Módulo a cargar</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_systype.py" line="46"/>
-      <source>hola python</source>
+      <location filename="../scripts/flreloadlast.py" line="51"/>
+      <source>Error en la carga del fichero xml .mod</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flreloadlast.py" line="94"/>
+      <source>Error al crear el área:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="24"/>
-      <source>variable %s</source>
+      <location filename="../scripts/flloadmod.py" line="23"/>
+      <source>Elegir Fichero</source>
+      <translation type="unfinished"/>
+    </message>
+    <message encoding="UTF-8">
+      <location filename="../scripts/flloadmod.py" line="57"/>
+      <source>Este módulo depende del módulo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../fllegacy/tests/test_flutil.py" line="26"/>
-      <source>multiple variable %s , %s</source>
+      <location filename="../scripts/flloadmod.py" line="59"/>
+      <source>, que no está instalado.
+FacturaLUX puede fallar por esta causa.
+¿Desea continuar la carga?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>sys</name>
     <message>
       <location filename="../forms/sys.ui" line="0"/>
```

### Comparing `pineboo-0.99.80.2/setup.py` & `pineboo-0.99.81/setup.py`

 * *Files identical despite different names*

