# Comparing `tmp/esi-leap-0.2.9.tar.gz` & `tmp/esi-leap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tzumainn/development/esi-leap/dist/tmpjopjl87r/esi-leap-0.2.9.tar", last modified: Thu Jul 13 17:57:03 2023, max compression
+gzip compressed data, was "esi-leap-0.3.0.tar", last modified: Wed Apr  3 14:10:26 2024, max compression
```

## Comparing `esi-leap-0.2.9.tar` & `esi-leap-0.3.0.tar`

### file list

```diff
@@ -1,170 +1,174 @@
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/.github/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/.github/workflows/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      604 2023-05-18 17:47:59.000000 esi-leap-0.2.9/.github/workflows/tests.yml
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/docs/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5858 2022-07-25 14:12:31.000000 esi-leap-0.2.9/docs/esi-leap-api-ref.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5962 2022-07-25 14:12:31.000000 esi-leap-0.2.9/docs/esi-leap-policy.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1176 2022-07-25 14:12:31.000000 esi-leap-0.2.9/docs/esi-leap-reporting.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8983 2022-07-25 14:12:31.000000 esi-leap-0.2.9/docs/esi-leap-requirements.md
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/api/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/api/controllers/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/api/controllers/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/api/controllers/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4170 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/api/controllers/v1/event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10348 2023-06-15 16:56:57.000000 esi-leap-0.2.9/esi_leap/api/controllers/v1/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4199 2022-09-19 15:54:31.000000 esi-leap-0.2.9/esi_leap/api/controllers/v1/node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11054 2023-05-25 15:41:42.000000 esi-leap-0.2.9/esi_leap/api/controllers/v1/offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1593 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/api/controllers/v1/root.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6501 2023-05-25 15:41:42.000000 esi-leap-0.2.9/esi_leap/api/controllers/v1/utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/api/controllers/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      928 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/api/controllers/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1424 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/api/controllers/root.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2014 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/api/controllers/types.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/api/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2060 2022-11-01 21:35:38.000000 esi-leap-0.2.9/esi_leap/api/app.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1380 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/api/service.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1032 2022-11-01 21:35:38.000000 esi-leap-0.2.9/esi_leap/api/wsgi.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/cmd/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       49 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/cmd/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1073 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/cmd/api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2928 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/cmd/dbsync.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      962 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/cmd/manager.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/common/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/common/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      603 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/common/constants.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5509 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/common/exception.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      770 2022-11-01 21:35:38.000000 esi-leap-0.2.9/esi_leap/common/i18n.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1956 2022-09-19 15:54:31.000000 esi-leap-0.2.9/esi_leap/common/ironic.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2509 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/common/keystone.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6157 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/common/notification_utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4899 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/common/policy.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3221 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/common/rpc.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1304 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/common/service.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      874 2022-08-19 19:29:16.000000 esi-leap-0.2.9/esi_leap/common/statuses.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      783 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/common/utils.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/conf/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1110 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/conf/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1058 2022-08-19 19:29:16.000000 esi-leap-0.2.9/esi_leap/conf/api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      819 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/conf/dummy_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2138 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/conf/ironic.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2154 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/conf/keystone.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      732 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/conf/netconf.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1638 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/conf/notification.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      976 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/conf/opts.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      984 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/conf/pecan.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/db/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/versions/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-07-08 14:49:10.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/versions/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2169 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/versions/a1ea63fec697_create_events_table.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      622 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-07-08 14:49:10.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1873 2022-07-08 14:49:10.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/env.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      494 2022-07-08 14:49:10.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/script.py.mako
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2180 2022-07-08 14:49:10.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic.ini
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    15049 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3140 2022-07-08 14:49:10.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/migration.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4964 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/db/sqlalchemy/models.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/db/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4131 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/db/api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      766 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/db/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1437 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/db/migration.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/manager/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/manager/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      994 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/manager/rpcapi.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5406 2022-09-19 15:54:31.000000 esi-leap-0.2.9/esi_leap/manager/service.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      944 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/manager/utils.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/objects/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      143 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/objects/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1578 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/objects/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1878 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/objects/event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2393 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/objects/fields.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13737 2023-07-13 17:54:02.000000 esi-leap-0.2.9/esi_leap/objects/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6880 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/objects/notification.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7616 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/objects/offer.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/resource_objects/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1405 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/resource_objects/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2261 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/resource_objects/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4240 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/resource_objects/dummy_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      910 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/resource_objects/error.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5560 2023-07-13 17:54:02.000000 esi-leap-0.2.9/esi_leap/resource_objects/ironic_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1491 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/resource_objects/test_node.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/api/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4017 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    34059 2023-06-15 16:56:57.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2313 2022-08-19 19:29:16.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    30769 2022-08-19 19:29:16.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    28120 2023-05-25 15:41:42.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1646 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/tests/api/controllers/test_types.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/api/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6213 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/tests/api/base.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/common/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/common/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1676 2022-09-19 15:54:31.000000 esi-leap-0.2.9/esi_leap/tests/common/test_ironic.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3594 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/tests/common/test_keystone.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3233 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/tests/common/test_notification_utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1576 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/tests/common/test_policy.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6450 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/tests/common/test_rpc.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      968 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/common/test_utils.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/db/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/db/sqlalchemy/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/db/sqlalchemy/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    32757 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/tests/db/sqlalchemy/test_api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/db/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/manager/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/manager/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8677 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/tests/manager/test_service.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/objects/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/objects/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2165 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/tests/objects/test_event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2715 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/tests/objects/test_fields.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    31005 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/tests/objects/test_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12706 2023-07-12 19:51:08.000000 esi-leap-0.2.9/esi_leap/tests/objects/test_notification.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13516 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/tests/objects/test_offer.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap/tests/resource_objects/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/resource_objects/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1950 2023-05-25 15:41:42.000000 esi-leap-0.2.9/esi_leap/tests/resource_objects/test_base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6019 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/tests/resource_objects/test_dummy_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9366 2023-07-13 17:54:02.000000 esi-leap-0.2.9/esi_leap/tests/resource_objects/test_ironic_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3966 2023-05-25 15:41:42.000000 esi-leap-0.2.9/esi_leap/tests/resource_objects/test_resource_objects.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2986 2023-06-08 21:26:09.000000 esi-leap-0.2.9/esi_leap/tests/resource_objects/test_test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/tests/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2563 2022-07-25 14:12:31.000000 esi-leap-0.2.9/esi_leap/tests/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      645 2022-05-25 19:28:05.000000 esi-leap-0.2.9/esi_leap/version.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap.egg-info/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6494 2023-07-13 17:57:02.000000 esi-leap-0.2.9/esi_leap.egg-info/PKG-INFO
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4346 2023-07-13 17:57:03.000000 esi-leap-0.2.9/esi_leap.egg-info/SOURCES.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2023-07-13 17:57:02.000000 esi-leap-0.2.9/esi_leap.egg-info/dependency_links.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      508 2023-07-13 17:57:02.000000 esi-leap-0.2.9/esi_leap.egg-info/entry_points.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-05-25 19:49:35.000000 esi-leap-0.2.9/esi_leap.egg-info/not-zip-safe
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2023-07-13 17:57:02.000000 esi-leap-0.2.9/esi_leap.egg-info/pbr.json
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      805 2023-07-13 17:57:02.000000 esi-leap-0.2.9/esi_leap.egg-info/requires.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        9 2023-07-13 17:57:02.000000 esi-leap-0.2.9/esi_leap.egg-info/top_level.txt
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/etc/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-07-13 17:57:03.000000 esi-leap-0.2.9/etc/esi-leap/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      395 2022-05-25 19:28:05.000000 esi-leap-0.2.9/etc/esi-leap/esi-leap-config-generator.conf
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       77 2022-05-25 19:28:05.000000 esi-leap-0.2.9/etc/esi-leap/esi-leap-policy-generator.conf
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       63 2022-05-25 19:28:05.000000 esi-leap-0.2.9/.stestr.conf
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      548 2023-07-13 17:57:02.000000 esi-leap-0.2.9/AUTHORS
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9574 2023-07-13 17:57:02.000000 esi-leap-0.2.9/ChangeLog
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      680 2023-05-25 15:41:42.000000 esi-leap-0.2.9/Containerfile
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10143 2022-05-25 19:28:05.000000 esi-leap-0.2.9/LICENSE
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5478 2023-05-25 15:41:42.000000 esi-leap-0.2.9/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       17 2022-05-25 19:28:05.000000 esi-leap-0.2.9/babel.cfg
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1410 2023-07-12 19:51:08.000000 esi-leap-0.2.9/requirements.txt
--rwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)      777 2023-05-25 15:41:42.000000 esi-leap-0.2.9/run_services.sh
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1364 2023-07-13 17:57:03.000000 esi-leap-0.2.9/setup.cfg
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      597 2022-06-16 17:07:25.000000 esi-leap-0.2.9/setup.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      750 2023-06-08 21:26:09.000000 esi-leap-0.2.9/test-requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1648 2023-05-18 17:47:59.000000 esi-leap-0.2.9/tox.ini
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6494 2023-07-13 17:57:03.000000 esi-leap-0.2.9/PKG-INFO
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.751906 esi-leap-0.3.0/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.737906 esi-leap-0.3.0/.github/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.739906 esi-leap-0.3.0/.github/workflows/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      597 2024-03-18 18:51:34.000000 esi-leap-0.3.0/.github/workflows/tests.yml
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       63 2022-05-25 19:28:05.000000 esi-leap-0.3.0/.stestr.conf
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      548 2024-04-03 14:10:25.000000 esi-leap-0.3.0/AUTHORS
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10010 2024-04-03 14:10:25.000000 esi-leap-0.3.0/ChangeLog
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      680 2024-03-18 18:51:34.000000 esi-leap-0.3.0/Containerfile
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10143 2022-05-25 19:28:05.000000 esi-leap-0.3.0/LICENSE
+-rw-r--r--   0 tzumainn  (3390) tzumainn  (3390)     7821 2024-04-03 14:10:26.751906 esi-leap-0.3.0/PKG-INFO
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5475 2024-03-26 13:08:14.000000 esi-leap-0.3.0/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       17 2022-05-25 19:28:05.000000 esi-leap-0.3.0/babel.cfg
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.740906 esi-leap-0.3.0/docs/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5858 2024-03-18 18:51:34.000000 esi-leap-0.3.0/docs/esi-leap-api-ref.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5962 2024-03-18 18:51:34.000000 esi-leap-0.3.0/docs/esi-leap-policy.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1176 2024-03-18 18:51:34.000000 esi-leap-0.3.0/docs/esi-leap-reporting.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8983 2024-03-18 18:51:34.000000 esi-leap-0.3.0/docs/esi-leap-requirements.md
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.740906 esi-leap-0.3.0/esi_leap/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.741906 esi-leap-0.3.0/esi_leap/api/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/api/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2060 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/api/app.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.742906 esi-leap-0.3.0/esi_leap/api/controllers/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/api/controllers/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      928 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/api/controllers/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1424 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/api/controllers/root.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2014 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/api/controllers/types.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.742906 esi-leap-0.3.0/esi_leap/api/controllers/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/api/controllers/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4170 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/api/controllers/v1/event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11525 2024-04-03 14:08:53.000000 esi-leap-0.3.0/esi_leap/api/controllers/v1/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4525 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/api/controllers/v1/node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11174 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/api/controllers/v1/offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1593 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/api/controllers/v1/root.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7104 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/api/controllers/v1/utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1380 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/api/service.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1032 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/api/wsgi.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.743906 esi-leap-0.3.0/esi_leap/cmd/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       49 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/cmd/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1073 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/cmd/api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2928 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/cmd/dbsync.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      962 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/cmd/manager.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.743906 esi-leap-0.3.0/esi_leap/common/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/common/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      603 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/common/constants.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5928 2024-04-03 14:08:53.000000 esi-leap-0.3.0/esi_leap/common/exception.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      770 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/common/i18n.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2139 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/common/ironic.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2509 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/common/keystone.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6157 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/common/notification_utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5080 2024-04-03 14:08:53.000000 esi-leap-0.3.0/esi_leap/common/policy.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3221 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/common/rpc.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1304 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/common/service.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      874 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/common/statuses.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      783 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/common/utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.744906 esi-leap-0.3.0/esi_leap/conf/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1110 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1153 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      819 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/dummy_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2138 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/ironic.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2154 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/keystone.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      732 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/netconf.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1638 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/notification.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      976 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/opts.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      984 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/conf/pecan.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.745906 esi-leap-0.3.0/esi_leap/db/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/db/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4127 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/db/api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      766 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/db/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1437 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/db/migration.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.745906 esi-leap-0.3.0/esi_leap/db/sqlalchemy/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.745906 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      622 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-07-08 14:49:10.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1873 2022-07-08 14:49:10.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/env.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      494 2022-07-08 14:49:10.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/script.py.mako
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.746906 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-07-08 14:49:10.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/versions/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2169 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/versions/a1ea63fec697_create_events_table.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2180 2022-07-08 14:49:10.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic.ini
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    15106 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3140 2022-07-08 14:49:10.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/migration.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4964 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/db/sqlalchemy/models.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.746906 esi-leap-0.3.0/esi_leap/manager/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/manager/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      994 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/manager/rpcapi.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5406 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/manager/service.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      944 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/manager/utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.747906 esi-leap-0.3.0/esi_leap/objects/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      143 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/objects/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1578 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/objects/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1878 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/objects/event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2393 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/objects/fields.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    15116 2024-04-03 14:08:53.000000 esi-leap-0.3.0/esi_leap/objects/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6880 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/objects/notification.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7635 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/objects/offer.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.747906 esi-leap-0.3.0/esi_leap/resource_objects/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1405 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/resource_objects/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2284 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/resource_objects/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4269 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/resource_objects/dummy_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      914 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/resource_objects/error.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5726 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/resource_objects/ironic_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1515 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/resource_objects/test_node.py
+-rwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)     6731 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/send_email_notification.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.748906 esi-leap-0.3.0/esi_leap/templates/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      281 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/templates/lease_create_email.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      357 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/templates/lease_expire_email.txt
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.748906 esi-leap-0.3.0/esi_leap/tests/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.748906 esi-leap-0.3.0/esi_leap/tests/api/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/api/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7200 2024-04-03 14:08:53.000000 esi-leap-0.3.0/esi_leap/tests/api/base.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.748906 esi-leap-0.3.0/esi_leap/tests/api/controllers/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/api/controllers/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1646 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/api/controllers/test_types.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.749906 esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4017 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    36899 2024-04-03 14:08:53.000000 esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2528 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    30769 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    30319 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2563 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/base.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.749906 esi-leap-0.3.0/esi_leap/tests/common/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/common/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2142 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/tests/common/test_ironic.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3594 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/common/test_keystone.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3233 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/common/test_notification_utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1576 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/common/test_policy.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6450 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/common/test_rpc.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      968 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/common/test_utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.749906 esi-leap-0.3.0/esi_leap/tests/db/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/db/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.749906 esi-leap-0.3.0/esi_leap/tests/db/sqlalchemy/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    33148 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/db/sqlalchemy/test_api.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.750906 esi-leap-0.3.0/esi_leap/tests/manager/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/manager/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8677 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/manager/test_service.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.750906 esi-leap-0.3.0/esi_leap/tests/objects/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/objects/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2165 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/objects/test_event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2715 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/objects/test_fields.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    34374 2024-04-03 14:08:53.000000 esi-leap-0.3.0/esi_leap/tests/objects/test_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12706 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/objects/test_notification.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13516 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/objects/test_offer.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.751906 esi-leap-0.3.0/esi_leap/tests/resource_objects/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/tests/resource_objects/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1950 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/resource_objects/test_base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6026 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/tests/resource_objects/test_dummy_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9503 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/tests/resource_objects/test_ironic_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3966 2024-03-18 18:51:34.000000 esi-leap-0.3.0/esi_leap/tests/resource_objects/test_resource_objects.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2994 2024-03-26 13:08:14.000000 esi-leap-0.3.0/esi_leap/tests/resource_objects/test_test_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      645 2022-05-25 19:28:05.000000 esi-leap-0.3.0/esi_leap/version.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.751906 esi-leap-0.3.0/esi_leap.egg-info/
+-rw-r--r--   0 tzumainn  (3390) tzumainn  (3390)     7821 2024-04-03 14:10:25.000000 esi-leap-0.3.0/esi_leap.egg-info/PKG-INFO
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4466 2024-04-03 14:10:26.000000 esi-leap-0.3.0/esi_leap.egg-info/SOURCES.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-04-03 14:10:25.000000 esi-leap-0.3.0/esi_leap.egg-info/dependency_links.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      575 2024-04-03 14:10:25.000000 esi-leap-0.3.0/esi_leap.egg-info/entry_points.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-05-25 19:49:35.000000 esi-leap-0.3.0/esi_leap.egg-info/not-zip-safe
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2024-04-03 14:10:25.000000 esi-leap-0.3.0/esi_leap.egg-info/pbr.json
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      832 2024-04-03 14:10:25.000000 esi-leap-0.3.0/esi_leap.egg-info/requires.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        9 2024-04-03 14:10:25.000000 esi-leap-0.3.0/esi_leap.egg-info/top_level.txt
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.738906 esi-leap-0.3.0/etc/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:10:26.751906 esi-leap-0.3.0/etc/esi-leap/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      395 2022-05-25 19:28:05.000000 esi-leap-0.3.0/etc/esi-leap/esi-leap-config-generator.conf
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       77 2022-05-25 19:28:05.000000 esi-leap-0.3.0/etc/esi-leap/esi-leap-policy-generator.conf
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1410 2024-03-18 18:51:34.000000 esi-leap-0.3.0/requirements.txt
+-rwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)      777 2024-03-18 18:51:34.000000 esi-leap-0.3.0/run_services.sh
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1433 2024-04-03 14:10:26.757906 esi-leap-0.3.0/setup.cfg
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      645 2024-03-18 18:51:34.000000 esi-leap-0.3.0/setup.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      750 2024-03-18 18:51:34.000000 esi-leap-0.3.0/test-requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1648 2024-03-18 18:51:34.000000 esi-leap-0.3.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `esi-leap-0.2.9/.github/workflows/tests.yml` & `esi-leap-0.3.0/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-20.04
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `esi-leap-0.2.9/docs/esi-leap-api-ref.md` & `esi-leap-0.3.0/docs/esi-leap-api-ref.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/docs/esi-leap-policy.md` & `esi-leap-0.3.0/docs/esi-leap-policy.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/docs/esi-leap-reporting.md` & `esi-leap-0.3.0/docs/esi-leap-reporting.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/docs/esi-leap-requirements.md` & `esi-leap-0.3.0/docs/esi-leap-requirements.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/v1/event.py` & `esi-leap-0.3.0/esi_leap/api/controllers/v1/event.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/v1/lease.py` & `esi-leap-0.3.0/esi_leap/api/controllers/v1/lease.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     project_id = wsme.wsattr(wtypes.text)
     project = wsme.wsattr(wtypes.text, readonly=True)
     owner_id = wsme.wsattr(wtypes.text, readonly=True)
     owner = wsme.wsattr(wtypes.text, readonly=True)
     resource_type = wsme.wsattr(wtypes.text)
     resource_uuid = wsme.wsattr(wtypes.text)
     resource_class = wsme.wsattr(wtypes.text)
