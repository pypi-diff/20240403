# Comparing `tmp/aodh-9.0.0.0rc1.tar.gz` & `tmp/aodh-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aodh-9.0.0.0rc1.tar", last modified: Wed Sep 25 08:55:14 2019, max compression
+gzip compressed data, was "dist/aodh-9.0.1.tar", last modified: Mon Jun 15 09:35:45 2020, max compression
```

## Comparing `aodh-9.0.0.0rc1.tar` & `aodh-9.0.1.tar`

### file list

```diff
@@ -1,360 +1,360 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/.testr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/conf/defaults.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2472 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/app.wsgi
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8369 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32115 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarms.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8782 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/gnocchi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3972 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/composite.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/loadbalancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15167 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/query.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4221 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13255 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/v2/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1780 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/controllers/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4332 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/policies.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5287 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3708 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/api/rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9264 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/coordination.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17911 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/impl_sqlalchemy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/bb07adac380_add_severity_to_alarm_history.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3997 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/12fe8fac9fe4_initial_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/367aadf5485f_precisetimestamp_to_datetime.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/f8c31b1ffe11_add_index_for_enabled_and_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/6ae0d05d9451_add_reason_column.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3726 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3741 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/impl_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4868 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8125 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5498 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/storage/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional_live/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional_live/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional_live/gabbi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional_live/gabbi/test_gabbi_live.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional_live/gabbi/gabbits-live/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4070 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional_live/gabbi/gabbits-live/alarms.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional_live/gabbi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3855 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional/hooks/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      706 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/hooks/post_test_hook.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6651 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/test_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/test_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1118 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_wsme_custom_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   119579 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_alarm_scenarios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9676 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_complex_query.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/policy.json-test
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7711 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15085 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_complex_query_scenarios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14204 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_query.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/sqlalchemy/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1367 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/test_impl_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22604 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/test_storage_scenarios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/test_impl_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3260 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/storage/test_get_connection.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1175 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/test_gabbi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/middleware.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5515 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/alarms.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/capabilities.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/basic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/healthcheck.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4623 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4204 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/test_bin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/test_messaging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2319 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/test_api_v2_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21026 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/test_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/cmd/test_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/test_event.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/unit/notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4396 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/notifier/test_heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/notifier/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/notifier/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6058 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/test_evaluator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28671 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_gnocchi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1857 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5657 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_loadbalancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18632 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6397 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22214 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_composite.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9997 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/unit/test_coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/tests/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/zh_TW/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3427 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/zh_TW/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5016 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/en_GB/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3655 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/zh_CN/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/pt/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4032 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/pt/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4750 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/pt_BR/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4441 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/ja/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3647 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/es/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6973 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/ru/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4366 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/de/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3680 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/fr/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5010 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/ko_KR/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh/locale/it/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3656 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/locale/it/LC_MESSAGES/aodh.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/cmd/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       27 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/cmd/aodh-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/cmd/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/cmd/aodh-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/cmd/alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2342 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/messaging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5484 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/notifier/heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5914 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/notifier/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4500 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/notifier/rest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/notifier/log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8876 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/notifier/zaqar.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/notifier/test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/notifier/trust.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4663 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/keystone_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh/evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7505 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/evaluator/gnocchi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9229 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/evaluator/composite.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9482 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/evaluator/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7027 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/evaluator/threshold.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10160 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/evaluator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5490 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/evaluator/loadbalancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1661 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/evaluator/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2130 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/queue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2454 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/aodh/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4092 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/setup.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/aodh.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10139 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/aodh.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/MAINTAINERS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9869 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1918 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/cli/aodh-status.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22090 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/admin/telemetry-alarms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/admin/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2259 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/configure-common.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1631 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/get_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5524 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/prereq-common.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/verify.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1632 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/install/install-obs.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/contributing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/contributor/webapi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/webapi/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3390 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/webapi/v2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/contributor/releasenotes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/releasenotes/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/event-alarm.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2608 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/testing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/contributor/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/install/mod_wsgi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/install/development.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/install/manual.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/contributor/install/uwsgi.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/configuration/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/configuration/aodh-config-options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/configuration/sample-policy-yaml.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/configuration/aodh-config-file.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6027 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/doc/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/bindep.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2173 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/.zuul.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/rally-jobs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/rally-jobs/extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/rally-jobs/extra/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/rally-jobs/extra/fake.img
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/rally-jobs/plugins/plugin_sample.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/rally-jobs/plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5118 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/rally-jobs/ceilometer.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/rally-jobs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/keystone-v3-support-ffc0f804dbe9d7e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/pecan-debug-removed-7c7a528a1aea98bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/queue-communication-1b884feab4078dde.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/loadbalancer-evaluator-85732c5e5f6e11e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/deprecate-threshold-alarm-d89da351d4f6f50f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/mysql-precise-datetime-e374c77e6707985e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/remove-combination-alarms-a1a53655f3f7d1d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/fix-empty-statistics-3852da99b1c0b297.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/fix-rbac-50825144e0897d7d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/fix-ssl-request-8107616b6a85a217.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/fix-ceilometerclient-init-8bc7a6742937c3e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/add-a-data-migration-tool-daa14b0cb5d4cc62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/partition-coordinator-improvement-ff1c257f69f120ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/enable-aodh-service-multi-processes-67ed9a0b7fac69aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/bug1540395-reason-string-0aad56966007d0e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/gnocchi-capability-cache-75d011e77b8ecc72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/auto-healing-notifier-794b64de776811e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/remove-no-sql-drivers-21dfdbd750751340.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/remove-threshold-alarm-a7901991d2da09f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/Add-state-reason-to-the-API-7bc5a9465466db2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/fix-gnocchi-aggregation-eval-7c2c1c67bdf2d11c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/remove-alarm-name-unique-constraint-4fb0b14f3ad46f0b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/ingestion-lag-2317725887287fbc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/gnocchi-client-a62ca5a0c717807e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/gnocchi-external-resource-owner-3fad253d30746b0d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/deprecate-nosql-backends-13079883eec7e8e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/deprecate-combination-alarms-7ff26b73b61a0e59.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/support-combination-to-composite-conversion-3e688a6b7d01a57e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/event-listener-batch-support-04e6ff159ef34d8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/policy-in-code-79edd9282f1e4603.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/fix-combination-alarms-8097adf08b837a50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/healthcheck-560700b72ae68e18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/notifier-batch-listener-01796e2cb06344dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/composite-alarm-1b1ca9ea0e8f55c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/remove-eventlet-18ada1cff213af5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/notes/add-upgrade-check-framework-ab35e6eb65504bc3.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5266 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8427 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/ocata.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18963 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2646 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17217 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16098 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2229 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/stein.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11578 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1203 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/devstack/settings
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/devstack/apache-aodh.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13356 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2843 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:55:14.000000 aodh-9.0.0.0rc1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      426 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/tools/pretty_tox.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/README.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/run-tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1990 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   120943 2019-09-25 08:55:13.000000 aodh-9.0.0.0rc1/ChangeLog
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      522 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/run-functional-tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2019-09-25 08:53:59.000000 aodh-9.0.0.0rc1/HACKING.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-15 09:34:02.000000 aodh-9.0.1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2842 2020-06-15 09:34:02.000000 aodh-9.0.1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2020-06-15 09:34:02.000000 aodh-9.0.1/bindep.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   121145 2020-06-15 09:35:45.000000 aodh-9.0.1/ChangeLog
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      522 2020-06-15 09:34:02.000000 aodh-9.0.1/run-functional-tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2020-06-15 09:34:02.000000 aodh-9.0.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-06-15 09:34:02.000000 aodh-9.0.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2020-06-15 09:34:02.000000 aodh-9.0.1/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2020-06-15 09:34:02.000000 aodh-9.0.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2020-06-15 09:34:02.000000 aodh-9.0.1/MAINTAINERS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2020-06-15 09:35:45.000000 aodh-9.0.1/PKG-INFO
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2020-06-15 09:34:02.000000 aodh-9.0.1/run-tests.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2472 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/event.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/conf/defaults.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9264 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2130 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/queue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/profiler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/storage/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/storage/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3741 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/bb07adac380_add_severity_to_alarm_history.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/367aadf5485f_precisetimestamp_to_datetime.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3997 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/12fe8fac9fe4_initial_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/f8c31b1ffe11_add_index_for_enabled_and_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/6ae0d05d9451_add_reason_column.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3726 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17911 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/impl_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5498 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8125 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/impl_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4868 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2342 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/messaging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       27 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/cmd/aodh-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/cmd/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/cmd/aodh-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/cmd/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/cmd/alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/notifier/test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/notifier/log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/notifier/trust.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8876 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/notifier/zaqar.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5914 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/notifier/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4445 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/notifier/heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4500 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/notifier/rest.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional_live/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional_live/gabbi/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional_live/gabbi/gabbits-live/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4070 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional_live/gabbi/gabbits-live/alarms.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional_live/gabbi/test_gabbi_live.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional_live/gabbi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional_live/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional/gabbi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1175 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/gabbi/test_gabbi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/healthcheck.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/middleware.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/capabilities.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5515 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/alarms.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/basic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4623 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/gabbi/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/gabbi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/storage/test_impl_log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional/storage/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/storage/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/storage/sqlalchemy/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1367 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/storage/test_impl_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22604 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/storage/test_storage_scenarios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3260 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/storage/test_get_connection.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional/hooks/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      706 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/hooks/post_test_hook.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3855 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/test_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/test_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6651 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/functional/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9676 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/test_complex_query.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   119579 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/test_alarm_scenarios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15085 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/test_complex_query_scenarios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/test_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/policy.json-test
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7711 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/test_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14204 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/test_query.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1118 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/functional/api/v2/test_wsme_custom_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2319 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/test_api_v2_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6058 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/test_evaluator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/test_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9997 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/test_coordination.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/cmd/test_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/cmd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/unit/notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3113 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/notifier/test_heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/notifier/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/notifier/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4204 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/test_bin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21026 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/tests/unit/evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22214 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/evaluator/test_composite.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28671 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/evaluator/test_gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5657 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/evaluator/test_loadbalancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18632 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/evaluator/test_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1857 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/evaluator/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/evaluator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6397 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/evaluator/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/tests/unit/test_messaging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6973 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/ru/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/it/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3656 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/it/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5010 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/ko_KR/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3655 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/zh_CN/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/pt/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4032 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/pt/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5016 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/en_GB/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/zh_TW/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3427 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/zh_TW/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3647 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/es/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3680 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/fr/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4750 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/pt_BR/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4366 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/de/LC_MESSAGES/aodh.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4441 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/locale/ja/LC_MESSAGES/aodh.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9482 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/evaluator/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5519 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/evaluator/loadbalancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1661 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/evaluator/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9229 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/evaluator/composite.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7027 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/evaluator/threshold.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10160 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/evaluator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7505 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/evaluator/gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2454 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5287 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/app.wsgi
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/api-paste.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1780 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/api/controllers/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15167 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/query.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32241 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/alarms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13255 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/loadbalancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3972 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/composite.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8782 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8369 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4221 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/controllers/v2/capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3708 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4332 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/api/policies.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4869 2020-06-15 09:34:02.000000 aodh-9.0.1/aodh/keystone_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2020-06-15 09:34:02.000000 aodh-9.0.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2020-06-15 09:34:02.000000 aodh-9.0.1/CONTRIBUTING.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6027 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/contributing.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/contributor/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/install/manual.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/install/uwsgi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/install/mod_wsgi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/install/development.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/event-alarm.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2608 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/testing.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/contributor/releasenotes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/releasenotes/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/contributor/webapi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/webapi/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3390 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/contributor/webapi/v2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1631 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/verify.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/get_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1632 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/install-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5524 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/prereq-common.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2259 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/configure-common.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/glossary.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/configuration/aodh-config-file.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/configuration/sample-policy-yaml.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/configuration/aodh-config-options.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/configuration/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9869 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22090 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/admin/telemetry-alarms.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1918 2020-06-15 09:34:02.000000 aodh-9.0.1/doc/source/cli/aodh-status.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      426 2020-06-15 09:34:02.000000 aodh-9.0.1/tools/pretty_tox.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4092 2020-06-15 09:35:45.000000 aodh-9.0.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2020-06-15 09:34:02.000000 aodh-9.0.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13356 2020-06-15 09:35:45.000000 aodh-9.0.1/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5118 2020-06-15 09:34:02.000000 aodh-9.0.1/rally-jobs/ceilometer.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2020-06-15 09:34:02.000000 aodh-9.0.1/rally-jobs/plugins/plugin_sample.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2020-06-15 09:34:02.000000 aodh-9.0.1/rally-jobs/plugins/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/rally-jobs/extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/rally-jobs/extra/fake.img
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-06-15 09:34:02.000000 aodh-9.0.1/rally-jobs/extra/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2020-06-15 09:34:02.000000 aodh-9.0.1/rally-jobs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/ingestion-lag-2317725887287fbc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/mysql-precise-datetime-e374c77e6707985e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/notifier-batch-listener-01796e2cb06344dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/gnocchi-external-resource-owner-3fad253d30746b0d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/gnocchi-client-a62ca5a0c717807e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/event-listener-batch-support-04e6ff159ef34d8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/gnocchi-capability-cache-75d011e77b8ecc72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/support-combination-to-composite-conversion-3e688a6b7d01a57e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/add-a-data-migration-tool-daa14b0cb5d4cc62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/keystone-v3-support-ffc0f804dbe9d7e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/fix-gnocchi-aggregation-eval-7c2c1c67bdf2d11c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/deprecate-threshold-alarm-d89da351d4f6f50f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/auto-healing-notifier-794b64de776811e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/partition-coordinator-improvement-ff1c257f69f120ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/fix-empty-statistics-3852da99b1c0b297.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/deprecate-combination-alarms-7ff26b73b61a0e59.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/remove-no-sql-drivers-21dfdbd750751340.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/policy-in-code-79edd9282f1e4603.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/remove-threshold-alarm-a7901991d2da09f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/Add-state-reason-to-the-API-7bc5a9465466db2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/deprecate-nosql-backends-13079883eec7e8e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/remove-alarm-name-unique-constraint-4fb0b14f3ad46f0b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/fix-combination-alarms-8097adf08b837a50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/remove-eventlet-18ada1cff213af5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/add-upgrade-check-framework-ab35e6eb65504bc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/pecan-debug-removed-7c7a528a1aea98bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/enable-aodh-service-multi-processes-67ed9a0b7fac69aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/fix-ssl-request-8107616b6a85a217.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/healthcheck-560700b72ae68e18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/remove-combination-alarms-a1a53655f3f7d1d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/composite-alarm-1b1ca9ea0e8f55c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/fix-ceilometerclient-init-8bc7a6742937c3e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/bug1540395-reason-string-0aad56966007d0e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/fix-rbac-50825144e0897d7d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/loadbalancer-evaluator-85732c5e5f6e11e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/notes/queue-communication-1b884feab4078dde.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5266 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/ocata.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2229 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18963 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2646 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16098 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17217 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8427 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/liberty.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-06-15 09:34:02.000000 aodh-9.0.1/releasenotes/source/pike.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2020-06-15 09:34:02.000000 aodh-9.0.1/devstack/apache-aodh.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1203 2020-06-15 09:34:02.000000 aodh-9.0.1/devstack/settings
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11578 2020-06-15 09:34:02.000000 aodh-9.0.1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2020-06-15 09:34:02.000000 aodh-9.0.1/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10139 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-06-15 09:35:45.000000 aodh-9.0.1/aodh.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2173 2020-06-15 09:34:02.000000 aodh-9.0.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1990 2020-06-15 09:34:02.000000 aodh-9.0.1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2020-06-15 09:34:02.000000 aodh-9.0.1/README.rst
```

### Comparing `aodh-9.0.0.0rc1/PKG-INFO` & `aodh-9.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aodh
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: OpenStack Telemetry Alarming
 Home-page: https://docs.openstack.org/aodh/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: aodh
         ====
