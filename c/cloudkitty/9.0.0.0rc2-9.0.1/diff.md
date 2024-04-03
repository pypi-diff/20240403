# Comparing `tmp/cloudkitty-9.0.0.0rc2.tar.gz` & `tmp/cloudkitty-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudkitty-9.0.0.0rc2.tar", last modified: Thu Apr  4 09:56:02 2019, max compression
+gzip compressed data, was "dist/cloudkitty-9.0.1.tar", last modified: Thu Sep 10 09:27:25 2020, max compression
```

## Comparing `cloudkitty-9.0.0.0rc2.tar` & `cloudkitty-9.0.1.tar`

### file list

```diff
@@ -1,466 +1,469 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/contrib/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       98 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/contrib/cloudkitty.logrotate
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/contrib/ci/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    17039 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/contrib/ci/csv_writer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/contrib/init/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      290 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/contrib/init/cloudkitty-processor.service
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      272 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/contrib/init/cloudkitty-api.service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/etc/cloudkitty/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1711 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/etc/cloudkitty/metrics.yml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      696 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/etc/cloudkitty/api_paste.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/etc/oslo-config-generator/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      341 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/etc/oslo-config-generator/cloudkitty.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/etc/oslo-policy-generator/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       81 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/etc/oslo-policy-generator/cloudkitty.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/etc/apache2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1447 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/etc/apache2/cloudkitty
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21424 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/ChangeLog
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5618 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/write_orchestrator.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9442 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/transformer/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2402 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/transformer/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1287 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/transformer/format.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/backend/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      922 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/backend/file.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1701 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/writer/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8262 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/writer/csv_base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5184 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/writer/csv_map.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2961 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/writer/osrf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4587 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/writer/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2961 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7159 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1313 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      912 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/env.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      979 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1020 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/307430ab38bc_improve_qty_precision.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      951 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/792b438b663_added_tenant_informations.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1085 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/c703a1bad612_improve_qty_digit.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1431 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/17fd1b237aa3_initial_migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7130 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1305 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/backends/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18301 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/backends/gnocchi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3036 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/backends/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4639 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1313 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/alembic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      900 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/alembic/env.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      494 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/alembic/versions/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1295 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/alembic/versions/03da4bb002b9_initial_revision.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5013 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12592 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v2/influx.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6239 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage/v2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1843 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4341 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1313 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      896 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/env.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      494 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/versions/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1398 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/versions/c14eea9d3cc1_initial.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1111 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/versions/d9d103dd4dcf_add_state_management_columns.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3825 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/state.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4502 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/datamodels/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1730 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/datamodels/script.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/datamodels/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/controllers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4998 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/controllers/script.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      956 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/controllers/root.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/controllers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3045 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3181 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1313 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4143 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      912 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/env.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      979 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/versions/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1360 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/versions/4f9efa4601c0_initial_migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2817 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/api.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1398 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/noop.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1704 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/field.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2639 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/mapping.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1499 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2863 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/threshold.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1649 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/group.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3687 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/field.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6749 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/mapping.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3627 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1824 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/root.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6941 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/threshold.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5189 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/group.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10889 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10128 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1313 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20871 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      905 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/env.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      979 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8713 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/f8c799db4aa0_fix_unnamed_constraints.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3079 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/4da82e1c11c8_add_per_tenant_hashmap_support.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4172 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/54cc17accf2c_fixed_constraint_name.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      883 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/10d2738b67df_rename_mapping_table_to_hashmap_mappings.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3153 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/644faa4491fd_update_tenant_id_type_from_uuid_to_text.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2455 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/4fa888fd7eda_added_threshold_support.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1691 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/c88a06b1cfce_clean_hashmap_fields_constraints.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3777 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/3dd7e13527f3_initial_migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/models/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9799 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/models/f8c799db4aa0_fix_unnamed_constraints.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/models/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12643 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4435 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/gnocchi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1331 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/source.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3689 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/keystone.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1321 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      781 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/i18n.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1728 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1745 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2437 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/storage.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1695 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/info.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2306 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/report.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2966 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/rating.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2291 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/collector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      920 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4136 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/storage.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4690 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/info.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5716 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/report.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7687 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/rating.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5869 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/collector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1356 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1694 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1809 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1978 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/hooks.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2291 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/root.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1715 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/middleware.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3082 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/app.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7982 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1808 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/example/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2317 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/example/example.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      871 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/example/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      859 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/api/app.wsgi
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1072 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/storage.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2079 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/info.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1541 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/report.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2105 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/rating.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2246 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/collector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1052 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1315 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1224 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v2/example.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v2/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2996 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1589 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/defaults.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5347 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/policy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/db/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1095 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/db/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/db/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/db/alembic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1502 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/db/alembic/env.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1119 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/db/alembic/alembic.ini
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/db/alembic/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2118 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/common/db/alembic/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1494 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_state.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2079 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/transformers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2712 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/transformers/test_base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1727 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/transformers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3449 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_orchestrator.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4257 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_rating.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      804 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/collectors/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10872 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/collectors/test_prometheus.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4897 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/collectors/test_gnocchi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4253 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/collectors/test_validation.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/collectors/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10763 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v1/test_storage.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4622 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v1/test_hybrid_storage.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v1/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v2/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4453 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v2/influx_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12273 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v2/test_storage_unit.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      555 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/ks_middleware_auth.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      851 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v2-example.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      182 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/no_auth.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3380 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-collector.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7289 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-report.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4152 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-rating.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1454 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-info.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1045 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/ks_middleware_cors.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8293 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-storage.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      377 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/root-v1-storage.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      449 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/root-v2-storage.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1109 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/test_gabbi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/gabbits/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4174 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/gabbits/pyscripts.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1187 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/test_gabbi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1044 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/fixtures.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9378 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-errors.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4780 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-location.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10066 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/hash.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      782 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-empty.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1379 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/test_gabbi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1031 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/fixtures.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1195 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/handlers.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14020 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/fixtures.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      705 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbi_paste.ini
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11434 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/samples.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12231 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_pyscripts.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1057 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_json.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1289 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v1/test_summary.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v1/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2004 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v1/test_types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v2/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5944 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v2/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5030 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_policy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4165 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_storage_state.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2821 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7086 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2914 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_keystone_fetcher.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12865 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_hacking.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    47919 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_hashmap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/cli/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1365 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/cli/test_status.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/tests/cli/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      666 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10959 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/orchestrator.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2543 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/messaging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/hacking/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/hacking/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12209 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/collector/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7013 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/collector/prometheus.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14211 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/collector/gnocchi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      694 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/collector/exceptions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9419 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/collector/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9425 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/collector/monasca.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1143 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/json_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      649 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/version.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1361 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/extension_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2935 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1313 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7616 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      896 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/env.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      979 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/versions/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      946 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/versions/385e33fef139_added_priority_to_modules_state.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1286 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/versions/464e951dc3b8_initial_migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1088 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/versions/2ac2217dcbd9_added_support_for_meta_collector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1109 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4198 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/db/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty/cli/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      991 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/cli/storage.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3888 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/cli/writer.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/cli/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4671 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/cli/dbsync.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1292 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/cli/processor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1528 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/cloudkitty/cli/status.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4077 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/PKG-INFO
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1379 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/lower-constraints.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1806 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/.zuul.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3165 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/README.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1258 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/devstack/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      498 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/devstack/apache-cloudkitty.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1257 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/devstack/files/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19965 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/devstack/files/influxdb.conf
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3297 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/devstack/settings
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    14702 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/devstack/plugin.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      910 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8359 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      147 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/queens.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/rocky.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      143 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/pike.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      152 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/ocata.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/_static/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/_templates/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/_templates/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      107 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/source/unreleased.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       97 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/remove-gnocchi-transformer-1dad750b9ba6c2e4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      179 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/deprecate-ceilometer-collector-6d8f72c84b95662b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      143 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/remove-deprecated-api-endpoints-26606e322b8a225e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      177 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/status-upgrade-check-fdcf054643e071d8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      177 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/rework-prometheus-collector-f9f34a3792888dad.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      226 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/skip-period-if-nonexistent-metric-ba56a671e68f5bf5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      336 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/add-influx-storage-backend-3ace5b451e789e64.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/deprecate-collector-mappings-5a69b31c8037fc01.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      137 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/source-fetcher-43c4352508f7f944.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      108 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/add-gnocchi-fetcher-b8a6e2ea49fcfec5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      268 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/fix-gnocchi-metadata-collection-74665e862483a383.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      123 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/deprecate-report-total-62544dce42bb19a6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      251 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/harden-dataframes-policy-7786286525e52dfb.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      106 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/add-tempest-plugin-3584e1918f344fb2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       88 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/remove-ceilometer-collector-b310bf6c5736c88a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/add-scope-key-58135c2a5c6dae68.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      315 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/added-v2-api-1ef829355c2feea4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      312 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/fix-hashmap-mapping-value-match-56570510203ce3e5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       94 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/remove-deprecated-storage-backends-158fbec099846ec7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      342 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/deprecate-info-services-endpoints-0c5018cb08a30d5f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       84 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/fix-csv-usage-end-7bcf4cb5effc4461.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       90 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/remove-fake-fetcher-9c264520a3cec9d0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      159 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/collector-monasca-f0871406513ff22c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      492 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/default-to-v2-storage-a5ecac7e73dafa6d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/remove-v2-gnocchi-storage-a83bd58008bfd92e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      200 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/rework-prometheus-collector-02bd6351d447e4fe.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/fix-lock-release-74d112c8599c9a59.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      482 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/refactor-storage-e5453296e477e594.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      291 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/deprecate_section_name-9f1ce1f84d09adf8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      182 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/change-metrology-organization-1e11900eb30780cc.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      114 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/improve-metrics-configuration-271102366f8e6fe7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      103 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/releasenotes/notes/remove-fake-meta-collectors-5ed94ab1165e9661.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      762 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/test-requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      109 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15281 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/dependency_links.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3978 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/AUTHORS
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      961 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/rtd-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6787 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/Makefile
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        6 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/.gitignore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7035 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/configuration.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2116 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/storage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/samples/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      288 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/samples/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      194 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/samples/policy-yaml.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8350 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/collector.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      319 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/policy.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      185 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3374 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/architecture.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/install/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/install/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1804 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/install/mod_wsgi.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      451 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/install/install-rdo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2053 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/install/install-source.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      581 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/install/install-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      828 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/devstack.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      760 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/sample_policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/cli/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      237 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/cli/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2114 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/admin/cli/cloudkitty-status.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2583 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8075 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/developer/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      134 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/developer/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/developer/api/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       69 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/developer/api/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      431 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/developer/api/utils.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8854 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/developer/api/tutorial.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      510 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/developer/storage.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5285 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/developer/collector.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/user/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      104 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/user/rating/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2133 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/user/rating/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5359 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/user/rating/pyscripts.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16024 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/user/rating/hashmap.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/user/rating/graph/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1229 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/user/rating/graph/hashmap.dot
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      220 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2520 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v1/v1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v1/rating/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      547 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v1/rating/pyscripts.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1608 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v1/rating/hashmap.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       55 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v2/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v2/http_status.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v2/example/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      349 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v2/example/example_parameters.yml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v2/example/http_status.yml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      837 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/api-reference/v2/example/example.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/_static/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2453 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/_static/cloudkitty.policy.yaml.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/doc/source/images/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   103564 2019-04-04 09:54:04.000000 cloudkitty-9.0.0.0rc2/doc/source/images/cloudkitty-logo.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2682 2019-04-04 09:56:02.000000 cloudkitty-9.0.0.0rc2/setup.cfg
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1897 2019-04-04 09:54:07.000000 cloudkitty-9.0.0.0rc2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2682 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/.gitignore
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8075 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/developer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5285 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/developer/collector.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/developer/storage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/developer/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/developer/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8854 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/developer/api/tutorial.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/developer/api/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/developer/api/utils.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/admin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/admin/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1804 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/install/mod_wsgi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2053 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/install/install-source.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/admin/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/cli/cloudkitty-status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/sample_policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3374 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/architecture.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/admin/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8350 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/configuration/collector.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/configuration/storage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7035 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/configuration/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/configuration/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/admin/configuration/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/configuration/samples/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/admin/configuration/samples/policy-yaml.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   103564 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/images/cloudkitty-logo.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2583 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/user/rating/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/user/rating/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16024 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/user/rating/hashmap.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5359 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/user/rating/pyscripts.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/user/rating/graph/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/user/rating/graph/hashmap.dot
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2453 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/_static/cloudkitty.policy.yaml.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/api-reference/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/api-reference/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/v2/http_status.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/api-reference/v2/example/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/v2/example/example_parameters.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/v2/example/example.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/v2/example/http_status.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/api-reference/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2520 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/v1/v1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/doc/source/api-reference/v1/rating/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/v1/rating/hashmap.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/v1/rating/pyscripts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/source/api-reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6787 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/lower-constraints.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3165 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4913 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15488 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty.egg-info/SOURCES.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/devstack/README.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14702 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/devstack/plugin.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/devstack/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19965 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/devstack/files/influxdb.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3297 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/devstack/settings
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/devstack/apache-cloudkitty.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4913 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/rtd-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21691 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1794 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4077 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/add-gnocchi-fetcher-b8a6e2ea49fcfec5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/fix-lock-release-74d112c8599c9a59.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/deprecate-report-total-62544dce42bb19a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/remove-deprecated-api-endpoints-26606e322b8a225e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/improve-metrics-configuration-271102366f8e6fe7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/remove-v2-gnocchi-storage-a83bd58008bfd92e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/fix-gnocchi-metadata-collection-74665e862483a383.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/remove-gnocchi-transformer-1dad750b9ba6c2e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/status-upgrade-check-fdcf054643e071d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/deprecate-collector-mappings-5a69b31c8037fc01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/default-to-v2-storage-a5ecac7e73dafa6d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/rework-prometheus-collector-f9f34a3792888dad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/rework-prometheus-collector-02bd6351d447e4fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/fix-csv-usage-end-7bcf4cb5effc4461.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/added-v2-api-1ef829355c2feea4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/deprecate_section_name-9f1ce1f84d09adf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/change-metrology-organization-1e11900eb30780cc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/add-scope-key-58135c2a5c6dae68.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/collector-monasca-f0871406513ff22c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/refactor-storage-e5453296e477e594.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/use-interface-param-endpoint-discovery-monasca-collector-7477e86cd7e5acf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/remove-ceilometer-collector-b310bf6c5736c88a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/deprecate-ceilometer-collector-6d8f72c84b95662b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/fix-hashmap-mapping-value-match-56570510203ce3e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/remove-deprecated-storage-backends-158fbec099846ec7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/source-fetcher-43c4352508f7f944.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/add-tempest-plugin-3584e1918f344fb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/deprecate-info-services-endpoints-0c5018cb08a30d5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/remove-fake-fetcher-9c264520a3cec9d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/harden-dataframes-policy-7786286525e52dfb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/fix-v1-storage-groupby-e865d1315bd390cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/skip-period-if-nonexistent-metric-ba56a671e68f5bf5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/add-influx-storage-backend-3ace5b451e789e64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/notes/remove-fake-meta-collectors-5ed94ab1165e9661.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8359 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/ocata.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/_templates/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/releasenotes/source/pike.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage_state/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage_state/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage_state/alembic/env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage_state/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage_state/alembic/versions/c14eea9d3cc1_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage_state/alembic/versions/d9d103dd4dcf_add_state_management_columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage_state/alembic/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage_state/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage_state/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4341 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage_state/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/json_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/extension_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4198 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/versions/385e33fef139_added_priority_to_modules_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/versions/464e951dc3b8_initial_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1088 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/versions/2ac2217dcbd9_added_support_for_meta_collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7616 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2935 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/write_orchestrator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1745 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4671 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/cli/dbsync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3888 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/cli/writer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/cli/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/cli/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1292 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/cli/processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/messaging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12865 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_hacking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1365 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/cli/test_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/cli/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/collectors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4253 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/collectors/test_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4897 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/collectors/test_gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10872 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/collectors/test_prometheus.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/collectors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5030 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12273 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v2/test_storage_unit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v2/influx_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1889 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v2/test_influxdb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10763 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v1/test_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v1/test_hybrid_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4257 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_rating.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_keystone_fetcher.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbi_paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14020 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1195 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/handlers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8293 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-storage.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7289 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-report.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-info.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4152 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-rating.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-collector.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/root-v1-storage.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/no_auth.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/ks_middleware_cors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/root-v2-storage.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v2-example.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/ks_middleware_auth.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4780 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-location.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9378 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-errors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-empty.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10066 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/hash.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/test_gabbi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4174 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/gabbits/pyscripts.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/test_gabbi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/test_gabbi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/gabbi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7086 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/transformers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/transformers/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1727 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/transformers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12231 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_pyscripts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4165 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_storage_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3449 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_orchestrator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11434 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/samples.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2821 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5944 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/api/v2/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/api/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/tests/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/api/v1/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/api/v1/test_summary.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_json.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47919 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/tests/test_hashmap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10959 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/orchestrator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3825 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/state.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12710 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v2/influx.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6239 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18301 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/backends/gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3036 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/backends/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/alembic/env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/alembic/versions/03da4bb002b9_initial_revision.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/alembic/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4639 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7130 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/792b438b663_added_tenant_informations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/307430ab38bc_improve_qty_precision.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1431 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/17fd1b237aa3_initial_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/c703a1bad612_improve_qty_digit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2961 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7180 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5013 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/storage/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/transformer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1287 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/transformer/format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2402 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/transformer/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12209 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9442 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/noop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12643 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9799 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/models/f8c799db4aa0_fix_unnamed_constraints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3079 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/4da82e1c11c8_add_per_tenant_hashmap_support.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8713 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/f8c799db4aa0_fix_unnamed_constraints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4172 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/54cc17accf2c_fixed_constraint_name.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/c88a06b1cfce_clean_hashmap_fields_constraints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/10d2738b67df_rename_mapping_table_to_hashmap_mappings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3153 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/644faa4491fd_update_tenant_id_type_from_uuid_to_text.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/4fa888fd7eda_added_threshold_support.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/3dd7e13527f3_initial_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20871 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10128 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2863 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/threshold.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/field.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1649 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/mapping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3627 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6941 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/threshold.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3687 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/field.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5189 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6749 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/mapping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10889 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/hash/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2817 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/versions/4f9efa4601c0_initial_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4143 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/datamodels/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1730 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/datamodels/script.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/datamodels/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/controllers/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/controllers/script.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/pyscripts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4502 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/rating/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/collector/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7013 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/collector/prometheus.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14211 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/collector/gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9504 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/collector/monasca.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9419 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/collector/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/collector/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1728 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/fetcher/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/fetcher/source.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4435 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/fetcher/gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3689 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/fetcher/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/fetcher/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/writer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5184 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/writer/csv_map.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2961 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/writer/osrf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8262 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/writer/csv_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/writer/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/backend/file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/backend/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/middleware.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7982 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v2/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/api/v2/example/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2317 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v2/example/example.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v2/example/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1978 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/hooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/rating.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/report.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/api/v1/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7687 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/controllers/rating.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5869 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/controllers/collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4136 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/controllers/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4690 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/controllers/info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5716 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/controllers/report.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3082 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/api/app.wsgi
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/common/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/common/db/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/common/db/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/db/alembic/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/db/alembic/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/db/alembic/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/db/alembic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/db/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/defaults.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/common/policies/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v2/example.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2105 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v1/rating.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v1/collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v1/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v1/info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v1/report.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5347 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2998 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/cloudkitty/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4023 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/.stestr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/etc/oslo-config-generator/cloudkitty.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/etc/apache2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1447 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/etc/apache2/cloudkitty
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/etc/oslo-policy-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/etc/oslo-policy-generator/cloudkitty.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/etc/cloudkitty/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/etc/cloudkitty/api_paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/etc/cloudkitty/metrics.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/contrib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/contrib/init/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/contrib/init/cloudkitty-api.service
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/contrib/init/cloudkitty-processor.service
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-10 09:27:25.000000 cloudkitty-9.0.1/contrib/ci/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    17039 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/contrib/ci/csv_writer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2020-09-10 09:26:34.000000 cloudkitty-9.0.1/contrib/cloudkitty.logrotate
```

### Comparing `cloudkitty-9.0.0.0rc2/contrib/ci/csv_writer.py` & `cloudkitty-9.0.1/contrib/ci/csv_writer.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/etc/cloudkitty/metrics.yml` & `cloudkitty-9.0.1/etc/cloudkitty/metrics.yml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/etc/cloudkitty/api_paste.ini` & `cloudkitty-9.0.1/etc/cloudkitty/api_paste.ini`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/etc/apache2/cloudkitty` & `cloudkitty-9.0.1/etc/apache2/cloudkitty`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/setup.py` & `cloudkitty-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/ChangeLog` & `cloudkitty-9.0.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 CHANGES
 =======
 