+    resource_properties = {wtypes.text: types.jsontype}
     resource = wsme.wsattr(wtypes.text, readonly=True)
     start_time = wsme.wsattr(datetime.datetime)
     fulfill_time = wsme.wsattr(datetime.datetime, readonly=True)
     expire_time = wsme.wsattr(datetime.datetime, readonly=True)
     end_time = wsme.wsattr(datetime.datetime)
     status = wsme.wsattr(wtypes.text, readonly=True)
     properties = {wtypes.text: types.jsontype}
@@ -58,15 +59,16 @@
     parent_lease_uuid = wsme.wsattr(wtypes.text, readonly=True)
 
     def __init__(self, **kwargs):
         self.fields = lease_obj.Lease.fields
         for field in self.fields:
             setattr(self, field, kwargs.get(field, wtypes.Unset))
 
-        for attr in ('project', 'owner', 'resource', 'resource_class'):
+        for attr in ('project', 'owner', 'resource', 'resource_class',
+                     'resource_properties'):
             setattr(self, attr, kwargs.get(attr, wtypes.Unset))
 
 
 class LeaseCollection(types.Collection):
     leases = [Lease]
 
     def __init__(self, **kwargs):
@@ -160,15 +162,21 @@
             lease_dict['project_id'] = keystone.get_project_uuid_from_ident(
                 lease_dict['project_id'])
 
         if 'start_time' not in lease_dict:
             lease_dict['start_time'] = datetime.datetime.now()
 
         if 'end_time' not in lease_dict:
-            lease_dict['end_time'] = datetime.datetime.max
+            lease_dict['end_time'] = lease_dict['start_time'] + \
+                datetime.timedelta(days=CONF.api.default_lease_time)
+        else:
+            utils.check_lease_length(cdict,
+                                     lease_dict['start_time'],
+                                     lease_dict['end_time'],
+                                     CONF.api.max_lease_time)
 
         try:
             utils.check_resource_admin(cdict, resource, request.project_id)
         except exception.HTTPResourceForbidden:
             parent_lease_uuid = utils.check_resource_lease_admin(
                 cdict,
                 resource,
@@ -179,14 +187,33 @@
                 raise
             lease_dict['parent_lease_uuid'] = parent_lease_uuid
 
         lease = lease_obj.Lease(**lease_dict)
         lease.create(request)
         return Lease(**utils.lease_get_dict_with_added_info(lease))
 
+    @wsme_pecan.wsexpose(Lease, wtypes.text, body={wtypes.text: wtypes.text})
+    def patch(self, lease_uuid, patch=None):
+        request = pecan.request.context
+
+        lease = utils.check_lease_policy_and_retrieve(
+            request, 'esi_leap:lease:update', lease_uuid)
+
+        # check that patch has acceptable fields; only end_time for now
+        patch_keys = patch.keys()
+        if not('end_time' in patch_keys and len(patch_keys) == 1):
+            raise exception.LeaseInvalidPatch()
+
+        new_end_time = datetime.datetime.strptime(
+            patch['end_time'], '%Y-%m-%dT%H:%M:%S')
+        updates = {'end_time': new_end_time}
+        lease.update(updates, request)
+
+        return Lease(**utils.lease_get_dict_with_added_info(lease))
+
     @wsme_pecan.wsexpose(Lease, wtypes.text)
     def delete(self, lease_id):
         request = pecan.request.context
 
         lease = utils.check_lease_policy_and_retrieve(
             request, 'esi_leap:lease:get', lease_id,
             statuses.LEASE_CAN_DELETE)
```

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/v1/node.py` & `esi-leap-0.3.0/esi_leap/api/controllers/v1/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,25 +32,28 @@
 
 class Node(base.ESILEAPBase):
 
     name = wsme.wsattr(wtypes.text)
     owner = wsme.wsattr(wtypes.text)
     maintenance = wsme.wsattr(wtypes.text)
     provision_state = wsme.wsattr(wtypes.text)
+    properties = {wtypes.text: types.jsontype}
+    resource_class = wsme.wsattr(wtypes.text)
     uuid = wsme.wsattr(wtypes.text)
     offer_uuid = wsme.wsattr(wtypes.text)
     lease_uuid = wsme.wsattr(wtypes.text)
     lessee = wsme.wsattr(wtypes.text)
     future_offers = wsme.wsattr(wtypes.text)
     future_leases = wsme.wsattr(wtypes.text)
 
     def __init__(self, **kwargs):
         self.fields = ('name', 'owner', 'uuid', 'offer_uuid', 'lease_uuid',
                        'lessee', 'future_offers', 'future_leases',
-                       'provision_state', 'maintenance')
+                       'resource_class', 'provision_state', 'maintenance',
+                       'properties')
         for field in self.fields:
             setattr(self, field, kwargs.get(field, wtypes.Unset))
 
 
 class NodeCollection(types.Collection):
     nodes = [Node]
 
@@ -99,14 +102,17 @@
             future_offers = ' '.join(future_offers)
 
             f_lease_uuids = ''.join([lease.uuid for lease in leases
                                      if lease.resource_uuid == node.uuid])
 
             n = Node(name=node.name, uuid=node.uuid,
                      provision_state=node.provision_state,
+                     resource_class=node.resource_class,
+                     properties=ironic.get_condensed_properties(
+                         node.properties, node.traits),
                      maintenance=str(node.maintenance),
                      owner=keystone.get_project_name(node.owner, project_list),
                      lessee=keystone.get_project_name(node.lessee,
                                                       project_list),
                      future_offers=future_offers,
                      future_leases=f_lease_uuids)
```

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/v1/offer.py` & `esi-leap-0.3.0/esi_leap/api/controllers/v1/offer.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,29 +44,31 @@
     project = wsme.wsattr(wtypes.text, readonly=True)
     lessee_id = wsme.wsattr(wtypes.text)
     lessee = wsme.wsattr(wtypes.text, readonly=True)
     resource_type = wsme.wsattr(wtypes.text)
     resource_uuid = wsme.wsattr(wtypes.text, mandatory=True)
     resource = wsme.wsattr(wtypes.text, readonly=True)
     resource_class = wsme.wsattr(wtypes.text)
+    resource_properties = {wtypes.text: types.jsontype}
     start_time = wsme.wsattr(datetime.datetime)
     end_time = wsme.wsattr(datetime.datetime)
     status = wsme.wsattr(wtypes.text, readonly=True)
     properties = {wtypes.text: types.jsontype}
     availabilities = wsme.wsattr([[datetime.datetime]], readonly=True)
     parent_lease_uuid = wsme.wsattr(wtypes.text, readonly=True)
 
     def __init__(self, **kwargs):
 
         self.fields = offer_obj.Offer.fields
         for field in self.fields:
             setattr(self, field, kwargs.get(field, wtypes.Unset))
 
         for attr in ('availabilities', 'project', 'lessee',
-                     'resource', 'resource_class'):
+                     'resource', 'resource_class',
+                     'resource_properties'):
             setattr(self, attr, kwargs.get(attr, wtypes.Unset))
 
 
 class OfferCollection(types.Collection):
     offers = [Offer]
 
     def __init__(self, **kwargs):
@@ -268,15 +270,16 @@
         if offer.parent_lease_uuid is not None:
             lease_dict['parent_lease_uuid'] = offer.parent_lease_uuid
 
         if 'start_time' not in lease_dict:
             lease_dict['start_time'] = datetime.datetime.now()
 
         if 'end_time' not in lease_dict:
-            q = offer.get_first_availability(lease_dict['start_time'])
+            q = offer.get_next_lease_start_time(
+                lease_dict['start_time'])
             if q is None:
                 lease_dict['end_time'] = offer.end_time
             else:
                 lease_dict['end_time'] = q.start_time
 
         new_lease = lease_obj.Lease(**lease_dict)
         new_lease.create(request)
```

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/v1/root.py` & `esi-leap-0.3.0/esi_leap/api/controllers/v1/root.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/v1/utils.py` & `esi-leap-0.3.0/esi_leap/api/controllers/v1/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from oslo_policy import policy as oslo_policy
 from oslo_utils import uuidutils
 
+import datetime
+
 from esi_leap.common import exception
 from esi_leap.common import keystone
 from esi_leap.common import policy
 from esi_leap.objects import lease as lease_obj
 from esi_leap.objects import offer as offer_obj
 
 
@@ -149,21 +151,33 @@
 
     o = offer.to_dict()
     o['availabilities'] = offer.get_availabilities()
     o['project'] = keystone.get_project_name(offer.project_id, project_list)
     o['lessee'] = keystone.get_project_name(offer.lessee_id, project_list)
     o['resource'] = resource.get_name(node_list)
     o['resource_class'] = resource.get_resource_class(node_list)
+    o['resource_properties'] = resource.get_properties(node_list)
     return o
 
 
 def lease_get_dict_with_added_info(lease, project_list=None, node_list=None):
     resource = lease.resource_object()
 
     lease_dict = lease.to_dict()
     lease_dict['project'] = keystone.get_project_name(lease.project_id,
                                                       project_list)
     lease_dict['owner'] = keystone.get_project_name(lease.owner_id,
                                                     project_list)
     lease_dict['resource'] = resource.get_name(node_list)
     lease_dict['resource_class'] = resource.get_resource_class(node_list)
+    lease_dict['resource_properties'] = resource.get_properties(node_list)
     return lease_dict
+
+
+def check_lease_length(cdict, start_time, end_time, max_time):
+    if (end_time - start_time) > datetime.timedelta(days=max_time):
+        # Check if the current project is admin
+        # Only admin project can set a lease beyond the max length
+        try:
+            policy_authorize('esi_leap:lease:lease_admin', cdict, cdict)
+        except exception.HTTPForbidden:
+            raise exception.LeaseExceedMaxTimeRange(max_time=max_time)
```

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/base.py` & `esi-leap-0.3.0/esi_leap/api/controllers/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/root.py` & `esi-leap-0.3.0/esi_leap/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/api/controllers/types.py` & `esi-leap-0.3.0/esi_leap/api/controllers/types.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/api/app.py` & `esi-leap-0.3.0/esi_leap/api/app.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/api/service.py` & `esi-leap-0.3.0/esi_leap/api/service.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/api/wsgi.py` & `esi-leap-0.3.0/esi_leap/api/wsgi.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/cmd/api.py` & `esi-leap-0.3.0/esi_leap/cmd/api.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/cmd/dbsync.py` & `esi-leap-0.3.0/esi_leap/cmd/dbsync.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/cmd/manager.py` & `esi-leap-0.3.0/esi_leap/cmd/manager.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/common/constants.py` & `esi-leap-0.3.0/esi_leap/common/constants.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/common/exception.py` & `esi-leap-0.3.0/esi_leap/common/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,24 @@
             except Exception:
                 message = self.msg_fmt
 
         self.message = message
         super(ESILeapException, self).__init__(message)
 
 
+class LeaseExceedMaxTimeRange(ESILeapException):
+    code = http_client.FORBIDDEN
+    msg_fmt = _('Attempted to create lease with an invalid '
+                'time range. The max time range is %(max_time)s days.')
+
+
+class LeaseInvalidPatch(ESILeapException):
+    msg_fmt = _('Only the end_time field may be updated')
+
+
 class HTTPForbidden(ESILeapException):
     code = http_client.FORBIDDEN
     msg_fmt = _('Access was denied to %(rule)s.')
 
 
 class HTTPResourceForbidden(ESILeapException):
     code = http_client.FORBIDDEN
@@ -59,14 +69,15 @@
 
 
 class LeaseNotActive(ESILeapException):
     msg_fmt = _('Lease with name or uuid %(lease_id)s not active.')
 
 
 class LeaseNotFound(ESILeapException):
+    code = http_client.NOT_FOUND
     msg_fmt = _('Lease with name or uuid %(lease_id)s not found.')
 
 
 class LeaseNoOfferUUID(ESILeapException):
     msg_fmt = _('Cannot create lease without parameter offer_uuid.')
 
 
@@ -81,14 +92,15 @@
 
 
 class OfferDuplicateName(ESILeapException):
     msg_fmt = _('Duplicate offers with name %(name)s.')
 
 
 class OfferNotFound(ESILeapException):
+    code = http_client.NOT_FOUND
     msg_fmt = _('Offer with name or uuid %(offer_uuid)s not found.')
 
 
 class OfferNoTimeAvailabilities(ESILeapException):
     msg_fmt = _('Offer %(offer_uuid)s has no availabilities at given '
                 'time range %(start_time)s, %(end_time)s.')
 
@@ -143,14 +155,15 @@
 class InvalidTimeRange(ESILeapException):
     msg_fmt = _('Attempted to create %(resource)s resource with an invalid '
                 'Start Time and End Time. Start Time must be strictly less '
                 'than End Time. Got %(start_time)s, %(end_time)s.')
 
 
 class NodeNotFound(ESILeapException):
+    code = http_client.NOT_FOUND
     msg_fmt = _('Encountered an error fetching info for node %(uuid)s '
                 '(%(resource_type)s): %(err)s')
 
 
 class NotificationPayloadError(ESILeapException):
     _msg_fmt = _("Payload not populated when trying to send notification "
                  "\"%(class_name)s\"")
```

### Comparing `esi-leap-0.2.9/esi_leap/common/i18n.py` & `esi-leap-0.3.0/esi_leap/common/i18n.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/common/ironic.py` & `esi-leap-0.3.0/esi_leap/common/ironic.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,7 +49,15 @@
 
 def get_node(node_uuid, node_list=None):
     if node_list is None:
         node = get_ironic_client().node.get(node_uuid)
     else:
         node = next((n for n in node_list if n.uuid == node_uuid), None)
     return node