@@ -31,11 +31,11 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: System :: Monitoring
+Provides-Extra: mysql
+Provides-Extra: postgresql
 Provides-Extra: zaqar
 Provides-Extra: test
-Provides-Extra: postgresql
-Provides-Extra: mysql
```

### Comparing `aodh-9.0.0.0rc1/setup.py` & `aodh-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/LICENSE` & `aodh-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/conf/defaults.py` & `aodh-9.0.1/aodh/conf/defaults.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/profiler.py` & `aodh-9.0.1/aodh/profiler.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/event.py` & `aodh-9.0.1/aodh/event.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/service.py` & `aodh-9.0.1/aodh/service.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/__init__.py` & `aodh-9.0.1/aodh/__init__.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/api-paste.ini` & `aodh-9.0.1/aodh/api/api-paste.ini`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/hooks.py` & `aodh-9.0.1/aodh/api/hooks.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/__init__.py` & `aodh-9.0.1/aodh/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/app.wsgi` & `aodh-9.0.1/aodh/api/app.wsgi`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/base.py` & `aodh-9.0.1/aodh/api/controllers/v2/base.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarms.py` & `aodh-9.0.1/aodh/api/controllers/v2/alarms.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,20 +458,22 @@
                         url = urlparse.SplitResult(url.scheme, netloc,
                                                    url.path, url.query,
                                                    url.fragment)
                         actions[index] = url.geturl()
         if trust_id is not None and not trust_id_used:
             prev_trust_ids.add(trust_id)
         for old_trust_id in prev_trust_ids:
-            keystone_client.delete_trust_id(old_trust_id, auth_plugin)
+            keystone_client.delete_trust_id(pecan.request.cfg, old_trust_id,
+                                            auth_plugin)
 
     def delete_actions(self):
         auth_plugin = pecan.request.environ.get('keystone.token_auth')
         for trust_id in self._get_existing_trust_ids():
-            keystone_client.delete_trust_id(trust_id, auth_plugin)
+            keystone_client.delete_trust_id(pecan.request.cfg, trust_id,
+                                            auth_plugin)
 
 
 Alarm.add_attributes(**{"%s_rule" % ext.name: ext.plugin
                         for ext in ALARMS_RULES})
 
 
 class AlarmChange(base.Base):
```

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/gnocchi.py` & `aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/gnocchi.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/composite.py` & `aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/composite.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/event.py` & `aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/event.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/alarm_rules/loadbalancer.py` & `aodh-9.0.1/aodh/api/controllers/v2/alarm_rules/loadbalancer.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/query.py` & `aodh-9.0.1/aodh/api/controllers/v2/query.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/capabilities.py` & `aodh-9.0.1/aodh/api/controllers/v2/capabilities.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/root.py` & `aodh-9.0.1/aodh/api/controllers/v2/root.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/v2/utils.py` & `aodh-9.0.1/aodh/api/controllers/v2/utils.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/controllers/root.py` & `aodh-9.0.1/aodh/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/policies.py` & `aodh-9.0.1/aodh/api/policies.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/app.py` & `aodh-9.0.1/aodh/api/app.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/middleware.py` & `aodh-9.0.1/aodh/api/middleware.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/api/rbac.py` & `aodh-9.0.1/aodh/api/rbac.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/coordination.py` & `aodh-9.0.1/aodh/coordination.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/impl_sqlalchemy.py` & `aodh-9.0.1/aodh/storage/impl_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/script.py.mako` & `aodh-9.0.1/aodh/storage/sqlalchemy/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/bb07adac380_add_severity_to_alarm_history.py` & `aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/bb07adac380_add_severity_to_alarm_history.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/12fe8fac9fe4_initial_base.py` & `aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/12fe8fac9fe4_initial_base.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/367aadf5485f_precisetimestamp_to_datetime.py` & `aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/367aadf5485f_precisetimestamp_to_datetime.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/f8c31b1ffe11_add_index_for_enabled_and_type.py` & `aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/f8c31b1ffe11_add_index_for_enabled_and_type.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/versions/6ae0d05d9451_add_reason_column.py` & `aodh-9.0.1/aodh/storage/sqlalchemy/alembic/versions/6ae0d05d9451_add_reason_column.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/env.py` & `aodh-9.0.1/aodh/storage/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/alembic/alembic.ini` & `aodh-9.0.1/aodh/storage/sqlalchemy/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/models.py` & `aodh-9.0.1/aodh/storage/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/sqlalchemy/utils.py` & `aodh-9.0.1/aodh/storage/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/impl_log.py` & `aodh-9.0.1/aodh/storage/impl_log.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/__init__.py` & `aodh-9.0.1/aodh/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/base.py` & `aodh-9.0.1/aodh/storage/base.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/storage/models.py` & `aodh-9.0.1/aodh/storage/models.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional_live/gabbi/test_gabbi_live.py` & `aodh-9.0.1/aodh/tests/functional_live/gabbi/test_gabbi_live.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional_live/gabbi/gabbits-live/alarms.yaml` & `aodh-9.0.1/aodh/tests/functional_live/gabbi/gabbits-live/alarms.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/db.py` & `aodh-9.0.1/aodh/tests/functional/db.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/hooks/post_test_hook.sh` & `aodh-9.0.1/aodh/tests/functional/hooks/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/__init__.py` & `aodh-9.0.1/aodh/tests/functional/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/test_app.py` & `aodh-9.0.1/aodh/tests/functional/api/test_app.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/test_versions.py` & `aodh-9.0.1/aodh/tests/functional/api/test_versions.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_wsme_custom_type.py` & `aodh-9.0.1/aodh/tests/functional/api/v2/test_wsme_custom_type.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_alarm_scenarios.py` & `aodh-9.0.1/aodh/tests/functional/api/v2/test_alarm_scenarios.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_complex_query.py` & `aodh-9.0.1/aodh/tests/functional/api/v2/test_complex_query.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/__init__.py` & `aodh-9.0.1/aodh/tests/functional/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_capabilities.py` & `aodh-9.0.1/aodh/tests/functional/api/v2/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_app.py` & `aodh-9.0.1/aodh/tests/functional/api/v2/test_app.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_complex_query_scenarios.py` & `aodh-9.0.1/aodh/tests/functional/api/v2/test_complex_query_scenarios.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/api/v2/test_query.py` & `aodh-9.0.1/aodh/tests/functional/api/v2/test_query.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/storage/sqlalchemy/test_migrations.py` & `aodh-9.0.1/aodh/tests/functional/storage/sqlalchemy/test_migrations.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/storage/test_impl_sqlalchemy.py` & `aodh-9.0.1/aodh/tests/functional/storage/test_impl_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/storage/test_storage_scenarios.py` & `aodh-9.0.1/aodh/tests/functional/storage/test_storage_scenarios.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/storage/test_impl_log.py` & `aodh-9.0.1/aodh/tests/functional/storage/test_impl_log.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/storage/test_get_connection.py` & `aodh-9.0.1/aodh/tests/functional/storage/test_get_connection.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/test_gabbi.py` & `aodh-9.0.1/aodh/tests/functional/gabbi/test_gabbi.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/middleware.yaml` & `aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/middleware.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/alarms.yaml` & `aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/alarms.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/gabbits/basic.yaml` & `aodh-9.0.1/aodh/tests/functional/gabbi/gabbits/basic.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/functional/gabbi/fixtures.py` & `aodh-9.0.1/aodh/tests/functional/gabbi/fixtures.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/test_bin.py` & `aodh-9.0.1/aodh/tests/unit/test_bin.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/test_messaging.py` & `aodh-9.0.1/aodh/tests/unit/test_messaging.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/test_api_v2_capabilities.py` & `aodh-9.0.1/aodh/tests/unit/test_api_v2_capabilities.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/test_notifier.py` & `aodh-9.0.1/aodh/tests/unit/test_notifier.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/cmd/test_status.py` & `aodh-9.0.1/aodh/tests/unit/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/test_event.py` & `aodh-9.0.1/aodh/tests/unit/test_event.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/notifier/test_heat.py` & `aodh-9.0.1/aodh/tests/unit/notifier/test_heat.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,50 +17,15 @@
 
 from aodh.notifier import heat as heat_notifier
 from aodh.tests.unit.notifier import base
 
 
 class TestTrustHeatAlarmNotifier(base.TestNotifierBase):
     @mock.patch("aodh.keystone_client.get_heat_client_from_trust")
-    def test_notify_with_tags(self, mock_heatclient):
-        action = netutils.urlsplit("trust+autohealer://fake_trust_id:delete@")
-        alarm_id = "fake_alarm_id"
-        alarm_name = "fake_alarm_name"
-        severity = "low"
-        previous = "ok"
-        current = "alarm"
-        reason = "no good reason"
-        reason_data = {
-            "stack_id": "fake_stack_id",
-            "asg_id": "fake_asg_id",
-            "unhealthy_members": [
-                {"tags": ["3bd8bc5a-7632-11e9-84cd-00224d6b7bc1"]}
-            ]
-        }
-
-        notifier = heat_notifier.TrustHeatAlarmNotifier(self.conf)
-        notifier.notify(action, alarm_id, alarm_name, severity, previous,
-                        current, reason, reason_data)
-
-        mock_heatclient.assert_called_once_with(self.conf, "fake_trust_id")
-
-        mock_client = mock_heatclient.return_value
-        mock_client.resources.mark_unhealthy.assert_called_once_with(
-            "fake_asg_id",
-            "3bd8bc5a-7632-11e9-84cd-00224d6b7bc1",
-            True,
-            "unhealthy load balancer member"
-        )
-
-        mock_client.stacks.update.assert_called_once_with(
-            "fake_stack_id", existing=True
-        )
-
-    @mock.patch("aodh.keystone_client.get_heat_client_from_trust")
-    def test_notify_without_tags(self, mock_heatclient):
+    def test_notify(self, mock_heatclient):
         action = netutils.urlsplit("trust+autohealer://fake_trust_id:delete@")
         alarm_id = "fake_alarm_id"
         alarm_name = "fake_alarm_name"
         severity = "low"
         previous = "ok"
         current = "alarm"
         reason = "no good reason"
@@ -70,15 +35,15 @@
             "unhealthy_members": [
                 {"id": "3bd8bc5a-7632-11e9-84cd-00224d6b7bc1"}
             ]
         }
 
         class FakeResource(object):
             def __init__(self, resource_name):
-                self.resource_name = resource_name
+                self.parent_resource = resource_name
 
         mock_client = mock_heatclient.return_value
         mock_client.resources.list.return_value = [
             FakeResource("fake_resource_name")
         ]
 
         notifier = heat_notifier.TrustHeatAlarmNotifier(self.conf)
```

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/notifier/base.py` & `aodh-9.0.1/aodh/tests/unit/notifier/base.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/test_evaluator.py` & `aodh-9.0.1/aodh/tests/unit/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_gnocchi.py` & `aodh-9.0.1/aodh/tests/unit/evaluator/test_gnocchi.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/base.py` & `aodh-9.0.1/aodh/tests/unit/evaluator/base.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_loadbalancer.py` & `aodh-9.0.1/aodh/tests/unit/evaluator/test_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_event.py` & `aodh-9.0.1/aodh/tests/unit/evaluator/test_event.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_base.py` & `aodh-9.0.1/aodh/tests/unit/evaluator/test_base.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/evaluator/test_composite.py` & `aodh-9.0.1/aodh/tests/unit/evaluator/test_composite.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/unit/test_coordination.py` & `aodh-9.0.1/aodh/tests/unit/test_coordination.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/base.py` & `aodh-9.0.1/aodh/tests/base.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/tests/constants.py` & `aodh-9.0.1/aodh/tests/constants.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/zh_TW/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/zh_TW/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/en_GB/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/en_GB/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/zh_CN/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/zh_CN/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/pt/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/pt/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/pt_BR/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/pt_BR/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/ja/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/ja/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/es/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/es/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/ru/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/ru/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/de/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/de/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/fr/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/fr/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/ko_KR/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/ko_KR/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/locale/it/LC_MESSAGES/aodh.po` & `aodh-9.0.1/aodh/locale/it/LC_MESSAGES/aodh.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/cmd/status.py` & `aodh-9.0.1/aodh/cmd/status.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/cmd/__init__.py` & `aodh-9.0.1/aodh/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/cmd/storage.py` & `aodh-9.0.1/aodh/cmd/storage.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/cmd/alarm.py` & `aodh-9.0.1/aodh/cmd/alarm.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/messaging.py` & `aodh-9.0.1/aodh/messaging.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/notifier/heat.py` & `aodh-9.0.1/aodh/notifier/heat.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from oslo_log import log
-from oslo_utils import uuidutils
 import six
 
 from aodh import keystone_client as aodh_keystone
 from aodh import notifier
 
 LOG = log.getLogger(__name__)
 