-9.0.0.0rc2
-----------
+9.0.1
+-----
+
+* [devstack] Collector Variable
+* Use "interface" option for monasca endpoint discovery
+* Fix InfluxDB storage's "\_point\_to\_dataframe\_entry" method
+* Fix section name in config file generation
+* Fix sqlalchemy grouping on v1 storage
+* OpenDev Migration Patch
+
+9.0.0
+-----
 
 * Bootstrap the v2 API
 * Update the default policy rule for /v1/storage/dataframes
 * Update the default metrics.yml file
 * Add storage backend documentation
 * Fix HashMap field mapping comparison
 * Update admin documentation for Prometheus collector
```

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/write_orchestrator.py` & `cloudkitty-9.0.1/cloudkitty/write_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/utils.py` & `cloudkitty-9.0.1/cloudkitty/utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/transformer/__init__.py` & `cloudkitty-9.0.1/cloudkitty/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/transformer/format.py` & `cloudkitty-9.0.1/cloudkitty/transformer/format.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/backend/file.py` & `cloudkitty-9.0.1/cloudkitty/backend/file.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/backend/__init__.py` & `cloudkitty-9.0.1/cloudkitty/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/writer/csv_base.py` & `cloudkitty-9.0.1/cloudkitty/writer/csv_base.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/writer/csv_map.py` & `cloudkitty-9.0.1/cloudkitty/writer/csv_map.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/writer/osrf.py` & `cloudkitty-9.0.1/cloudkitty/writer/osrf.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/writer/__init__.py` & `cloudkitty-9.0.1/cloudkitty/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/models.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/__init__.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             q = q.filter(
                 self.frame_model.res_type == service)
         q = q.filter(
             self.frame_model.begin >= begin,
             self.frame_model.end <= end,
             self.frame_model.res_type != '_NO_DATA_')
         if groupby:
-            q = q.group_by(groupby)
+            q = q.group_by(sqlalchemy.sql.text(groupby))
 
         # Order by sum(rate)
         q = q.order_by(sqlalchemy.func.sum(self.frame_model.rate))
         results = q.all()
         totallist = []
         for r in results:
             total = {model.name: value for model, value in zip(querymodels, r)}
```

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/migration.py` & `cloudkitty-9.0.1/cloudkitty/storage_state/migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/env.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/script.py.mako` & `cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/307430ab38bc_improve_qty_precision.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/307430ab38bc_improve_qty_precision.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/792b438b663_added_tenant_informations.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/792b438b663_added_tenant_informations.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/c703a1bad612_improve_qty_digit.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/c703a1bad612_improve_qty_digit.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/sqlalchemy/alembic/versions/17fd1b237aa3_initial_migration.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/versions/17fd1b237aa3_initial_migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/__init__.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/models.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/models.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/backends/gnocchi.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/backends/gnocchi.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/backends/__init__.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/__init__.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/migration.py` & `cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/alembic/env.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/alembic/env.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v1/hybrid/alembic/versions/03da4bb002b9_initial_revision.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/alembic/versions/03da4bb002b9_initial_revision.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/__init__.py` & `cloudkitty-9.0.1/cloudkitty/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v2/influx.py` & `cloudkitty-9.0.1/cloudkitty/storage/v2/influx.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,16 +266,18 @@
             output.update(group_filters)
         elif group_filters:
             output = group_filters
         return output
 
     @staticmethod
     def _point_to_dataframe_entry(point):