+
+
+def get_condensed_properties(properties, traits):
+    cp = properties.copy()
+    cp.pop('lease_uuid', None)
+    cp.pop('capabilities', None)
+    cp['traits'] = traits
+    return cp
```

### Comparing `esi-leap-0.2.9/esi_leap/common/keystone.py` & `esi-leap-0.3.0/esi_leap/common/keystone.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/common/notification_utils.py` & `esi-leap-0.3.0/esi_leap/common/notification_utils.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/common/policy.py` & `esi-leap-0.3.0/esi_leap/common/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,19 @@
          {'path': '/leases/{lease_ident}', 'method': 'DELETE'}]),
     policy.DocumentedRuleDefault(
         'esi_leap:lease:create',
         'rule:is_admin or rule:is_owner',
         'Create lease',
         [{'path': '/leases', 'method': 'POST'}]),
     policy.DocumentedRuleDefault(
+        'esi_leap:lease:update',
+        'rule:is_admin',
+        'Update lease',
+        [{'path': '/leases/{lease_ident}', 'method': 'PATCH'}]),
+    policy.DocumentedRuleDefault(
         'esi_leap:lease:get',
         'rule:is_admin or rule:is_lease_owner or rule:is_lease_lessee',
         'Retrieve a single lease',
         [{'path': '/leases/{lease_ident}', 'method': 'GET'}]),
     policy.DocumentedRuleDefault(
         'esi_leap:lease:get_all',
         'rule:is_admin or rule:is_owner or rule:is_lessee',
```

### Comparing `esi-leap-0.2.9/esi_leap/common/rpc.py` & `esi-leap-0.3.0/esi_leap/common/rpc.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/common/service.py` & `esi-leap-0.3.0/esi_leap/common/service.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/common/statuses.py` & `esi-leap-0.3.0/esi_leap/common/statuses.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/common/utils.py` & `esi-leap-0.3.0/esi_leap/common/utils.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/conf/__init__.py` & `esi-leap-0.3.0/esi_leap/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/conf/api.py` & `esi-leap-0.3.0/esi_leap/conf/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     cfg.HostAddressOpt('host_ip', default='0.0.0.0'),
     cfg.PortOpt('port', default=7777),
     cfg.IntOpt('max_limit', default=1000),
     cfg.StrOpt('public_endpoint'),
     cfg.IntOpt('api_workers'),
     cfg.BoolOpt('enable_ssl_api', default=False),
     cfg.StrOpt('default_resource_type', default='ironic_node'),
+    cfg.IntOpt('max_lease_time', default=21),
+    cfg.IntOpt('default_lease_time', default=7),
 ]
 
 
 api_group = cfg.OptGroup('api', title='API Options')
 
 
 def register_opts(conf):
```

### Comparing `esi-leap-0.2.9/esi_leap/conf/dummy_node.py` & `esi-leap-0.3.0/esi_leap/conf/dummy_node.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/conf/ironic.py` & `esi-leap-0.3.0/esi_leap/conf/ironic.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/conf/keystone.py` & `esi-leap-0.3.0/esi_leap/conf/keystone.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/conf/netconf.py` & `esi-leap-0.3.0/esi_leap/conf/netconf.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/conf/notification.py` & `esi-leap-0.3.0/esi_leap/conf/notification.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/conf/opts.py` & `esi-leap-0.3.0/esi_leap/conf/opts.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/conf/pecan.py` & `esi-leap-0.3.0/esi_leap/conf/pecan.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/versions/a1ea63fec697_create_events_table.py` & `esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/versions/a1ea63fec697_create_events_table.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/README.md` & `esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/README.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic/env.py` & `esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/db/sqlalchemy/alembic.ini` & `esi-leap-0.3.0/esi_leap/db/sqlalchemy/alembic.ini`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/db/sqlalchemy/api.py` & `esi-leap-0.3.0/esi_leap/db/sqlalchemy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,25 +165,26 @@
         order_by(models.Lease.start_time).\
         filter(models.Lease.offer_uuid == offer_ref.uuid,
                (models.Lease.status != statuses.EXPIRED) &
                (models.Lease.status != statuses.DELETED)
                ).all()
 
 
-def offer_get_first_availability(offer_uuid, start):
+def offer_get_next_lease_start_time(offer_uuid, start):
     l_query = model_query(models.Lease)
 
     return l_query.with_entities(
         models.Lease.start_time).\
         filter(models.Lease.offer_uuid == offer_uuid,
                (models.Lease.status == statuses.CREATED) |
                (models.Lease.status == statuses.ACTIVE)
                ).\
         order_by(models.Lease.start_time).\
-        filter(models.Lease.end_time >= start).first()
+        filter((models.Lease.end_time >= start) &
+               (models.Lease.start_time >= start)).first()
 
 
 def offer_verify_availability(offer_ref, start, end):
 
     if start < offer_ref.start_time or end > offer_ref.end_time:
         raise exception.OfferNoTimeAvailabilities(offer_uuid=offer_ref.uuid,
                                                   start_time=start,
```

### Comparing `esi-leap-0.2.9/esi_leap/db/sqlalchemy/migration.py` & `esi-leap-0.3.0/esi_leap/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/db/sqlalchemy/models.py` & `esi-leap-0.3.0/esi_leap/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/db/api.py` & `esi-leap-0.3.0/esi_leap/db/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,17 +88,17 @@
 
 
 @to_dict
 def offer_get_conflict_times(offer_ref):
     return IMPL.offer_get_conflict_times(offer_ref)
 
 
-def offer_get_first_availability(offer_uuid, start, end):
-    return IMPL.offer_get_first_availability(
-        offer_uuid, start, end)
+def offer_get_next_lease_start_time(offer_uuid, start):
+    return IMPL.offer_get_next_lease_start_time(
+        offer_uuid, start)
 
 
 def offer_verify_availability(offer_ref, start, end):
     return IMPL.offer_verify_availability(
         offer_ref, start, end)
```

### Comparing `esi-leap-0.2.9/esi_leap/db/base.py` & `esi-leap-0.3.0/esi_leap/db/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/db/migration.py` & `esi-leap-0.3.0/esi_leap/db/migration.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/manager/rpcapi.py` & `esi-leap-0.3.0/esi_leap/manager/rpcapi.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/manager/service.py` & `esi-leap-0.3.0/esi_leap/manager/service.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/manager/utils.py` & `esi-leap-0.3.0/esi_leap/manager/utils.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/objects/base.py` & `esi-leap-0.3.0/esi_leap/objects/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/objects/event.py` & `esi-leap-0.3.0/esi_leap/objects/event.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/objects/fields.py` & `esi-leap-0.3.0/esi_leap/objects/fields.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/objects/lease.py` & `esi-leap-0.3.0/esi_leap/objects/lease.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,17 +96,17 @@
 
     def __init__(self, lease, node):
         super(LeaseCRUDPayload, self).__init__()
 
         setattr(node, 'node_name', node.get_name())
         setattr(node, 'node_provision_state', node.get_node_provision_state())
         setattr(node, 'node_power_state', node.get_node_power_state())