@@ -38,26 +37,14 @@
     fails, the stack could be recovered by marking the given autoscaling group
     member unhealthy, then update Heat stack in place. In order to do that, the
     notifier needs to know:
 
     - Heat top/root stack ID.
     - Heat autoscaling group ID.
     - The failed Octavia pool members.
-
-    In order to find which autoscaling group member that the failed pool member
-    belongs to, there are two ways supported(both ways require specific
-    definition in the Heat template):
-
-    1. The autoscaling group member resource ID is saved in the Octavia member
-       tag, the user should define that using 'tags' property of the
-       OS::Octavia::PoolMember resource. So, only Octavia stable/stein or later
-       versions are supported.
-    2. User customizes the autoscaling group member resource identifier
-       according to
-       https://docs.openstack.org/heat/latest/template_guide/composition.html#making-your-template-resource-more-transparent
     """
 
     def __init__(self, conf):
         super(TrustHeatAlarmNotifier, self).__init__(conf)
         self.conf = conf
 
     def notify(self, action, alarm_id, alarm_name, severity, previous, current,
@@ -88,33 +75,28 @@
             return
 
         heat_client = aodh_keystone.get_heat_client_from_trust(
             self.conf, trust_id
         )
 
         for member in unhealthy_members:
-            for tag in member.get("tags", []):
-                if uuidutils.is_uuid_like(tag):
-                    unhealthy_resources.append(tag)
+            target_resources = heat_client.resources.list(
+                stack_id, nested_depth=3,
+                filters={"physical_resource_id": member["id"]}
+            )
+            if len(target_resources) > 0:
+                # There should be only one item.
+                unhealthy_resources.append(
+                    target_resources[0].parent_resource
+                )
 
         if not unhealthy_resources:
-            # Fall back to search resource by the pool member ID.
-            for member in unhealthy_members:
-                target_resources = heat_client.resources.list(
-                    stack_id, nested_depth=3, filters={"id": member["id"]})
-                if len(target_resources) > 0:
-                    # There should be only one item.
-                    unhealthy_resources.append(
-                        target_resources[0].resource_name)
-
-            # If we still can't find expected resources, do nothing.
-            if not unhealthy_resources:
-                LOG.warning("No unhealthy resource found for the alarm %s",
-                            alarm_id)
-                return
+            LOG.warning("No unhealthy resource found for the alarm %s",
+                        alarm_id)
+            return
 
         try:
             for res in unhealthy_resources:
                 heat_client.resources.mark_unhealthy(
                     asg_id,
                     res,
                     True,
```

### Comparing `aodh-9.0.0.0rc1/aodh/notifier/__init__.py` & `aodh-9.0.1/aodh/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/notifier/rest.py` & `aodh-9.0.1/aodh/notifier/rest.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/notifier/log.py` & `aodh-9.0.1/aodh/notifier/log.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/notifier/zaqar.py` & `aodh-9.0.1/aodh/notifier/zaqar.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/notifier/test.py` & `aodh-9.0.1/aodh/notifier/test.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/notifier/trust.py` & `aodh-9.0.1/aodh/notifier/trust.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/i18n.py` & `aodh-9.0.1/aodh/i18n.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/keystone_client.py` & `aodh-9.0.1/aodh/keystone_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 import os
 
 from heatclient import client as heatclient
 from keystoneauth1 import exceptions as ka_exception
 from keystoneauth1.identity.generic import password
 from keystoneauth1 import loading as ka_loading
-from keystoneauth1 import session
 from keystoneclient.v3 import client as ks_client_v3
 from oslo_config import cfg
 
 
 CFG_GROUP = "service_credentials"
 
 
@@ -48,46 +47,48 @@
         username=conf[CFG_GROUP].username,
         password=conf[CFG_GROUP].password,
         auth_url=conf[CFG_GROUP].auth_url,
         user_domain_id=conf[CFG_GROUP].user_domain_id,
         user_domain_name=conf[CFG_GROUP].user_domain_name,
         trust_id=trust_id)
 
-    sess = session.Session(auth=auth_plugin)
+    sess = ka_loading.load_session_from_conf_options(conf, CFG_GROUP,
+                                                     auth=auth_plugin)
     return ks_client_v3.Client(session=sess)
 
 
 def get_auth_token(client):
     return client.session.auth.get_access(client.session).auth_token
 
 
-def get_client_on_behalf_user(auth_plugin):
+def get_client_on_behalf_user(conf, auth_plugin):
     """Return a client for keystone v3 endpoint."""
-    sess = session.Session(auth=auth_plugin)
+    sess = ka_loading.load_session_from_conf_options(conf, CFG_GROUP,
+                                                     auth=auth_plugin)
     return ks_client_v3.Client(session=sess)
 
 
 def create_trust_id(conf, trustor_user_id, trustor_project_id, roles,
                     auth_plugin):
     """Create a new trust using the aodh service user."""
     admin_client = get_client(conf)
     trustee_user_id = admin_client.session.get_user_id()
 
-    client = get_client_on_behalf_user(auth_plugin)
+    client = get_client_on_behalf_user(conf, auth_plugin)
     trust = client.trusts.create(trustor_user=trustor_user_id,
                                  trustee_user=trustee_user_id,
                                  project=trustor_project_id,
                                  impersonation=True,
                                  role_names=roles)
     return trust.id
 
 
-def delete_trust_id(trust_id, auth_plugin):
+def delete_trust_id(conf, trust_id, auth_plugin):
     """Delete a trust previously setup for the aodh user."""
-    client = get_client_on_behalf_user(auth_plugin)
+    client = get_client_on_behalf_user(conf, auth_plugin)
     try:
         client.trusts.delete(trust_id)
     except ka_exception.NotFound:
         pass
 
 
 def url_for(conf, **kwargs):
@@ -97,15 +98,15 @@
 
 def get_heat_client_from_trust(conf, trust_id):
     ks_client = get_trusted_client(conf, trust_id)
     sess = ks_client.session
 
     endpoint = sess.get_endpoint(
         service_type='orchestration',
-        interface="internal",
+        interface=conf.service_credentials.interface,
         region_name=conf.service_credentials.region_name
     )
 
     return heatclient.Client("1", endpoint=endpoint, session=sess)
 
 
 OPTS = [
```

### Comparing `aodh-9.0.0.0rc1/aodh/evaluator/gnocchi.py` & `aodh-9.0.1/aodh/evaluator/gnocchi.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/evaluator/composite.py` & `aodh-9.0.1/aodh/evaluator/composite.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/evaluator/event.py` & `aodh-9.0.1/aodh/evaluator/event.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/evaluator/threshold.py` & `aodh-9.0.1/aodh/evaluator/threshold.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/evaluator/__init__.py` & `aodh-9.0.1/aodh/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/evaluator/loadbalancer.py` & `aodh-9.0.1/aodh/evaluator/loadbalancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     @property
     def lb_client(self):
         if self._lb_client is None:
             endpoint = aodh_keystone.url_for(
                 self.conf,
                 service_type='load-balancer',
-                interface="internal",
+                interface=self.conf.service_credentials.interface,
                 region_name=self.conf.service_credentials.region_name
             )
             self._lb_client = octavia.OctaviaAPI(
                 session=aodh_keystone.get_session(self.conf),
                 service_type='load-balancer',
                 endpoint=endpoint
             )
```

### Comparing `aodh-9.0.0.0rc1/aodh/evaluator/utils.py` & `aodh-9.0.1/aodh/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/queue.py` & `aodh-9.0.1/aodh/queue.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/opts.py` & `aodh-9.0.1/aodh/opts.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh/utils.py` & `aodh-9.0.1/aodh/utils.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/setup.cfg` & `aodh-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh.egg-info/PKG-INFO` & `aodh-9.0.1/aodh.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aodh
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: OpenStack Telemetry Alarming
 Home-page: https://docs.openstack.org/aodh/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: aodh
         ====
@@ -31,11 +31,11 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: System :: Monitoring
+Provides-Extra: mysql
+Provides-Extra: postgresql
 Provides-Extra: zaqar
 Provides-Extra: test
-Provides-Extra: postgresql
-Provides-Extra: mysql
```

### Comparing `aodh-9.0.0.0rc1/aodh.egg-info/requires.txt` & `aodh-9.0.1/aodh.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh.egg-info/SOURCES.txt` & `aodh-9.0.1/aodh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/aodh.egg-info/entry_points.txt` & `aodh-9.0.1/aodh.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/conf.py` & `aodh-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/index.rst` & `aodh-9.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/cli/aodh-status.rst` & `aodh-9.0.1/doc/source/cli/aodh-status.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/admin/telemetry-alarms.rst` & `aodh-9.0.1/doc/source/admin/telemetry-alarms.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/install/install-ubuntu.rst` & `aodh-9.0.1/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/install/configure-common.rst` & `aodh-9.0.1/doc/source/install/configure-common.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/install/install-rdo.rst` & `aodh-9.0.1/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/install/get_started.rst` & `aodh-9.0.1/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/install/prereq-common.rst` & `aodh-9.0.1/doc/source/install/prereq-common.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/install/install-obs.rst` & `aodh-9.0.1/doc/source/install/install-obs.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/contributing.rst` & `aodh-9.0.1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/webapi/index.rst` & `aodh-9.0.1/doc/source/contributor/webapi/index.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/webapi/v2.rst` & `aodh-9.0.1/doc/source/contributor/webapi/v2.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/index.rst` & `aodh-9.0.1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/releasenotes/index.rst` & `aodh-9.0.1/doc/source/contributor/releasenotes/index.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/event-alarm.rst` & `aodh-9.0.1/doc/source/contributor/event-alarm.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/architecture.rst` & `aodh-9.0.1/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/testing.rst` & `aodh-9.0.1/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/install/mod_wsgi.rst` & `aodh-9.0.1/doc/source/contributor/install/mod_wsgi.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/install/development.rst` & `aodh-9.0.1/doc/source/contributor/install/development.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/install/manual.rst` & `aodh-9.0.1/doc/source/contributor/install/manual.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/install/index.rst` & `aodh-9.0.1/doc/source/contributor/install/index.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/contributor/install/uwsgi.rst` & `aodh-9.0.1/doc/source/contributor/install/uwsgi.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/configuration/aodh-config-file.rst` & `aodh-9.0.1/doc/source/configuration/aodh-config-file.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/source/glossary.rst` & `aodh-9.0.1/doc/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/doc/Makefile` & `aodh-9.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/CONTRIBUTING.rst` & `aodh-9.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/.zuul.yaml` & `aodh-9.0.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/rally-jobs/plugins/plugin_sample.py` & `aodh-9.0.1/rally-jobs/plugins/plugin_sample.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/rally-jobs/ceilometer.yaml` & `aodh-9.0.1/rally-jobs/ceilometer.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/rally-jobs/README.rst` & `aodh-9.0.1/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/notes/queue-communication-1b884feab4078dde.yaml` & `aodh-9.0.1/releasenotes/notes/queue-communication-1b884feab4078dde.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/notes/fix-rbac-50825144e0897d7d.yaml` & `aodh-9.0.1/releasenotes/notes/fix-rbac-50825144e0897d7d.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/notes/gnocchi-external-resource-owner-3fad253d30746b0d.yaml` & `aodh-9.0.1/releasenotes/notes/gnocchi-external-resource-owner-3fad253d30746b0d.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/notes/policy-in-code-79edd9282f1e4603.yaml` & `aodh-9.0.1/releasenotes/notes/policy-in-code-79edd9282f1e4603.yaml`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/source/newton.rst` & `aodh-9.0.1/releasenotes/source/newton.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/source/conf.py` & `aodh-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `aodh-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po` & `aodh-9.0.1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `aodh-9.0.1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `aodh-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `aodh-9.0.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `aodh-9.0.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/devstack/plugin.sh` & `aodh-9.0.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/devstack/settings` & `aodh-9.0.1/devstack/settings`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/devstack/README.rst` & `aodh-9.0.1/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/AUTHORS` & `aodh-9.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/tox.ini` & `aodh-9.0.1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 minversion = 1.6
 skipsdist = True
 envlist = py{27,37}{,-mysql,-postgresql},functional,pep8
 
 [testenv]
 # NOTE(tonyb): This project has chosen to *NOT* consume upper-constraints.txt
 usedevelop = True
-install_command = pip install -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master} {opts} {packages}
+install_command = pip install -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train} {opts} {packages}
 setenv =
     AODH_TEST_DRIVERS=postgresql mysql
     mysql: AODH_TEST_DRIVERS=mysql
     postgresql: AODH_TEST_DRIVERS=postgresql
 
     AODH_TEST_DEPS=postgresql,mysql
     mysql: AODH_TEST_DEPS=mysql
```

### Comparing `aodh-9.0.0.0rc1/.mailmap` & `aodh-9.0.1/.mailmap`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/ChangeLog` & `aodh-9.0.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 CHANGES
 =======
 
-9.0.0.0rc1
-----------
+9.0.1
+-----
+
+* Use config options when creating keystone session
+* heat notifier: Fix getting unhealthy resource names
+* Update TOX/UPPER\_CONSTRAINTS\_FILE for stable/train
+* Update .gitreview for stable/train
+
+9.0.0
+-----
 
 * Update the constraints url
 * PDF documentation build
 * Update jsonschema according to requirements
 * Run 'telemetry-dsvm-integration-ipv6-only' job in gate
 * Add the native zuulv3 jobs instead of legacy way
 * Add \_static folder to fix docs build error
```

### Comparing `aodh-9.0.0.0rc1/run-functional-tests.sh` & `aodh-9.0.1/run-functional-tests.sh`

 * *Files identical despite different names*

### Comparing `aodh-9.0.0.0rc1/requirements.txt` & `aodh-9.0.1/requirements.txt`

 * *Files identical despite different names*