-        groupby = point.pop('groupby').split('|')
-        metadata = point.pop('metadata').split('|')
+        groupby = (point.pop('groupby', None) or '').split('|')
+        groupby = [g for g in groupby if g]
+        metadata = (point.pop('metadata', None) or '').split('|')
+        metadata = [m for m in metadata if m]
         return {
             'vol': {
                 'unit': point['unit'],
                 'qty': decimal.Decimal(point['qty']),
             },
             'rating': {
                 'price': point['price'],
```

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage/v2/__init__.py` & `cloudkitty-9.0.1/cloudkitty/storage/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/models.py` & `cloudkitty-9.0.1/cloudkitty/storage_state/models.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/__init__.py` & `cloudkitty-9.0.1/cloudkitty/storage_state/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/migration.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/hybrid/migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/env.py` & `cloudkitty-9.0.1/cloudkitty/storage_state/alembic/env.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/versions/c14eea9d3cc1_initial.py` & `cloudkitty-9.0.1/cloudkitty/storage_state/alembic/versions/c14eea9d3cc1_initial.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/storage_state/alembic/versions/d9d103dd4dcf_add_state_management_columns.py` & `cloudkitty-9.0.1/cloudkitty/storage_state/alembic/versions/d9d103dd4dcf_add_state_management_columns.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/state.py` & `cloudkitty-9.0.1/cloudkitty/state.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/__init__.py` & `cloudkitty-9.0.1/cloudkitty/rating/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/datamodels/script.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/datamodels/script.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/controllers/script.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/controllers/script.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/controllers/root.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/controllers/root.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/__init__.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/models.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/migration.py` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/api.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/env.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/script.py.mako` & `cloudkitty-9.0.1/cloudkitty/storage/v1/sqlalchemy/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/versions/4f9efa4601c0_initial_migration.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/versions/4f9efa4601c0_initial_migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/pyscripts/db/api.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/noop.py` & `cloudkitty-9.0.1/cloudkitty/rating/noop.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/field.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/field.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/mapping.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/mapping.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/service.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/service.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/threshold.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/threshold.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/datamodels/group.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/datamodels/group.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/field.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/field.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/mapping.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/mapping.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/service.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/service.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/root.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/root.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/threshold.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/threshold.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/controllers/group.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/controllers/group.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/__init__.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/models.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/migration.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/api.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/env.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/script.py.mako` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/f8c799db4aa0_fix_unnamed_constraints.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/f8c799db4aa0_fix_unnamed_constraints.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/4da82e1c11c8_add_per_tenant_hashmap_support.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/4da82e1c11c8_add_per_tenant_hashmap_support.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/54cc17accf2c_fixed_constraint_name.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/54cc17accf2c_fixed_constraint_name.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/10d2738b67df_rename_mapping_table_to_hashmap_mappings.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/10d2738b67df_rename_mapping_table_to_hashmap_mappings.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/644faa4491fd_update_tenant_id_type_from_uuid_to_text.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/644faa4491fd_update_tenant_id_type_from_uuid_to_text.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/4fa888fd7eda_added_threshold_support.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/4fa888fd7eda_added_threshold_support.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/c88a06b1cfce_clean_hashmap_fields_constraints.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/c88a06b1cfce_clean_hashmap_fields_constraints.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/3dd7e13527f3_initial_migration.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/versions/3dd7e13527f3_initial_migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/sqlalchemy/alembic/models/f8c799db4aa0_fix_unnamed_constraints.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/sqlalchemy/alembic/models/f8c799db4aa0_fix_unnamed_constraints.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/rating/hash/db/api.py` & `cloudkitty-9.0.1/cloudkitty/rating/hash/db/api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/gnocchi.py` & `cloudkitty-9.0.1/cloudkitty/fetcher/gnocchi.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/source.py` & `cloudkitty-9.0.1/cloudkitty/fetcher/source.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/keystone.py` & `cloudkitty-9.0.1/cloudkitty/fetcher/keystone.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/fetcher/__init__.py` & `cloudkitty-9.0.1/cloudkitty/fetcher/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/i18n.py` & `cloudkitty-9.0.1/cloudkitty/i18n.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/config.py` & `cloudkitty-9.0.1/cloudkitty/config.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/service.py` & `cloudkitty-9.0.1/cloudkitty/service.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/storage.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/storage.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/info.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/info.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/report.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/report.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/rating.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/rating.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/datamodels/collector.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/datamodels/collector.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/config.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/config.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/storage.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/controllers/storage.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/info.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/controllers/info.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/report.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/controllers/report.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/rating.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/controllers/rating.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/collector.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/controllers/collector.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/controllers/__init__.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/__init__.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/types.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/types.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v1/hooks.py` & `cloudkitty-9.0.1/cloudkitty/api/v1/hooks.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/root.py` & `cloudkitty-9.0.1/cloudkitty/api/root.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/middleware.py` & `cloudkitty-9.0.1/cloudkitty/api/middleware.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/app.py` & `cloudkitty-9.0.1/cloudkitty/api/app.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/utils.py` & `cloudkitty-9.0.1/cloudkitty/api/v2/utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/__init__.py` & `cloudkitty-9.0.1/cloudkitty/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/example/example.py` & `cloudkitty-9.0.1/cloudkitty/api/v2/example/example.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/v2/example/__init__.py` & `cloudkitty-9.0.1/cloudkitty/api/v2/example/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/api/app.wsgi` & `cloudkitty-9.0.1/cloudkitty/api/app.wsgi`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/storage.py` & `cloudkitty-9.0.1/cloudkitty/common/policies/v1/storage.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/info.py` & `cloudkitty-9.0.1/cloudkitty/common/policies/v1/info.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/report.py` & `cloudkitty-9.0.1/cloudkitty/common/policies/v1/report.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/rating.py` & `cloudkitty-9.0.1/cloudkitty/common/policies/v1/rating.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v1/collector.py` & `cloudkitty-9.0.1/cloudkitty/common/policies/v1/collector.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/base.py` & `cloudkitty-9.0.1/cloudkitty/common/policies/base.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/__init__.py` & `cloudkitty-9.0.1/cloudkitty/common/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policies/v2/example.py` & `cloudkitty-9.0.1/cloudkitty/common/policies/v2/example.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/config.py` & `cloudkitty-9.0.1/cloudkitty/common/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         cloudkitty.orchestrator.orchestrator_opts))),
     ('output', list(itertools.chain(
         cloudkitty.config.output_opts))),
     ('state', list(itertools.chain(
         cloudkitty.config.state_opts))),
     ('storage', list(itertools.chain(
         cloudkitty.storage.storage_opts))),