-        node_config = node.get_config().copy()
-        node_config.pop('lease_uuid', None)
-        setattr(node, 'node_properties', node_config)
+        node_properties = node.get_properties().copy()
+        node_properties.pop('lease_uuid', None)
+        setattr(node, 'node_properties', node_properties)
 
         self.populate_schema(lease=lease, node=node)
 
     def get_event_dict(self, event_type):
         event_dict = super().get_event_dict(event_type)
         event_dict.update({
             'object_type': 'lease',
@@ -156,55 +156,56 @@
     @classmethod
     def get_all(cls, filters, context=None):
         db_leases = cls.dbapi.lease_get_all(filters)
         return cls._from_db_object_list(context, db_leases)
 
     def create(self, context=None):
         updates = self.obj_get_changes()
+        resource_type = updates['resource_type']
+        resource_uuid = updates['resource_uuid']
+        start_time = updates['start_time']
+        end_time = updates['end_time']
+        with utils.lock(utils.get_resource_lock_name(resource_type,
+                                                     resource_uuid),
+                        external=True):
+            self.verify_time_range(
+                start_time, end_time,
+                updates.get('offer_uuid', None),
+                updates.get('parent_lease_uuid', None),
+                resource_type, resource_uuid)
 
-        with utils.lock(utils.get_resource_lock_name(updates['resource_type'],
-                                                     updates['resource_uuid']),
+            db_lease = self.dbapi.lease_create(updates)
+            self._from_db_object(context, self, db_lease)
+
+    def update(self, updates, context=None):
+        # only allow updates to end_time right now
+        if 'end_time' not in updates:
+            return
+        new_end_time = updates['end_time']
+        with utils.lock(utils.get_resource_lock_name(self.resource_type,
+                                                     self.resource_uuid),
                         external=True):
-            if updates['start_time'] >= updates['end_time']:
+            if self.start_time >= new_end_time:
                 raise exception.InvalidTimeRange(
                     resource='lease',
-                    start_time=str(updates['start_time']),
-                    end_time=str(updates['end_time'])
+                    start_time=str(self.start_time),
+                    end_time=str(new_end_time)
                     )
 
-            # check availability
-            if 'offer_uuid' in updates:
-                # lease is being created from an offer
-                related_offer = offer_obj.Offer.get(updates['offer_uuid'])
-
-                if related_offer.status != statuses.AVAILABLE:
-                    raise exception.OfferNotAvailable(
-                        offer_uuid=related_offer.uuid,
-                        status=related_offer.status)
-
-                related_offer.verify_availability(updates['start_time'],
-                                                  updates['end_time'])
-            elif 'parent_lease_uuid' in updates:
-                # lease is a child of an existing lease
-                parent_lease = Lease.get(updates['parent_lease_uuid'])
-
-                if parent_lease.status != statuses.ACTIVE:
-                    raise exception.LeaseNotActive(
-                        updates['parent_lease_uuid'])
-
-                parent_lease.verify_child_availability(updates['start_time'],
-                                                       updates['end_time'])
-            else:
-                ro = get_resource_object(updates['resource_type'],
-                                         updates['resource_uuid'])
-                ro.verify_availability(updates['start_time'],
-                                       updates['end_time'])
+            # only need to check availabilities if new end time is greater
+            # than previous end time
+            if new_end_time > self.end_time:
+                self.verify_time_range(
+                    self.end_time, new_end_time,
+                    self.offer_uuid, self.parent_lease_uuid,
+                    self.resource_type, self.resource_uuid)
 
-            db_lease = self.dbapi.lease_create(updates)
-            self._from_db_object(context, self, db_lease)
+            # lease is available in new range; set and save
+            self.end_time = new_end_time
+            self.save(context)
 
     def cancel(self, context=None):
         leases = Lease.get_all(
             {'parent_lease_uuid': self.uuid,
              'status': statuses.LEASE_CAN_DELETE},
             None)
         for lease in leases:
@@ -331,7 +332,42 @@
                 if self.parent_lease_uuid is not None:
                     parent_lease = Lease.get(self.parent_lease_uuid)
                     resource.set_lease(parent_lease)
 
         notify.emit_end_notification(context, self,
                                      'delete', CRUD_NOTIFY_OBJ,
                                      node=resource)
+
+    @staticmethod
+    def verify_time_range(start_time, end_time,
+                          offer_uuid, parent_lease_uuid,
+                          resource_type, resource_uuid):
+        if start_time >= end_time:
+            raise exception.InvalidTimeRange(
+                resource='lease',
+                start_time=str(start_time),
+                end_time=str(end_time)
+            )
+
+        # check availability
+        if offer_uuid:
+            # lease is related to an offer
+            related_offer = offer_obj.Offer.get(offer_uuid)
+            if related_offer.status != statuses.AVAILABLE:
+                raise exception.OfferNotAvailable(
+                    offer_uuid=related_offer.uuid,
+                    status=related_offer.status)
+            related_offer.verify_availability(start_time,
+                                              end_time)
+        elif parent_lease_uuid:
+            # lease is a child of an existing lease
+            parent_lease = Lease.get(parent_lease_uuid)
+            if parent_lease.status != statuses.ACTIVE:
+                raise exception.LeaseNotActive(
+                    parent_lease_uuid)
+            parent_lease.verify_child_availability(start_time,
+                                                   end_time)
+        else:
+            ro = get_resource_object(resource_type,
+                                     resource_uuid)
+            ro.verify_availability(start_time, end_time)
+        return
```

### Comparing `esi-leap-0.2.9/esi_leap/objects/notification.py` & `esi-leap-0.3.0/esi_leap/objects/notification.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/objects/offer.py` & `esi-leap-0.3.0/esi_leap/objects/offer.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,17 @@
                           for j in range(0, len(times) - 1, 2)]
 
         else:
             avails = [[start_time, self.end_time]]
 
         return avails
 
-    def get_first_availability(self, start):
-        return self.dbapi.offer_get_first_availability(self.uuid, start)
+    def get_next_lease_start_time(self, start):
+        return self.dbapi.offer_get_next_lease_start_time(
+            self.uuid, start)
 
     def create(self, context=None):
         updates = self.obj_get_changes()
 
         with utils.lock(utils.get_resource_lock_name(updates['resource_type'],
                                                      updates['resource_uuid']),
                         external=True):
```

### Comparing `esi-leap-0.2.9/esi_leap/resource_objects/__init__.py` & `esi-leap-0.3.0/esi_leap/resource_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/resource_objects/base.py` & `esi-leap-0.3.0/esi_leap/resource_objects/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         """Return resource's name, if any"""
 
     @abc.abstractmethod
     def get_resource_class(self, resource_list):
         """Return resource's associated class, if any"""
 
     @abc.abstractmethod
-    def get_config(self):
-        """Return resource's associated config, if any"""
+    def get_properties(self, resource_list):
+        """Return resource's associated properties, if any"""
 
     @abc.abstractmethod
     def get_owner_project_id(self):
         """Return the project id of the resource's owner"""
 
     @abc.abstractmethod
     def get_lease_uuid(self):
```

### Comparing `esi-leap-0.2.9/esi_leap/resource_objects/dummy_node.py` & `esi-leap-0.3.0/esi_leap/resource_objects/dummy_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 
     def get_resource_class(self, resource_list=None):
         return self._get_node_attr('resource_class', '',
                                    resource_list=resource_list,
                                    err_msg='Error getting resource class',
                                    err_val=error.UNKNOWN['resource_class'])
 
-    def get_config(self):
-        return self._get_node_attr('server_config', {},
-                                   err_msg='Error getting resource config',
-                                   err_val=error.UNKNOWN['config'])
+    def get_properties(self, resource_list=None):
+        return self._get_node_attr('properties', {},
+                                   err_msg='Error getting resource properties',
+                                   err_val=error.UNKNOWN['properties'])
 
     def get_owner_project_id(self):
         return self._get_node_attr('project_owner_id', None,
                                    err_msg='Error getting owner project id',
                                    err_val=error.UNKNOWN['owner_project_id'])
 
     def get_lease_uuid(self):
```

### Comparing `esi-leap-0.2.9/esi_leap/resource_objects/error.py` & `esi-leap-0.3.0/esi_leap/resource_objects/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 UNKNOWN = {
     'uuid': 'unknown-uuid',
     'name': 'unknown-name',
     'resource_class': 'unknown-class',
-    'config': {},
+    'properties': {},
     'owner_project_id': 'unknown-owner',
     'lease_uuid': 'unknown-lease',
     'lessee_project_id': 'unknown-lessee',
     'provision_state': 'unknown-provision-state',
     'power_state': 'unknown-power-state'
 }
```

### Comparing `esi-leap-0.2.9/esi_leap/resource_objects/ironic_node.py` & `esi-leap-0.3.0/esi_leap/resource_objects/ironic_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,19 +57,22 @@
 
     def get_resource_class(self, resource_list=None):
         return self._get_node_attr('resource_class', '',
                                    resource_list=resource_list,
                                    err_msg='Error getting resource class',
                                    err_val=error.UNKNOWN['resource_class'])
 
-    def get_config(self):
-        config = self._get_node_attr('properties', {},
-                                     err_msg='Error getting resource config',
-                                     err_val=error.UNKNOWN['config'])
-        return config
+    def get_properties(self, resource_list=None):
+        properties = self._get_node_attr(
+            'properties', {}, resource_list=resource_list,
+            err_msg='Error getting resource properties',
+            err_val=error.UNKNOWN['properties'])
+        traits = self._get_node_attr(
+            'traits', [], resource_list=resource_list)
+        return ironic.get_condensed_properties(properties, traits)
 
     def get_owner_project_id(self):
         return self._get_node_attr('owner', '',
                                    err_msg='Error getting owner project id',
                                    err_val=error.UNKNOWN['owner_project_id'])
 
     def get_lease_uuid(self):
```

### Comparing `esi-leap-0.2.9/esi_leap/resource_objects/test_node.py` & `esi-leap-0.3.0/esi_leap/resource_objects/test_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def get_name(self, resource_list=None):
         return 'test-node-%s' % self._uuid
 
     def get_resource_class(self, resource_list=None):
         return 'fake'
 
-    def get_config(self):
+    def get_properties(self, resource_list=None):
         return {}
 
     def get_owner_project_id(self):
         return self._project_id
 
     def get_lease_uuid(self):
         return '12345'
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_event.py` & `esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_event.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_lease.py` & `esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_lease.py`

 * *Files 6% similar despite different names*

```diff
@@ -272,14 +272,80 @@
             resource,
             self.context.project_id,
             datetime.datetime(2016, 7, 17, 19, 20, 30),
             datetime.datetime(2016, 8, 14, 19, 20, 30))
         mock_create.assert_not_called()
         self.assertEqual(http_client.FORBIDDEN, request.status_int)
 
+    @mock.patch('esi_leap.api.controllers.v1.utils.'
+                'lease_get_dict_with_added_info')
+    @mock.patch('esi_leap.objects.lease.Lease.update')
+    @mock.patch('esi_leap.api.controllers.v1.utils.'
+                'check_lease_policy_and_retrieve')
+    def test_patch(self, mock_clpar, mock_lease_update, mock_lgdwai):
+        mock_clpar.return_value = self.test_lease
+
+        data = {
+            'end_time': '2016-09-16T19:20:30'
+        }
+        request = self.patch_json(
+            "/leases/%s" % self.test_lease.uuid, data)
+
+        mock_clpar.assert_called_once_with(self.context,
+                                           'esi_leap:lease:update',
+                                           self.test_lease.uuid)
+        mock_lease_update.assert_called_once()
+        mock_lgdwai.assert_called_once()
+        self.assertEqual(http_client.OK, request.status_int)
+
+    @mock.patch('esi_leap.api.controllers.v1.utils.'
+                'lease_get_dict_with_added_info')
+    @mock.patch('esi_leap.objects.lease.Lease.update')
+    @mock.patch('esi_leap.api.controllers.v1.utils.'
+                'check_lease_policy_and_retrieve')
+    def test_patch_no_end_time(self, mock_clpar, mock_lease_update,
+                               mock_lgdwai):
+        mock_clpar.return_value = self.test_lease
+
+        data = {
+            'name': 'foo'
+        }
+        request = self.patch_json(
+            "/leases/%s" % self.test_lease.uuid, data, expect_errors=True)
+
+        mock_clpar.assert_called_once_with(self.context,
+                                           'esi_leap:lease:update',
+                                           self.test_lease.uuid)
+        mock_lease_update.assert_not_called()
+        mock_lgdwai.assert_not_called()
+        self.assertEqual(http_client.INTERNAL_SERVER_ERROR, request.status_int)
+
+    @mock.patch('esi_leap.api.controllers.v1.utils.'
+                'lease_get_dict_with_added_info')
+    @mock.patch('esi_leap.objects.lease.Lease.update')
+    @mock.patch('esi_leap.api.controllers.v1.utils.'
+                'check_lease_policy_and_retrieve')
+    def test_patch_end_time_and_more(self, mock_clpar, mock_lease_update,
+                                     mock_lgdwai):
+        mock_clpar.return_value = self.test_lease
+
+        data = {
+            'end_time': '2016-09-16T19:20:30',
+            'name': 'foo'
+        }
+        request = self.patch_json(
+            "/leases/%s" % self.test_lease.uuid, data, expect_errors=True)
+
+        mock_clpar.assert_called_once_with(self.context,
+                                           'esi_leap:lease:update',
+                                           self.test_lease.uuid)
+        mock_lease_update.assert_not_called()
+        mock_lgdwai.assert_not_called()
+        self.assertEqual(http_client.INTERNAL_SERVER_ERROR, request.status_int)
+
     @mock.patch('esi_leap.common.ironic.get_node_list')
     @mock.patch('esi_leap.common.keystone.get_project_list')
     @mock.patch('esi_leap.api.controllers.v1.utils.'
                 'lease_get_dict_with_added_info')
     @mock.patch('esi_leap.api.controllers.v1.lease.LeasesController.'
                 '_lease_get_all_authorize_filters')
     @mock.patch('esi_leap.objects.lease.Lease.get_all')
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_node.py` & `esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_node.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 
 
 class FakeIronicNode(object):
     def __init__(self):
         self.name = 'fake-node'
         self.owner = 'fake-project-uuid'
         self.uuid = 'fake-uuid'
-        self.properties = {'lease_uuid': 'fake-lease-uuid'}
+        self.properties = {'lease_uuid': 'fake-lease-uuid', 'cpu': '40'}
+        self.traits = ['trait1', 'trait2']
         self.lessee = 'fake-project-uuid'
         self.maintenance = False
         self.provision_state = 'active'
+        self.resource_class = 'baremetal'
 
 
 class FakeProject(object):
     def __init__(self):
         self.name = 'fake-project'
         self.id = 'fake-project-uuid'
 
@@ -57,7 +59,9 @@
         mock_gpl.assert_called_once()
 
         self.assertEqual(data['nodes'][0]['name'], 'fake-node')
         self.assertEqual(data['nodes'][0]['uuid'], 'fake-uuid')
         self.assertEqual(data['nodes'][0]['owner'], 'fake-project')
         self.assertEqual(data['nodes'][0]['lease_uuid'], 'fake-lease-uuid')
         self.assertEqual(data['nodes'][0]['lessee'], 'fake-project')
+        self.assertEqual(data['nodes'][0]['properties'], {
+            'cpu': '40', 'traits': ['trait1', 'trait2']})
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_offer.py` & `esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_offer.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/api/controllers/v1/test_utils.py` & `esi-leap-0.3.0/esi_leap/tests/api/controllers/v1/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -638,14 +638,15 @@
 
         o_dict = utils.offer_get_dict_with_added_info(o)
 
         expected_offer_dict = {
             'resource_type': o.resource_type,
             'resource_uuid': o.resource_uuid,
             'resource_class': 'fake',
+            'resource_properties': {},
             'resource': 'test-node-1234567890',
             'name': o.name,
             'project_id': o.project_id,
             'project': 'project-name',
             'lessee_id': None,
             'lessee': 'project-name',
             'start_time': o.start_time,
@@ -685,12 +686,58 @@
         output_dict = utils.lease_get_dict_with_added_info(self.test_lease)
 
         expected_output_dict = self.test_lease.to_dict()
         expected_output_dict['resource'] = 'resource-name'
         expected_output_dict['project'] = 'project-name'
         expected_output_dict['owner'] = 'project-name'
         expected_output_dict['resource_class'] = 'fake'
+        expected_output_dict['resource_properties'] = {}
 
         mock_gro.assert_called_once()
         self.assertEqual(2, mock_gpn.call_count)
         mock_gn.assert_called_once()
         self.assertEqual(expected_output_dict, output_dict)
+
+
+class TestCheckLeaseLength(testtools.TestCase):
+    def setUp(self):
+        super(TestCheckLeaseLength, self).setUp()
+        self.max_time = 21
+        self.start_time = datetime.datetime(2016, 7, 16, 19, 20, 30)
+        self.end_time = datetime.datetime(2016, 8, 16, 19, 20, 30)
+        self.end_time_1 = datetime.datetime(2016, 7, 20, 19, 20, 30)
+
+    @mock.patch('esi_leap.api.controllers.v1.utils.policy_authorize')
+    def test_check_lease_length_admin_exceed_max(self, mock_authorize):
+        utils.check_lease_length(admin_ctx.to_policy_values(),
+                                 self.start_time,
+                                 self.end_time,
+                                 self.max_time)
+
+        mock_authorize.assert_called_once_with('esi_leap:lease:lease_admin',
+                                               admin_ctx.to_policy_values(),
+                                               admin_ctx.to_policy_values())
+
+    @mock.patch('esi_leap.api.controllers.v1.utils.policy_authorize')
+    def test_check_lease_length_exception(self, mock_authorize):
+        mock_authorize.side_effect = exception.HTTPForbidden(
+            'esi_leap:lease:lease_admin')
+
+        self.assertRaises(exception.LeaseExceedMaxTimeRange,
+                          utils.check_lease_length,
+                          lessee_ctx.to_policy_values(),
+                          self.start_time,
+                          self.end_time,
+                          self.max_time)
+
+        mock_authorize.assert_called_once_with('esi_leap:lease:lease_admin',
+                                               lessee_ctx.to_policy_values(),
+                                               lessee_ctx.to_policy_values())
+
+    @mock.patch('esi_leap.api.controllers.v1.utils.policy_authorize')
+    def test_check_lease_length_non_admin_valid(self, mock_authorize):
+        utils.check_lease_length(lessee_ctx.to_policy_values(),
+                                 self.start_time,
+                                 self.end_time_1,
+                                 self.max_time)
+
+        assert not mock_authorize.called
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/api/controllers/test_types.py` & `esi-leap-0.3.0/esi_leap/tests/api/controllers/test_types.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/api/base.py` & `esi-leap-0.3.0/esi_leap/tests/api/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -95,14 +95,33 @@
         """
         return self._request_json(path=path, params=params,
                                   expect_errors=expect_errors,
                                   headers=headers, extra_environ=extra_environ,
                                   status=status, method='post')
 
     # borrowed from Ironic
+    def patch_json(self, path, params, expect_errors=False, headers=None,
+                   extra_environ=None, status=None):
+        """Sends simulated HTTP PATCH request to Pecan test app.
+
+        :param path: url path of target service
+        :param params: content for wsgi.input of request
+        :param expect_errors: Boolean value; whether an error is expected based
+                              on request
+        :param headers: a dictionary of headers to send along with the request
+        :param extra_environ: a dictionary of environ variables to send along
+                              with the request
+        :param status: expected status code of response
+        """
+        return self._request_json(path=path, params=params,
+                                  expect_errors=expect_errors,
+                                  headers=headers, extra_environ=extra_environ,
+                                  status=status, method='patch')
+
+    # borrowed from Ironic
     def delete_json(self, path, expect_errors=False, headers=None,
                     extra_environ=None, status=None):
         """Sends simulated HTTP POST request to Pecan test app.
 
         :param path: url path of target service
         :param expect_errors: Boolean value; whether an error is expected based
                               on request
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/common/test_ironic.py` & `esi-leap-0.3.0/esi_leap/tests/common/test_ironic.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,7 +44,24 @@
     @mock.patch.object(ironic, 'get_ironic_client', autospec=True)
     def test_get_node_list_no_match(self, mock_ironic):
         fake_node = FakeNode()
         node_list = [fake_node]
         node = ironic.get_node('uuid2', node_list)
 
         self.assertEqual(None, node)
+
+    def test_get_condensed_properties(self):
+        properties = {
+            'lease_uuid': '12345',
+            'capabilities': 'magic',
+            'cpu': '40',
+            'local_gb': '1000'
+        }
+        traits = ['trait1', 'trait2']
+        cp = ironic.get_condensed_properties(
+            properties, traits)
+
+        self.assertEqual(cp, {
+            'cpu': '40',
+            'local_gb': '1000',
+            'traits': ['trait1', 'trait2']
+        })
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/common/test_keystone.py` & `esi-leap-0.3.0/esi_leap/tests/common/test_keystone.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/common/test_notification_utils.py` & `esi-leap-0.3.0/esi_leap/tests/common/test_notification_utils.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/common/test_policy.py` & `esi-leap-0.3.0/esi_leap/tests/common/test_policy.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/common/test_rpc.py` & `esi-leap-0.3.0/esi_leap/tests/common/test_rpc.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/common/test_utils.py` & `esi-leap-0.3.0/esi_leap/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/db/sqlalchemy/test_api.py` & `esi-leap-0.3.0/esi_leap/tests/db/sqlalchemy/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,28 @@
     start_time=now + datetime.timedelta(days=5),
     end_time=now + datetime.timedelta(days=30),
     uuid='6666',
     properties={},
     status=statuses.EXPIRED,
 )
 
+test_lease_7 = dict(
+    uuid='77777',
+    project_id='1e5533_2',
+    owner_id='0wn3r_2',
+    name='l1',
+    resource_uuid='1111',
+    resource_type='dummy_node',
+    purpose='test_purpose',
+    start_time=now - datetime.timedelta(days=10),
+    end_time=now + datetime.timedelta(days=10),
+    properties={},
+    status=statuses.ACTIVE,
+)
+
 test_event_1 = dict(
     id=1,
     event_type='fake:event:start',
     event_time=now - datetime.timedelta(days=20),
     object_type='lease',
     object_uuid='11111',
     resource_type='dummy_node',
@@ -336,23 +350,26 @@
         api.lease_create(test_lease_3)
         api.lease_create(test_lease_4)
         api.lease_create(test_lease_5)
         self.assertEqual(api.offer_get_conflict_times(o1),
                          [(now + datetime.timedelta(days=50),
                           now + datetime.timedelta(days=60))])
 
-    def test_offer_get_first_availability(self):
+    def test_offer_get_next_lease_start_time(self):
         o1 = api.offer_create(test_offer_1)
-        self.assertEqual(api.offer_get_first_availability
+        self.assertEqual(api.offer_get_next_lease_start_time
                          (o1.uuid, o1.start_time,), None)
         test_lease_3['offer_uuid'] = o1.uuid
         api.lease_create(test_lease_3)
-        self.assertEqual(api.offer_get_first_availability(o1.uuid,
-                                                          o1.start_time),
-                         (now + datetime.timedelta(days=50),))
+        test_lease_7['offer_uuid'] = o1.uuid
+        api.lease_create(test_lease_7)
+        self.assertEqual(
+            api.offer_get_next_lease_start_time(
+                o1.uuid, o1.start_time),
+            (now + datetime.timedelta(days=50),))
 
     def test_offer_get_by_uuid(self):
         o1 = api.offer_create(test_offer_1)
         res = api.offer_get_by_uuid(o1.uuid)
         self.assertEqual(o1.uuid, res.uuid)
         self.assertEqual(o1.project_id, res.project_id)
         self.assertEqual(o1.properties, res.properties)
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/manager/test_service.py` & `esi-leap-0.3.0/esi_leap/tests/manager/test_service.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/objects/test_event.py` & `esi-leap-0.3.0/esi_leap/tests/objects/test_event.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/objects/test_fields.py` & `esi-leap-0.3.0/esi_leap/tests/objects/test_fields.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/objects/test_lease.py` & `esi-leap-0.3.0/esi_leap/tests/objects/test_lease.py`

 * *Files 12% similar despite different names*

```diff
@@ -115,139 +115,132 @@
             leases = lease_obj.Lease.get_all({}, self.context)
 
             mock_lease_get_all.assert_called_once_with({})
             self.assertEqual(len(leases), 2)
             self.assertIsInstance(leases[0], lease_obj.Lease)
             self.assertEqual(self.context, leases[0]._context)
 
-    @mock.patch('esi_leap.db.sqlalchemy.api.resource_verify_availability')
-    @mock.patch('esi_leap.db.sqlalchemy.api.offer_verify_availability')
-    @mock.patch('esi_leap.objects.offer.Offer.get')
+    @mock.patch('esi_leap.objects.lease.Lease.verify_time_range')
     @mock.patch('esi_leap.db.sqlalchemy.api.lease_create')
-    def test_create(self, mock_lc, mock_og, mock_ova, mock_rva):
+    def test_create(self, mock_lc, mock_vtr):
         lease = lease_obj.Lease(self.context, **self.test_lease_create_dict)
         mock_lc.return_value = self.test_lease_dict
 
         lease.create()
 
         mock_lc.assert_called_once_with(self.test_lease_create_dict)
-        mock_og.assert_not_called
-        mock_ova.assert_not_called
-        mock_rva.assert_called_once_with(lease.resource_type,
-                                         lease.resource_uuid,
-                                         lease.start_time,
-                                         lease.end_time)
+        mock_vtr.assert_called_once_with(
+            lease.start_time, lease.end_time,
+            None, None,
+            lease.resource_type, lease.resource_uuid)
 
-    @mock.patch('esi_leap.db.sqlalchemy.api.resource_verify_availability')
-    @mock.patch('esi_leap.db.sqlalchemy.api.offer_verify_availability')
-    @mock.patch('esi_leap.objects.offer.Offer.get')
-    @mock.patch('esi_leap.db.sqlalchemy.api.lease_create')
-    def test_create_with_offer(self, mock_lc, mock_og, mock_ova, mock_rva):
+    def test_create_conflict(self):
         lease = lease_obj.Lease(self.context,
                                 **self.test_lease_create_offer_dict)
-        mock_lc.return_value = self.test_lease_offer_dict
-        mock_og.return_value = self.test_offer
+        lease2 = lease_obj.Lease(self.context,
+                                 **self.test_lease_create_offer_dict)
+        lease2.id = 28
 
-        lease.create()
+        with mock.patch.object(self.db_api, 'lease_create',
+                               autospec=True) as mock_lease_create:
+            with mock.patch.object(lease_obj.Lease, 'verify_time_range',
+                                   autospec=True) as mock_vtr:
+                def update_mock(context):
+                    mock_vtr.side_effect = Exception('bad')
 
-        mock_lc.assert_called_once_with(self.test_lease_create_offer_dict)
-        mock_og.assert_called_once_with(lease.offer_uuid)
-        mock_ova.assert_called_once_with(self.test_offer,
-                                         lease.start_time,
-                                         lease.end_time)
-        mock_rva.assert_not_called
+                mock_lease_create.side_effect = update_mock
 
-    @mock.patch('esi_leap.db.sqlalchemy.api.lease_verify_child_availability')
-    @mock.patch('esi_leap.objects.lease.Lease.get')
-    @mock.patch('esi_leap.db.sqlalchemy.api.lease_create')
-    def test_create_with_parent_lease(self, mock_lc, mock_lg, mock_lvca):
-        lease = lease_obj.Lease(self.context,
-                                **self.test_lease_create_parent_lease_dict)
-        mock_lc.return_value = self.test_lease_offer_dict
-        mock_lg.return_value = self.test_parent_lease
+                thread = threading.Thread(target=lease.create)
+                thread2 = threading.Thread(target=lease2.create)
 
-        lease.create()
+                thread.start()
+                thread2.start()
 
-        mock_lc.assert_called_once_with(
-            self.test_lease_create_parent_lease_dict)
-        mock_lg.assert_called_once_with('parent-lease-uuid')
-        mock_lvca.assert_called_once_with(self.test_parent_lease,
-                                          lease.start_time,
-                                          lease.end_time)
+                thread.join()
+                thread2.join()
 
-    @mock.patch('esi_leap.db.sqlalchemy.api.lease_verify_child_availability')
-    @mock.patch('esi_leap.objects.lease.Lease.get')
-    @mock.patch('esi_leap.db.sqlalchemy.api.lease_create')
-    def test_create_with_parent_lease_expired(self, mock_lc, mock_lg,
-                                              mock_lvca):
-        lease = lease_obj.Lease(self.context,
-                                **self.test_lease_create_parent_lease_dict)
-        mock_lg.return_value = self.test_parent_lease_expired
+                assert mock_vtr.call_count == 2
+                mock_lease_create.assert_called_once()
 
-        self.assertRaises(exception.LeaseNotActive, lease.create)
+    @mock.patch('esi_leap.objects.lease.Lease.save')
+    @mock.patch('esi_leap.objects.lease.Lease.verify_time_range')
+    def test_update(self, mock_vtr, mock_save):
+        lease = lease_obj.Lease(self.context, **self.test_lease_dict)
+        end_time = lease.end_time
+        new_end_time = end_time + datetime.timedelta(days=10)
+        updates = {
+            'end_time': new_end_time
+        }
+        lease.update(updates)
 
-        mock_lc.assert_not_called()
-        mock_lg.assert_called_once_with('parent-lease-uuid')
-        mock_lvca.assert_not_called()
+        mock_vtr.assert_called_once_with(
+            end_time, new_end_time,
+            lease.offer_uuid, lease.parent_lease_uuid,
+            lease.resource_type, lease.resource_uuid)
+        mock_save.assert_called_once
 
-    def test_create_invalid_time(self):
-        bad_lease = {
-            'id': 30,
-            'name': 'bad-lease',
-            'uuid': '534653c9-880d-4c2d-6d6d-44444444444',
-            'project_id': 'le55ee_2',
-            'owner_id': 'ownerid',
-            'resource_type': 'dummy_node',
-            'resource_uuid': '1111',
-            'start_time': self.start_time + datetime.timedelta(days=30),
-            'end_time': self.start_time + datetime.timedelta(days=20),
-            'fulfill_time': self.start_time + datetime.timedelta(days=35),
-            'expire_time': self.start_time + datetime.timedelta(days=40),
+    @mock.patch('esi_leap.objects.lease.Lease.save')
+    @mock.patch('esi_leap.objects.lease.Lease.verify_time_range')
+    def test_update_no_end_time(self, mock_vtr, mock_save):
+        lease = lease_obj.Lease(self.context, **self.test_lease_dict)
+        updates = {
+            'name': 'foo'
         }
+        lease.update(updates)
 
-        lease = lease_obj.Lease(self.context, **bad_lease)
+        mock_vtr.assert_not_called
+        mock_save.assert_not_called
 
-        self.assertRaises(exception.InvalidTimeRange, lease.create)
+    @mock.patch('esi_leap.objects.lease.Lease.save')
+    @mock.patch('esi_leap.objects.lease.Lease.verify_time_range')
+    def test_update_invalid_end_time(self, mock_vtr, mock_save):
+        lease = lease_obj.Lease(self.context, **self.test_lease_dict)
+        end_time = lease.end_time
+        new_end_time = end_time - datetime.timedelta(days=10)
+        updates = {
+            'end_time': new_end_time
+        }
 
-    def test_create_concurrent_offer_conflict(self):
-        lease = lease_obj.Lease(self.context,
-                                **self.test_lease_create_offer_dict)
+        self.assertRaises(exception.InvalidTimeRange,
+                          lease.update, updates)
+        mock_vtr.assert_not_called
+        mock_save.assert_not_called
 
+    def test_update_conflict(self):
+        lease = lease_obj.Lease(self.context,
+                                **self.test_lease_dict)
         lease2 = lease_obj.Lease(self.context,
-                                 **self.test_lease_create_offer_dict)
-
+                                 **self.test_lease_dict)
         lease2.id = 28
+        lease_updates = {
+            'end_time': lease.end_time + datetime.timedelta(days=10)
+        }
 
-        with mock.patch.object(self.db_api, 'lease_create',
-                               autospec=True) as mock_lease_create:
-            with mock.patch.object(offer_obj.Offer, 'get',
-                                   autospec=True) as mock_offer_get:
-                with mock.patch.object(self.db_api,
-                                       'offer_verify_availability',
-                                       autospec=True) as mock_ovca:
-
-                    mock_offer_get.return_value = self.test_offer
-
-                    def update_mock(updates):
-                        mock_ovca.side_effect = Exception('bad')
-
-                    mock_lease_create.side_effect = update_mock
-
-                    thread = threading.Thread(target=lease.create)
-                    thread2 = threading.Thread(target=lease2.create)
+        with mock.patch.object(lease_obj.Lease, 'save',
+                               autospec=True) as mock_save:
+            with mock.patch.object(lease_obj.Lease, 'verify_time_range',
+                                   autospec=True) as mock_vtr:
+                def update_mock(updates, context):
+                    mock_vtr.side_effect = Exception('bad')
+
+                mock_save.side_effect = update_mock
+
+                thread = threading.Thread(
+                    target=lease.update, args=[lease_updates])
+                thread2 = threading.Thread(
+                    target=lease2.update, args=[lease_updates])
 
-                    thread.start()
-                    thread2.start()
+                thread.start()
+                thread2.start()
 
-                    thread.join()
-                    thread2.join()
+                thread.join()
+                thread2.join()
 
-                    assert mock_offer_get.call_count == 2
-                    assert mock_ovca.call_count == 2
-                    mock_lease_create.assert_called_once()
+                assert mock_vtr.call_count == 2
+                mock_save.assert_called_once()
 
     @mock.patch('esi_leap.objects.lease.Lease.resource_object')
     @mock.patch('esi_leap.resource_objects.test_node.TestNode.set_lease')
     @mock.patch('esi_leap.objects.lease.Lease.save')
     @mock.patch('esi_leap.common.notification_utils'
                 '._emit_notification')
     def test_fulfill(self, mock_notify,
@@ -602,14 +595,103 @@
     @mock.patch('esi_leap.objects.lease.get_resource_object')
     def test_resource_object(self, mock_gro):
         lease = lease_obj.Lease(self.context, **self.test_lease_dict)
         lease.resource_object()
         mock_gro.assert_called_once_with(lease.resource_type,
                                          lease.resource_uuid)
 
+    @mock.patch('esi_leap.db.sqlalchemy.api.resource_verify_availability')
+    @mock.patch('esi_leap.db.sqlalchemy.api.offer_verify_availability')
+    @mock.patch('esi_leap.objects.offer.Offer.get')
+    def test_verify_time_range(self, mock_og, mock_ova, mock_rva):
+        lease = lease_obj.Lease(self.context, **self.test_lease_create_dict)
+        lease.verify_time_range(lease.start_time, lease.end_time,
+                                None, None,
+                                lease.resource_type, lease.resource_uuid)
+
+        mock_og.assert_not_called
+        mock_ova.assert_not_called
+        mock_rva.assert_called_once_with(lease.resource_type,
+                                         lease.resource_uuid,
+                                         lease.start_time,
+                                         lease.end_time)
+
+    @mock.patch('esi_leap.db.sqlalchemy.api.resource_verify_availability')
+    @mock.patch('esi_leap.db.sqlalchemy.api.offer_verify_availability')
+    @mock.patch('esi_leap.objects.offer.Offer.get')
+    def test_verify_time_range_with_offer(self, mock_og, mock_ova, mock_rva):
+        lease = lease_obj.Lease(self.context,
+                                **self.test_lease_create_offer_dict)
+        mock_og.return_value = self.test_offer
+        lease.verify_time_range(lease.start_time, lease.end_time,
+                                lease.offer_uuid, None,
+                                lease.resource_type, lease.resource_uuid)
+
+        mock_og.assert_called_once_with(lease.offer_uuid)
+        mock_ova.assert_called_once_with(self.test_offer,
+                                         lease.start_time,
+                                         lease.end_time)
+        mock_rva.assert_not_called
+
+    @mock.patch('esi_leap.db.sqlalchemy.api.lease_verify_child_availability')
+    @mock.patch('esi_leap.objects.lease.Lease.get')
+    def test_verify_time_range_with_parent_lease(self, mock_lg, mock_lvca):
+        lease = lease_obj.Lease(self.context,
+                                **self.test_lease_create_parent_lease_dict)
+        mock_lg.return_value = self.test_parent_lease
+        lease.verify_time_range(lease.start_time, lease.end_time,
+                                None, lease.parent_lease_uuid,
+                                lease.resource_type, lease.resource_uuid)
+
+        mock_lg.assert_called_once_with('parent-lease-uuid')
+        mock_lvca.assert_called_once_with(self.test_parent_lease,
+                                          lease.start_time,
+                                          lease.end_time)
+
+    @mock.patch('esi_leap.db.sqlalchemy.api.lease_verify_child_availability')
+    @mock.patch('esi_leap.objects.lease.Lease.get')
+    def test_verify_time_range_with_parent_lease_expired(
+            self, mock_lg, mock_lvca):
+        lease = lease_obj.Lease(self.context,
+                                **self.test_lease_create_parent_lease_dict)
+        mock_lg.return_value = self.test_parent_lease_expired
+
+        self.assertRaises(exception.LeaseNotActive,
+                          lease.verify_time_range,
+                          lease.start_time, lease.end_time,
+                          None, lease.parent_lease_uuid,
+                          lease.resource_type, lease.resource_uuid)
+
+        mock_lg.assert_called_once_with('parent-lease-uuid')
+        mock_lvca.assert_not_called()
+
+    def test_verify_time_range_invalid_time(self):
+        bad_lease = {
+            'id': 30,
+            'name': 'bad-lease',
+            'uuid': '534653c9-880d-4c2d-6d6d-44444444444',
+            'project_id': 'le55ee_2',
+            'owner_id': 'ownerid',
+            'resource_type': 'dummy_node',
+            'resource_uuid': '1111',
+            'start_time': self.start_time + datetime.timedelta(days=30),
+            'end_time': self.start_time + datetime.timedelta(days=20),
+            'fulfill_time': self.start_time + datetime.timedelta(days=35),
+            'expire_time': self.start_time + datetime.timedelta(days=40),
+        }
+
+        lease = lease_obj.Lease(self.context, **bad_lease)
+
+        self.assertRaises(exception.InvalidTimeRange,
+                          lease.verify_time_range,
+                          bad_lease['start_time'], bad_lease['end_time'],
+                          None, None,
+                          bad_lease['resource_type'],
+                          bad_lease['resource_uuid'])
+
 
 class TestLeaseCRUDPayloads(base.DBTestCase):
 
     def setUp(self):
         super(TestLeaseCRUDPayloads, self).setUp()
         self.lease = lease_obj.Lease(
             id='12345',
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/objects/test_notification.py` & `esi-leap-0.3.0/esi_leap/tests/objects/test_notification.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/objects/test_offer.py` & `esi-leap-0.3.0/esi_leap/tests/objects/test_offer.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/resource_objects/test_base.py` & `esi-leap-0.3.0/esi_leap/tests/resource_objects/test_base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/resource_objects/test_dummy_node.py` & `esi-leap-0.3.0/esi_leap/tests/resource_objects/test_dummy_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,28 +38,28 @@
     test_node_1 = {
         'project_owner_id': '123456',
         'project_id': '654321',
         'lease_uuid': '001',
         'resource_class': 'fake',
         'power_state': 'off',
         'provision_state': 'enroll',
-        'server_config': {
+        'properties': {
             'new attribute XYZ': 'new attribute XYZ',
             'cpu_type': 'Intel Xeon',
             'cores': 16,
             'ram_gb': 512,
             'storage_type': 'samsung SSD',
             'storage_size_gb': 204
         }
     }
 
     test_node_2 = {
         'project_owner_id': '123456',
         'resource_class': 'fake',
-        'server_config': {
+        'properties': {
             'new attribute XYZ': 'new attribute XYZ',
             'cpu_type': 'Intel Xeon',
             'cores': 16,
             'ram_gb': 512,
             'storage_type': 'samsung SSD',
             'storage_size_gb': 204
         }
@@ -85,19 +85,19 @@
         mock_open = mock.mock_open(read_data=self.fake_read_data_1)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
             resource_class = self.fake_dummy_node.get_resource_class()
             self.assertEqual(resource_class,
                              self.test_node_1['resource_class'])
             mock_file_open.assert_called_once()
 
-    def test_get_config(self):
+    def test_get_properties(self):
         mock_open = mock.mock_open(read_data=self.fake_read_data_1)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
-            config = self.fake_dummy_node.get_config()
-            self.assertEqual(config, self.test_node_1['server_config'])
+            properties = self.fake_dummy_node.get_properties()
+            self.assertEqual(properties, self.test_node_1['properties'])
             mock_file_open.assert_called_once()
 
     def test_get_owner_project_id(self):
         mock_open = mock.mock_open(read_data=self.fake_read_data_1)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
             self.assertEqual(self.fake_dummy_node.get_owner_project_id(),
                              self.test_node_1['project_owner_id'])
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/resource_objects/test_ironic_node.py` & `esi-leap-0.3.0/esi_leap/tests/resource_objects/test_ironic_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 
 class FakeIronicNode(object):
     def __init__(self):
         self.created_at = start
         self.lessee = 'abcdef'
         self.owner = '123456'
         self.name = 'fake-node'
-        self.properties = {'lease_uuid': '001'}
+        self.properties = {'lease_uuid': '001', 'cpu': '40'}
         self.provision_state = 'available'
+        self.traits = ['trait1', 'trait2']
         self.uuid = fake_uuid
         self.resource_class = 'baremetal'
         self.power_state = 'off'
 
 
 class FakeLease(object):
     def __init__(self):
@@ -83,23 +84,26 @@
         mock_gn.return_value = fake_get_node
 
         resource_class = test_ironic_node.get_resource_class()
         self.assertEqual('baremetal', resource_class)
         mock_gn.assert_called_once()
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
-    def test_get_config(self, mock_gn):
+    def test_get_properties(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
 
-        config = test_ironic_node.get_config()
-        expected_config = fake_get_node.properties
-        self.assertEqual(config, expected_config)
-        mock_gn.assert_called_once()
+        properties = test_ironic_node.get_properties()
+        expected_properties = {
+            'cpu': '40',
+            'traits': ['trait1', 'trait2']
+        }
+        self.assertEqual(properties, expected_properties)
+        assert mock_gn.call_count == 2
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
     def test_get_owner_project_id(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/resource_objects/test_resource_objects.py` & `esi-leap-0.3.0/esi_leap/tests/resource_objects/test_resource_objects.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/tests/resource_objects/test_test_node.py` & `esi-leap-0.3.0/esi_leap/tests/resource_objects/test_test_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 
     def test_get_name(self):
         self.assertEqual(self.fake_test_node.get_name(), 'test-node-1111')
 
     def test_get_resource_class(self):
         self.assertEqual(self.fake_test_node.get_resource_class(), 'fake')
 
-    def test_get_config(self):
-        self.assertEqual(self.fake_test_node.get_config(), {})
+    def test_get_properties(self):
+        self.assertEqual(self.fake_test_node.get_properties(), {})
 
     def test_get_owner_project_id(self):
         self.assertEqual(self.fake_test_node.get_owner_project_id(), '123456')
 
     def test_get_lease_uuid(self):
         self.assertEqual(self.fake_test_node.get_lease_uuid(), '12345')
```

### Comparing `esi-leap-0.2.9/esi_leap/tests/base.py` & `esi-leap-0.3.0/esi_leap/tests/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap/version.py` & `esi-leap-0.3.0/esi_leap/version.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/esi_leap.egg-info/PKG-INFO` & `esi-leap-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: esi-leap
-Version: 0.2.9
-Summary: ESI provider
-Home-page: UNKNOWN
-Author: ESI
-Author-email: esi@lists.massopen.cloud
-License: Apache License, Version 2.0
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Environment :: OpenStack
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
 # esi-leap
 
 esi-leap is an OpenStack service for leasing baremetal nodes, designed to run
 on top of [multi-tenant
 Ironic](https://docs.openstack.org/ironic/latest/admin/node-multitenancy.html).
 It consists of an API that provides endpoints for leasing operations and a
 manager service that updates the status of leases and offers as required. See
@@ -201,25 +173,22 @@
 If you wish to use dummy nodes instead of Ironic nodes, simply specify the `dummy_node_dir`
 as specified above. Once you do so, add dummy nodes as follows:
 
 ```
 cat <<EOF > /tmp/nodes/1718
 {
     "project_owner_id": "project id of dummy node owner",
-    "server_config": {
+    "properties": {
         "new attribute XYZ": "This is just a sample list of free-form attributes used for describing a server.",
         "cpu_type": "Intel Xeon",
         "cores": 16,
         "ram_gb": 512,
         "storage_type": "samsung SSD",
         "storage_size_gb": 204
     }
 }
 EOF
 ```
 
 `1718` is the dummy node UUID; replace it with whatever you'd like. When creating an offer
 for this dummy node, simply specify `resource_type` as `dummy_node` and `resource_uuid` as
 `1718`.
-
-
-
```

### Comparing `esi-leap-0.2.9/esi_leap.egg-info/SOURCES.txt` & `esi-leap-0.3.0/esi_leap.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 tox.ini
 .github/workflows/tests.yml
 docs/esi-leap-api-ref.md
 docs/esi-leap-policy.md
 docs/esi-leap-reporting.md
 docs/esi-leap-requirements.md
 esi_leap/__init__.py
+esi_leap/send_email_notification.py
 esi_leap/version.py
 esi_leap.egg-info/PKG-INFO
 esi_leap.egg-info/SOURCES.txt
 esi_leap.egg-info/dependency_links.txt
 esi_leap.egg-info/entry_points.txt
 esi_leap.egg-info/not-zip-safe
 esi_leap.egg-info/pbr.json
@@ -94,14 +95,16 @@
 esi_leap/objects/offer.py
 esi_leap/resource_objects/__init__.py
 esi_leap/resource_objects/base.py
 esi_leap/resource_objects/dummy_node.py
 esi_leap/resource_objects/error.py
 esi_leap/resource_objects/ironic_node.py
 esi_leap/resource_objects/test_node.py
+esi_leap/templates/lease_create_email.txt
+esi_leap/templates/lease_expire_email.txt
 esi_leap/tests/__init__.py
 esi_leap/tests/base.py
 esi_leap/tests/api/__init__.py
 esi_leap/tests/api/base.py
 esi_leap/tests/api/controllers/__init__.py
 esi_leap/tests/api/controllers/test_types.py
 esi_leap/tests/api/controllers/v1/__init__.py
```

### Comparing `esi-leap-0.2.9/esi_leap.egg-info/requires.txt` & `esi-leap-0.3.0/esi_leap.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 pbr!=2.1.0,>=2.0.0
 alembic>=1.4.2
 Babel!=2.4.0,>=2.3.4
 eventlet>=0.33.3
-importlib-metadata<5.0.0
 iso8601>=0.1.11
 keystoneauth1>=3.4.0
 keystonemiddleware>=4.17.0
 kombu!=4.0.2,>=4.0.0
 openstacksdk<1.3.0
 oslo.concurrency>=3.26.0
 oslo.config>=5.2.0
@@ -30,7 +29,10 @@
 requests>=2.18.4
 Routes>=2.3.1
 six>=1.10.0
 SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,<2.0,>=1.0.10
 stevedore>=1.20.0
 WebOb>=1.7.1
 WSME>=0.8.0
+
+[:(python_version<'3.8')]
+importlib-metadata<5.0.0
```

### Comparing `esi-leap-0.2.9/AUTHORS` & `esi-leap-0.3.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/ChangeLog` & `esi-leap-0.3.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 CHANGES
 =======
 
+0.3.0
+-----
+
+* Allow leases to update end\_time
+
+0.2.12
+------
+
+* Push up node resource\_class/properties/traits to node/lease/offer APIs
+* create a template directory and an esi\_leap\_query\_events endpoint
+
+0.2.11
+------
+
+* Fix bug with claiming offer
+* Send email notification when lease starts or ends soon Closes: #149
+
+0.2.10
+------
+
+* Add a max lease length and a default length
+* Change resource\_not\_found exceptions to 404
+
 0.2.9
 -----
 
 * Fix bug that causes expired leases to not be reflected on ironic nodes
 
 0.2.8
 -----
```

### Comparing `esi-leap-0.2.9/Containerfile` & `esi-leap-0.3.0/Containerfile`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/LICENSE` & `esi-leap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/requirements.txt` & `esi-leap-0.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/run_services.sh` & `esi-leap-0.3.0/run_services.sh`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/setup.cfg` & `esi-leap-0.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	esi-leap = esi_leap.common.policy:get_enforcer
 oslo.policy.policies = 
 	esi-leap = esi_leap.common.policy:list_rules
 console_scripts = 
 	esi-leap-api = esi_leap.cmd.api:main
 	esi-leap-dbsync = esi_leap.cmd.dbsync:main
 	esi-leap-manager = esi_leap.cmd.manager:main
+	esi-leap-email-notification = esi_leap.send_email_notification:main
 wsgi_scripts = 
 	esi-leap-api-wsgi = esi_leap.api.wsgi:initialize_wsgi_app
 esi_leap.database.migration_backend = 
 	sqlalchemy = esi_leap.db.sqlalchemy.migration
 
 [egg_info]
 tag_build =
```

### Comparing `esi-leap-0.2.9/setup.py` & `esi-leap-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     setup_requires=['pbr>=2.0.0'],
     long_description=long_description,
     long_description_content_type='text/markdown',
+    package_data={'esi_leap': ['templates/*']},
     pbr=True)
```

### Comparing `esi-leap-0.2.9/test-requirements.txt` & `esi-leap-0.3.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.9/tox.ini` & `esi-leap-0.3.0/tox.ini`

 * *Files identical despite different names*