-    ('storage_influx', list(itertools.chain(
+    ('storage_influxdb', list(itertools.chain(
         cloudkitty.storage.v2.influx.influx_storage_opts))),
     ('storage_gnocchi', list(itertools.chain(
         cloudkitty.storage.v1.hybrid.backends.gnocchi.gnocchi_storage_opts))),
     (None, list(itertools.chain(
         cloudkitty.api.app.auth_opts,
         cloudkitty.service.service_opts))),
 ]
```

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/defaults.py` & `cloudkitty-9.0.1/cloudkitty/common/defaults.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/policy.py` & `cloudkitty-9.0.1/cloudkitty/common/policy.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/db/models.py` & `cloudkitty-9.0.1/cloudkitty/common/db/models.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/db/alembic/env.py` & `cloudkitty-9.0.1/cloudkitty/common/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/db/alembic/alembic.ini` & `cloudkitty-9.0.1/cloudkitty/common/db/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/common/db/alembic/migration.py` & `cloudkitty-9.0.1/cloudkitty/common/db/alembic/migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_state.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/utils.py` & `cloudkitty-9.0.1/cloudkitty/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/transformers/test_base.py` & `cloudkitty-9.0.1/cloudkitty/tests/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/transformers/__init__.py` & `cloudkitty-9.0.1/cloudkitty/tests/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_orchestrator.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_rating.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_config.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/collectors/test_prometheus.py` & `cloudkitty-9.0.1/cloudkitty/tests/collectors/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/collectors/test_gnocchi.py` & `cloudkitty-9.0.1/cloudkitty/tests/collectors/test_gnocchi.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/collectors/test_validation.py` & `cloudkitty-9.0.1/cloudkitty/tests/collectors/test_validation.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v1/test_storage.py` & `cloudkitty-9.0.1/cloudkitty/tests/storage/v1/test_storage.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v1/test_hybrid_storage.py` & `cloudkitty-9.0.1/cloudkitty/tests/storage/v1/test_hybrid_storage.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v2/influx_utils.py` & `cloudkitty-9.0.1/cloudkitty/tests/storage/v2/influx_utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/storage/v2/test_storage_unit.py` & `cloudkitty-9.0.1/cloudkitty/tests/storage/v2/test_storage_unit.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/ks_middleware_auth.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/ks_middleware_auth.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v2-example.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v2-example.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-collector.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-collector.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-report.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-report.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-rating.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-rating.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-info.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-info.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/ks_middleware_cors.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/ks_middleware_cors.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbits/v1-storage.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbits/v1-storage.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/test_gabbi.py` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/test_gabbi.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/gabbits/pyscripts.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/gabbits/pyscripts.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/test_gabbi.py` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/test_gabbi.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/pyscripts/fixtures.py` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/pyscripts/fixtures.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-errors.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-errors.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-location.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-location.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/hash.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/hash.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-empty.yaml` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/gabbits/hash-empty.yaml`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/test_gabbi.py` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/test_gabbi.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/rating/hash/fixtures.py` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/rating/hash/fixtures.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/handlers.py` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/handlers.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/fixtures.py` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/fixtures.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/gabbi/gabbi_paste.ini` & `cloudkitty-9.0.1/cloudkitty/tests/gabbi/gabbi_paste.ini`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/samples.py` & `cloudkitty-9.0.1/cloudkitty/tests/samples.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_pyscripts.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_pyscripts.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_json.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v1/test_summary.py` & `cloudkitty-9.0.1/cloudkitty/tests/api/v1/test_summary.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v1/test_types.py` & `cloudkitty-9.0.1/cloudkitty/tests/api/v1/test_types.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/api/v2/test_utils.py` & `cloudkitty-9.0.1/cloudkitty/tests/api/v2/test_utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_policy.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_storage_state.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_storage_state.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/__init__.py` & `cloudkitty-9.0.1/cloudkitty/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_utils.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_keystone_fetcher.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_keystone_fetcher.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_hacking.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_hacking.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/test_hashmap.py` & `cloudkitty-9.0.1/cloudkitty/tests/test_hashmap.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/tests/cli/test_status.py` & `cloudkitty-9.0.1/cloudkitty/tests/cli/test_status.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/__init__.py` & `cloudkitty-9.0.1/cloudkitty/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/orchestrator.py` & `cloudkitty-9.0.1/cloudkitty/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/messaging.py` & `cloudkitty-9.0.1/cloudkitty/messaging.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/hacking/checks.py` & `cloudkitty-9.0.1/cloudkitty/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/collector/prometheus.py` & `cloudkitty-9.0.1/cloudkitty/collector/prometheus.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/collector/gnocchi.py` & `cloudkitty-9.0.1/cloudkitty/collector/gnocchi.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/collector/exceptions.py` & `cloudkitty-9.0.1/cloudkitty/collector/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/collector/__init__.py` & `cloudkitty-9.0.1/cloudkitty/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/collector/monasca.py` & `cloudkitty-9.0.1/cloudkitty/collector/monasca.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,18 @@
         self.auth = ks_loading.load_auth_from_conf_options(
             CONF,
             COLLECTOR_MONASCA_OPTS)
         self.session = ks_loading.load_session_from_conf_options(
             CONF,
             COLLECTOR_MONASCA_OPTS,
             auth=self.auth)
-        self.ks_client = ks_client.Client(session=self.session)
+        self.ks_client = ks_client.Client(
+            session=self.session,
+            interface=CONF.collector_monasca.interface,
+        )
         self.mon_endpoint = self._get_monasca_endpoint()
         if not self.mon_endpoint:
             raise EndpointNotFound()
         self._conn = mclient.Client(
             api_version=MONASCA_API_VERSION,
             session=self.session,
             endpoint=self.mon_endpoint)
```

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/json_utils.py` & `cloudkitty-9.0.1/cloudkitty/json_utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/version.py` & `cloudkitty-9.0.1/cloudkitty/version.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/extension_manager.py` & `cloudkitty-9.0.1/cloudkitty/extension_manager.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/models.py` & `cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/migration.py` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/api.py` & `cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/env.py` & `cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/script.py.mako` & `cloudkitty-9.0.1/cloudkitty/rating/pyscripts/db/sqlalchemy/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/versions/385e33fef139_added_priority_to_modules_state.py` & `cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/versions/385e33fef139_added_priority_to_modules_state.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/versions/464e951dc3b8_initial_migration.py` & `cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/versions/464e951dc3b8_initial_migration.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/sqlalchemy/alembic/versions/2ac2217dcbd9_added_support_for_meta_collector.py` & `cloudkitty-9.0.1/cloudkitty/db/sqlalchemy/alembic/versions/2ac2217dcbd9_added_support_for_meta_collector.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/__init__.py` & `cloudkitty-9.0.1/cloudkitty/db/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/db/api.py` & `cloudkitty-9.0.1/cloudkitty/db/api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/cli/storage.py` & `cloudkitty-9.0.1/cloudkitty/cli/storage.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/cli/writer.py` & `cloudkitty-9.0.1/cloudkitty/cli/writer.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/cli/dbsync.py` & `cloudkitty-9.0.1/cloudkitty/cli/dbsync.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/cli/processor.py` & `cloudkitty-9.0.1/cloudkitty/cli/processor.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty/cli/status.py` & `cloudkitty-9.0.1/cloudkitty/cli/status.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/HACKING.rst` & `cloudkitty-9.0.1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/PKG-INFO` & `cloudkitty-9.0.1/cloudkitty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudkitty
-Version: 9.0.0.0rc2
+Version: 9.0.1
 Summary: Rating as a Service component for OpenStack
 Home-page: https://docs.openstack.org/cloudkitty/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `cloudkitty-9.0.0.0rc2/lower-constraints.txt` & `cloudkitty-9.0.1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/.zuul.yaml` & `cloudkitty-9.0.1/.zuul.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     timeout: 5400
     irrelevant-files:
       - ^.*\.rst$
       - ^doc/.*$
       - ^releasenotes/.*$
     vars:
       devstack_plugins:
-        cloudkitty: https://git.openstack.org/openstack/cloudkitty
-        cloudkitty-tempest-plugin: https://git.openstack.org/openstack/cloudkitty-tempest-plugin
+        cloudkitty: https://opendev.org/openstack/cloudkitty
+        cloudkitty-tempest-plugin: https://opendev.org/openstack/cloudkitty-tempest-plugin
       devstack_services:
         ck-api: true
         ck-proc: true
         horizon: false
         tempest: true
       tempest_concurrency: 1
       tempest_test_regex: cloudkitty_tempest_plugin.*
```

### Comparing `cloudkitty-9.0.0.0rc2/README.rst` & `cloudkitty-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/requirements.txt` & `cloudkitty-9.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/devstack/README.rst` & `cloudkitty-9.0.1/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/devstack/files/influxdb.conf` & `cloudkitty-9.0.1/devstack/files/influxdb.conf`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/devstack/settings` & `cloudkitty-9.0.1/devstack/settings`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/devstack/plugin.sh` & `cloudkitty-9.0.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/releasenotes/source/index.rst` & `cloudkitty-9.0.1/releasenotes/source/index.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/releasenotes/source/conf.py` & `cloudkitty-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/test-requirements.txt` & `cloudkitty-9.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/SOURCES.txt` & `cloudkitty-9.0.1/cloudkitty.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
 cloudkitty/tests/gabbi/rating/pyscripts/gabbits/pyscripts.yaml
 cloudkitty/tests/storage/__init__.py
 cloudkitty/tests/storage/v1/__init__.py
 cloudkitty/tests/storage/v1/test_hybrid_storage.py
 cloudkitty/tests/storage/v1/test_storage.py
 cloudkitty/tests/storage/v2/__init__.py
 cloudkitty/tests/storage/v2/influx_utils.py
+cloudkitty/tests/storage/v2/test_influxdb.py
 cloudkitty/tests/storage/v2/test_storage_unit.py
 cloudkitty/tests/transformers/__init__.py
 cloudkitty/tests/transformers/test_base.py
 cloudkitty/transformer/__init__.py
 cloudkitty/transformer/format.py
 cloudkitty/writer/__init__.py
 cloudkitty/writer/csv_base.py
@@ -329,14 +330,15 @@
 releasenotes/notes/deprecate-info-services-endpoints-0c5018cb08a30d5f.yaml
 releasenotes/notes/deprecate-report-total-62544dce42bb19a6.yaml
 releasenotes/notes/deprecate_section_name-9f1ce1f84d09adf8.yaml
 releasenotes/notes/fix-csv-usage-end-7bcf4cb5effc4461.yaml
 releasenotes/notes/fix-gnocchi-metadata-collection-74665e862483a383.yaml
 releasenotes/notes/fix-hashmap-mapping-value-match-56570510203ce3e5.yaml
 releasenotes/notes/fix-lock-release-74d112c8599c9a59.yaml
+releasenotes/notes/fix-v1-storage-groupby-e865d1315bd390cb.yaml
 releasenotes/notes/harden-dataframes-policy-7786286525e52dfb.yaml
 releasenotes/notes/improve-metrics-configuration-271102366f8e6fe7.yaml
 releasenotes/notes/refactor-storage-e5453296e477e594.yaml
 releasenotes/notes/remove-ceilometer-collector-b310bf6c5736c88a.yaml
 releasenotes/notes/remove-deprecated-api-endpoints-26606e322b8a225e.yaml
 releasenotes/notes/remove-deprecated-storage-backends-158fbec099846ec7.yaml
 releasenotes/notes/remove-fake-fetcher-9c264520a3cec9d0.yaml
@@ -344,14 +346,15 @@
 releasenotes/notes/remove-gnocchi-transformer-1dad750b9ba6c2e4.yaml
 releasenotes/notes/remove-v2-gnocchi-storage-a83bd58008bfd92e.yaml
 releasenotes/notes/rework-prometheus-collector-02bd6351d447e4fe.yaml
 releasenotes/notes/rework-prometheus-collector-f9f34a3792888dad.yaml
 releasenotes/notes/skip-period-if-nonexistent-metric-ba56a671e68f5bf5.yaml
 releasenotes/notes/source-fetcher-43c4352508f7f944.yaml
 releasenotes/notes/status-upgrade-check-fdcf054643e071d8.yaml
+releasenotes/notes/use-interface-param-endpoint-discovery-monasca-collector-7477e86cd7e5acf4.yaml
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/unreleased.rst
```

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/PKG-INFO` & `cloudkitty-9.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudkitty
-Version: 9.0.0.0rc2
+Version: 9.0.1
 Summary: Rating as a Service component for OpenStack
 Home-page: https://docs.openstack.org/cloudkitty/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/entry_points.txt` & `cloudkitty-9.0.1/cloudkitty.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/cloudkitty.egg-info/requires.txt` & `cloudkitty-9.0.1/cloudkitty.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-pbr!=2.1.0,>=2.0.0
+Flask-RESTful>=0.3.5
+Flask>=1.0.2
+PasteDeploy>=1.5.0
+SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10
+WSME>=0.8
 alembic>=0.8.0
 eventlet!=0.18.3,!=0.20.1,!=0.21.0,!=0.23.0,>=0.18.2
-keystonemiddleware>=4.0.0
 gnocchiclient>=2.5.0
-python-monascaclient>=1.9.0
-python-keystoneclient!=2.1.0,>=1.9.0
-keystoneauth1>=2.1.0
+influxdb!=5.2.0,>=5.1.0
 iso8601>=0.1.9
-PasteDeploy>=1.5.0
-pecan!=1.0.2,!=1.0.3,!=1.0.4,!=1.2,>=1.0.0
-WSME>=0.8
+keystoneauth1>=2.1.0
+keystonemiddleware>=4.0.0
+oslo.concurrency>=3.5.0
 oslo.config!=4.3.0,!=4.4.0,>=3.7.0
 oslo.context>=2.9.0
-oslo.concurrency>=3.5.0
 oslo.db>=4.1.0
 oslo.i18n>=2.1.0
 oslo.log>=1.14.0
 oslo.messaging!=9.0.0,>=5.24.2
 oslo.middleware>=3.27.0
 oslo.policy>=0.5.0
-oslo.utils>=3.5.0
 oslo.upgradecheck>=0.1.1
-SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10
+oslo.utils>=3.5.0
+pbr!=2.1.0,>=2.0.0
+pecan!=1.0.2,!=1.0.3,!=1.0.4,!=1.2,>=1.0.0
+python-keystoneclient!=2.1.0,>=1.9.0
+python-monascaclient>=1.9.0
 six>=1.9.0
 stevedore>=1.5.0
 tooz>=1.28.0
 voluptuous>=0.11.1
-influxdb!=5.2.0,>=5.1.0
-Flask>=1.0.2
-Flask-RESTful>=0.3.5
```

### Comparing `cloudkitty-9.0.0.0rc2/LICENSE` & `cloudkitty-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/AUTHORS` & `cloudkitty-9.0.1/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Aaron-DH <344677472@qq.com>
 Aaron-DH <dinghh@awcloud.com>
+Abraham Arce <abraham.arce.moreno@intel.com>
 Adam <adammxa@126.com>
 Andreas Jaeger <aj@suse.com>
 Arundhati Surpur <arundhati@nectechnologies.in>
 Bertrand Lallau <bertrand.lallau@gmail.com>
 Cedric Brandily <zzelle@gmail.com>
 Chaozhe.Chen <chaozhe.chen@easystack.cn>
 Chris Dent <cdent@anticdent.org>
```

### Comparing `cloudkitty-9.0.0.0rc2/rtd-requirements.txt` & `cloudkitty-9.0.1/rtd-requirements.txt`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/Makefile` & `cloudkitty-9.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/configuration.rst` & `cloudkitty-9.0.1/doc/source/admin/configuration/configuration.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/storage.rst` & `cloudkitty-9.0.1/doc/source/admin/configuration/storage.rst`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
    [database]
 
    connection = mysql+pymysql://cloudkitty_user:cloudkitty_password@mariadb_host/cloudkitty_database
 
 InfluxDB (v2)
 -------------
 
-Section: ``storage_influx``.
+Section: ``storage_influxdb``.
 
 * ``username``: InfluxDB username.
 
 * ``password``: InfluxDB password.
 
 * ``database``: InfluxDB database.
```

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/configuration/collector.rst` & `cloudkitty-9.0.1/doc/source/admin/configuration/collector.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/architecture.rst` & `cloudkitty-9.0.1/doc/source/admin/architecture.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/install/mod_wsgi.rst` & `cloudkitty-9.0.1/doc/source/admin/install/mod_wsgi.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/install/install-source.rst` & `cloudkitty-9.0.1/doc/source/admin/install/install-source.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/install/install-ubuntu.rst` & `cloudkitty-9.0.1/doc/source/admin/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/devstack.rst` & `cloudkitty-9.0.1/doc/source/admin/devstack.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 DevStack installation
 =====================
 
 Add the following lines in your ``local.conf`` file to enable CloudKitty,
 Ceilometer and Gnocchi. By default, the fetcher will be ``gnocchi``
 (configurable via the ``CLOUDKITTY_FETCHER`` variable), the collector will be
-``gnocchi`` (configurable via the ``CLOUDKITTY_GNOCCHI`` variable), and the
+``gnocchi`` (configurable via the ``CLOUDKITTY_COLLECTOR`` variable), and the
 storage backend will be ``influxdb`` (configurable via the
 ``CLOUDKITTY_STORAGE_BACKEND`` and ``CLOUDKITTY_STORAGE_VERSION`` variables).
 
 .. code-block:: ini
 
     [[local|localrc]]
     # ceilometer
```

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/sample_policy.rst` & `cloudkitty-9.0.1/doc/source/admin/sample_policy.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/admin/cli/cloudkitty-status.rst` & `cloudkitty-9.0.1/doc/source/admin/cli/cloudkitty-status.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/index.rst` & `cloudkitty-9.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/conf.py` & `cloudkitty-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/developer/api/tutorial.rst` & `cloudkitty-9.0.1/doc/source/developer/api/tutorial.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/developer/collector.rst` & `cloudkitty-9.0.1/doc/source/developer/collector.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/user/rating/index.rst` & `cloudkitty-9.0.1/doc/source/user/rating/index.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/user/rating/pyscripts.rst` & `cloudkitty-9.0.1/doc/source/user/rating/pyscripts.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/user/rating/hashmap.rst` & `cloudkitty-9.0.1/doc/source/user/rating/hashmap.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/user/rating/graph/hashmap.dot` & `cloudkitty-9.0.1/doc/source/user/rating/graph/hashmap.dot`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/api-reference/v1/v1.rst` & `cloudkitty-9.0.1/doc/source/api-reference/v1/v1.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/api-reference/v1/rating/pyscripts.rst` & `cloudkitty-9.0.1/doc/source/api-reference/v1/rating/pyscripts.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/api-reference/v1/rating/hashmap.rst` & `cloudkitty-9.0.1/doc/source/api-reference/v1/rating/hashmap.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/api-reference/v2/example/example.inc` & `cloudkitty-9.0.1/doc/source/api-reference/v2/example/example.inc`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/_static/cloudkitty.policy.yaml.sample` & `cloudkitty-9.0.1/doc/source/_static/cloudkitty.policy.yaml.sample`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/doc/source/images/cloudkitty-logo.png` & `cloudkitty-9.0.1/doc/source/images/cloudkitty-logo.png`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/setup.cfg` & `cloudkitty-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloudkitty-9.0.0.0rc2/tox.ini` & `cloudkitty-9.0.1/tox.ini`

 * *Files identical despite different names*

