# Comparing `tmp/blazar-9.0.0.tar.gz` & `tmp/blazar-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blazar-9.0.0.tar", last modified: Wed Mar 30 11:43:19 2022, max compression
+gzip compressed data, was "blazar-9.0.0.0rc1.tar", last modified: Tue Mar  8 12:17:58 2022, max compression
```

## Comparing `blazar-9.0.0.tar` & `blazar-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,456 +1,456 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.573046 blazar-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-03-30 11:42:44.000000 blazar-9.0.0/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      579 2022-03-30 11:42:44.000000 blazar-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4408 2022-03-30 11:43:19.000000 blazar-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2022-03-30 11:42:44.000000 blazar-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29798 2022-03-30 11:43:19.000000 blazar-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2022-03-30 11:42:44.000000 blazar-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2022-03-30 11:42:44.000000 blazar-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-03-30 11:42:44.000000 blazar-9.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3278 2022-03-30 11:43:19.573046 blazar-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1762 2022-03-30 11:42:44.000000 blazar-9.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.485046 blazar-9.0.0/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.501046 blazar-9.0.0/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3890 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.501046 blazar-9.0.0/api-ref/source/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/v1/floatingips.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/v1/global-request-id.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8823 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/v1/hosts.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/v1/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14673 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/v1/leases.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15609 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/v1/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2022-03-30 11:42:44.000000 blazar-9.0.0/api-ref/source/v1/request-ids.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-03-30 11:42:44.000000 blazar-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.505046 blazar-9.0.0/blazar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.505046 blazar-9.0.0/blazar/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/root.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.509046 blazar-9.0.0/blazar/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6120 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/api_version_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3302 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/app.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.509046 blazar-9.0.0/blazar/api/v1/floatingips/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/floatingips/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/floatingips/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1784 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/floatingips/v1_0.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.509046 blazar-9.0.0/blazar/api/v1/leases/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/leases/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2880 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/leases/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2115 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/leases/v1_0.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.509046 blazar-9.0.0/blazar/api/v1/oshosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/oshosts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3454 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/oshosts/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/oshosts/v1_0.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/request_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2908 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/request_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/rest_api_version_history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12378 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v1/validation.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.509046 blazar-9.0.0/blazar/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/app.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.509046 blazar-9.0.0/blazar/api/v2/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2876 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/controllers/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.513046 blazar-9.0.0/blazar/api/v2/controllers/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/controllers/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5897 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/controllers/extensions/host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6002 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/controllers/extensions/lease.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4132 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/controllers/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/hooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.513046 blazar-9.0.0/blazar/api/v2/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5431 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/v2/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1483 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/api/wsgi_app.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.513046 blazar-9.0.0/blazar/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/cmd/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1627 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/cmd/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3085 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.513046 blazar-9.0.0/blazar/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14591 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1573 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.513046 blazar-9.0.0/blazar/db/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3335 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.513046 blazar-9.0.0/blazar/db/migration/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2661 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.517046 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3868 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/02e2f2186d98_resource_property.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5668 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/0_1_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1565 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/10e34bba18e8_add_service_name_to_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/1fd6c2eded89_add_trust_id_to_comp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/23d6240b51b2_add_status_to_leases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/2bcfe76b0474_change_tenant_to_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/35b314cd39ee_add_az_in_compute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/6bfd1c23aa18_allow_duplicate_lease_names.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3304 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/75a74e4539cb_update_lease_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/7f1a7bbb2cd2_add_aggregate_id_field_into_the_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/8805be233864_instance_reservation_table.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1427 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/9593f3656974_no_affinity_instance_reservation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2203 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/97d2cad1504e_add_fields_for_resource_monitoring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/ba75b766b64e_add_before_end_into_computehost.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/c0ae6b08b0d7_resource_properties_in_instance_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2001 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/e069c014356d_add_floatingip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/e66f199a5414_delete_unused_status_related_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3514 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/f4084140f608_add_floatingip_reservation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3743 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/migration/cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.521046 blazar-9.0.0/blazar/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38193 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/sqlalchemy/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/sqlalchemy/facade_wrapper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1699 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/sqlalchemy/model_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12540 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/sqlalchemy/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/sqlalchemy/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12349 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/sqlalchemy/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4552 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/db/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.521046 blazar-9.0.0/blazar/enforcement/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/enforcement/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3619 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/enforcement/enforcement.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/enforcement/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.521046 blazar-9.0.0/blazar/enforcement/filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/enforcement/filters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/enforcement/filters/base_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/enforcement/filters/max_lease_duration_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3088 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.521046 blazar-9.0.0/blazar/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1914 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.521046 blazar-9.0.0/blazar/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1150 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6317 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.521046 blazar-9.0.0/blazar/manager/floatingips/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/floatingips/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/floatingips/rpcapi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.525046 blazar-9.0.0/blazar/manager/leases/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/leases/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/leases/rpcapi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.525046 blazar-9.0.0/blazar/manager/oshosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/oshosts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2937 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/oshosts/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37171 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/manager/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.525046 blazar-9.0.0/blazar/monitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/monitor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/monitor/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5271 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/monitor/notification_monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2095 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/monitor/polling_monitor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.525046 blazar-9.0.0/blazar/notification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/notification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/notification/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2065 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/notification/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2078 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.525046 blazar-9.0.0/blazar/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6634 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/dummy_vm_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.525046 blazar-9.0.0/blazar/plugins/floatingips/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/floatingips/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18100 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/floatingips/floatingip_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.525046 blazar-9.0.0/blazar/plugins/instances/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/instances/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35478 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/instances/instance_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.525046 blazar-9.0.0/blazar/plugins/oshosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/oshosts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39310 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/plugins/oshosts/host_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.529046 blazar-9.0.0/blazar/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/policies/floatingips.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/policies/leases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3378 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/policies/oshosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3920 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12588 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.529046 blazar-9.0.0/blazar/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2729 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.529046 blazar-9.0.0/blazar/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10318 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/test_acl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4025 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1903 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/test_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6121 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/test_version_selector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.533046 blazar-9.0.0/blazar/tests/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.533046 blazar-9.0.0/blazar/tests/api/v1/leases/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/leases/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/leases/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8446 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/leases/test_v1_0.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.533046 blazar-9.0.0/blazar/tests/api/v1/oshosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/oshosts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1582 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/oshosts/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11645 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/oshosts/test_v1_0.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4750 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/test_api_version_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3458 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/test_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5597 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v1/test_validation.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.533046 blazar-9.0.0/blazar/tests/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15672 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v2/test_hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14101 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/api/v2/test_leases.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.533046 blazar-9.0.0/blazar/tests/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/cmd/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.533046 blazar-9.0.0/blazar/tests/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.537046 blazar-9.0.0/blazar/tests/db/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24615 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/migration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/migration/test_migrations.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7059 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/migration/test_migrations.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.537046 blazar-9.0.0/blazar/tests/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43757 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/sqlalchemy/test_sqlalchemy_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16946 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/sqlalchemy/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/db/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.537046 blazar-9.0.0/blazar/tests/enforcement/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/enforcement/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.537046 blazar-9.0.0/blazar/tests/enforcement/filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/enforcement/filters/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9732 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/enforcement/filters/test_max_lease_duration_filter.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10772 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/enforcement/test_enforcement.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/fake_lease.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1618 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/fake_requests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.537046 blazar-9.0.0/blazar/tests/local_hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/local_hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1427 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/local_hacking/test_hacking.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.537046 blazar-9.0.0/blazar/tests/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1924 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/manager/test_rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    73427 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/manager/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.537046 blazar-9.0.0/blazar/tests/monitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/monitor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4256 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/monitor/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3500 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/monitor/test_notification_monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/monitor/test_polling_monitor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.541046 blazar-9.0.0/blazar/tests/notification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/notification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/notification/test_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.541046 blazar-9.0.0/blazar/tests/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.541046 blazar-9.0.0/blazar/tests/plugins/floatingips/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/plugins/floatingips/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39555 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/plugins/floatingips/test_floatingip_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.541046 blazar-9.0.0/blazar/tests/plugins/instances/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/plugins/instances/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71658 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/plugins/instances/test_instance_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.541046 blazar-9.0.0/blazar/tests/plugins/oshosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/plugins/oshosts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   111539 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/plugins/oshosts/test_physical_host_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4242 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2314 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2396 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16300 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.541046 blazar-9.0.0/blazar/tests/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.545046 blazar-9.0.0/blazar/tests/utils/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4383 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/openstack/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5049 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/openstack/test_keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6174 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/openstack/test_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24815 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/openstack/test_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25831 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/openstack/test_placement.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3808 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/test_plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3862 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/tests/utils/test_trusts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.545046 blazar-9.0.0/blazar/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1094 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.545046 blazar-9.0.0/blazar/utils/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2763 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/openstack/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2335 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/openstack/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6525 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/openstack/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6437 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/openstack/neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22173 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/openstack/nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17908 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/openstack/placement.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3662 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3179 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/utils/trusts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2022-03-30 11:42:44.000000 blazar-9.0.0/blazar/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.505046 blazar-9.0.0/blazar.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3278 2022-03-30 11:43:19.000000 blazar-9.0.0/blazar.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14782 2022-03-30 11:43:19.000000 blazar-9.0.0/blazar.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-30 11:43:19.000000 blazar-9.0.0/blazar.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2022-03-30 11:43:19.000000 blazar-9.0.0/blazar.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-30 11:43:19.000000 blazar-9.0.0/blazar.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-30 11:43:19.000000 blazar-9.0.0/blazar.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2022-03-30 11:43:19.000000 blazar-9.0.0/blazar.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-03-30 11:43:19.000000 blazar-9.0.0/blazar.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.545046 blazar-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8343 2022-03-30 11:42:44.000000 blazar-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2022-03-30 11:42:44.000000 blazar-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.545046 blazar-9.0.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.493046 blazar-9.0.0/doc/api_samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.545046 blazar-9.0.0/doc/api_samples/floatingips/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/floatingips/floatingip-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/floatingips/floatingip-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/floatingips/floatingip-details-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/floatingips/floatingip-list-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.549046 blazar-9.0.0/doc/api_samples/hosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      645 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/allocation-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/allocation-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-details-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-property-list-detail.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-property-list.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-property-update-res.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-property-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/hosts/host-update-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.549046 blazar-9.0.0/doc/api_samples/leases/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/leases/lease-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/leases/lease-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/leases/lease-details-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3631 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/leases/lease-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/leases/lease-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/api_samples/leases/lease-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.553046 blazar-9.0.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.553046 blazar-9.0.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/admin/blazar-status.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1507 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/admin/usage-enforcement.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.553046 blazar-9.0.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15744 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/cli/floatingip-reservation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13259 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/cli/host-reservation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9696 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/cli/instance-reservation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8242 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.553046 blazar-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/configuration/blazar-conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/configuration/blazar-policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      502 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/configuration/nova-conf.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.553046 blazar-9.0.0/doc/source/configuration/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/configuration/samples/blazar-conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/configuration/samples/blazar-policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.553046 blazar-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/contributor/contribution.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/contributor/development.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/contributor/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.557046 blazar-9.0.0/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18674 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/blazar-architecture-old.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18114 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/blazar-architecture.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17477 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/event_statuses.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/healing_flow.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55752 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/lease_statuses.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24998 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/reservation_statuses.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.557046 blazar-9.0.0/doc/source/images/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/source/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/source/event_statuses.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/source/healing_flow.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/source/lease_statuses.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/images/source/reservation_statuses.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.557046 blazar-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/install/install-dashboard.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/install/install-using-devstack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3918 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/install/install-without-devstack.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.557046 blazar-9.0.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/reference/api-microversion-history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.557046 blazar-9.0.0/doc/source/restapi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/restapi/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.561046 blazar-9.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3300 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/user/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/user/compute-host-monitor.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5812 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/user/introduction.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4012 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/user/resource-monitoring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4138 2022-03-30 11:42:44.000000 blazar-9.0.0/doc/source/user/state-machines.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.493046 blazar-9.0.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.561046 blazar-9.0.0/etc/blazar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-30 11:42:44.000000 blazar-9.0.0/etc/blazar/README-blazar.conf.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-03-30 11:42:44.000000 blazar-9.0.0/etc/blazar/blazar-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-03-30 11:42:44.000000 blazar-9.0.0/etc/blazar/blazar-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2062 2022-03-30 11:42:44.000000 blazar-9.0.0/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7473 2022-03-30 11:42:44.000000 blazar-9.0.0/pylintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.493046 blazar-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.569046 blazar-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/add-newly-allocated-hosts-to-aggregate-95bb75410afc6b8d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/alembic-fix-alter-column-42a87657992d1e78.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/api-microversioning-141e473bff34aad2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/before-end-actions-7e53e740e006195a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/blazar-status-upgrade-check-framework-895079486d8085f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/bug-1779660-b623de868955e7d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/bug-1786031-800a33c681fafdc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/bug-1786031-836c6d6acae08403.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/bug-1847821-2f9d6e61f438dc4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/bug-1880646-f1af8c48f895f00e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/bug-1881162-ebe012fcc7176594.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/bug-1957761-8b126a392c0c79ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/bug-1958307-63bf308ca6a97068.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/cleaning-time-825d148b704b0c56.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/create-extra-capabilities-in-update-host-c74ce75c88e88c67.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/delete-on-end-3a6d3ced93ffed25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/deprecate-climate-filter-f1ffca52a7a4e70c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/deprecate-json-formatted-policy-file-5ceba2a580b69101.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/devstack-dashboard-1b96128952e64c1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/drop-python2-support-148148077280122c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/floatingip-reservation-6c2f3c3ad8843948.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/floatingip-reservation-update-f53c0c6239ccf9ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/global_request_id-f30e900f20752c2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/host-allocation-dates-6da5ac1ec9befa8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/host-dashboard-570a9971be1a86ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/internal-endpoint-interface-748511b8b25455c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/issue-instance-reservation-7b3c0868caaabc85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/move-hosts-back-to-freepool-041fcda9fb3fc6c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/move-specs-cf3568febaaf3b1c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/multi-freepools-9d88b1f79c330a3c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/new-instance-reservation-1f3cbfe21146e251.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/no-affinity-instance-reservation-d356e33088772ea3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/periodic-healing-143ed251d990580b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/policy-in-code-3107271b0636fcea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/prevent-delete-during-events-c206a8f0a116798c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/python3-support-d9657c136cad2a41.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/region-in-placement-client-dfbd0bcd09f81aac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/remove-climate-fb62d72ca8fc5c7d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/remove-old-instance-reservation-60820d8afe00819e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/request_id-0ebc34f09c6d01f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/resource-allocation-api-f2fff51fc4556cd4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/resource-monitoring-622b6ebcb7472cf2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/resource-property-discovery-42df197a1a49bd76.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/response-code-fix-in-rocky-2197a9c1516a0ac4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/state-machine-37be751ed54c1c75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/update-reserved-capacity-9f079395959f4474.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/update-used-extra-capability-6d7bc7fa23c91295.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/upgrade-info-1a5b8bfbb323d525.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/notes/usage-enforcement-f997ce618f542104.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.573046 blazar-9.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.573046 blazar-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.573046 blazar-9.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8563 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-03-30 11:42:44.000000 blazar-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1343 2022-03-30 11:42:44.000000 blazar-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2022-03-30 11:43:19.577046 blazar-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-30 11:42:44.000000 blazar-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2022-03-30 11:42:44.000000 blazar-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:43:19.573046 blazar-9.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2014 2022-03-30 11:42:44.000000 blazar-9.0.0/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3598 2022-03-30 11:42:44.000000 blazar-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.675523 blazar-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      579 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4408 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29808 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2022-03-08 12:17:58.675523 blazar-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1762 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.591520 blazar-9.0.0.0rc1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.603520 blazar-9.0.0.0rc1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3890 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.603520 blazar-9.0.0.0rc1/api-ref/source/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/v1/floatingips.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/v1/global-request-id.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8823 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/v1/hosts.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/v1/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14673 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/v1/leases.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15609 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/v1/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/api-ref/source/v1/request-ids.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.607520 blazar-9.0.0.0rc1/blazar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.611520 blazar-9.0.0.0rc1/blazar/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/root.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.611520 blazar-9.0.0.0rc1/blazar/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6120 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/api_version_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3302 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/app.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.611520 blazar-9.0.0.0rc1/blazar/api/v1/floatingips/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/floatingips/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/floatingips/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1784 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/floatingips/v1_0.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.611520 blazar-9.0.0.0rc1/blazar/api/v1/leases/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/leases/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2880 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/leases/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2115 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/leases/v1_0.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.611520 blazar-9.0.0.0rc1/blazar/api/v1/oshosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/oshosts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3454 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/oshosts/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/oshosts/v1_0.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/request_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2908 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/request_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/rest_api_version_history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12378 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v1/validation.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.611520 blazar-9.0.0.0rc1/blazar/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/app.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.615521 blazar-9.0.0.0rc1/blazar/api/v2/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2876 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/controllers/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.615521 blazar-9.0.0.0rc1/blazar/api/v2/controllers/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/controllers/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5897 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/controllers/extensions/host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6002 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/controllers/extensions/lease.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4132 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/controllers/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/hooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.615521 blazar-9.0.0.0rc1/blazar/api/v2/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5431 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/v2/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1483 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/api/wsgi_app.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.615521 blazar-9.0.0.0rc1/blazar/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/cmd/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1627 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/cmd/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3085 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.615521 blazar-9.0.0.0rc1/blazar/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14591 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1573 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.615521 blazar-9.0.0.0rc1/blazar/db/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3335 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.615521 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2661 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.619521 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3868 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/02e2f2186d98_resource_property.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5668 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/0_1_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1565 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/10e34bba18e8_add_service_name_to_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/1fd6c2eded89_add_trust_id_to_comp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/23d6240b51b2_add_status_to_leases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/2bcfe76b0474_change_tenant_to_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/35b314cd39ee_add_az_in_compute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/6bfd1c23aa18_allow_duplicate_lease_names.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3304 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/75a74e4539cb_update_lease_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/7f1a7bbb2cd2_add_aggregate_id_field_into_the_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/8805be233864_instance_reservation_table.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1427 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/9593f3656974_no_affinity_instance_reservation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2203 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/97d2cad1504e_add_fields_for_resource_monitoring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/ba75b766b64e_add_before_end_into_computehost.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/c0ae6b08b0d7_resource_properties_in_instance_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2001 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/e069c014356d_add_floatingip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/e66f199a5414_delete_unused_status_related_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3514 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/f4084140f608_add_floatingip_reservation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3743 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/migration/cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.623521 blazar-9.0.0.0rc1/blazar/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38193 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/sqlalchemy/facade_wrapper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1699 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/sqlalchemy/model_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12540 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/sqlalchemy/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12349 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/sqlalchemy/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4552 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/db/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.623521 blazar-9.0.0.0rc1/blazar/enforcement/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/enforcement/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3619 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/enforcement/enforcement.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/enforcement/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.623521 blazar-9.0.0.0rc1/blazar/enforcement/filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/enforcement/filters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/enforcement/filters/base_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/enforcement/filters/max_lease_duration_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3088 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.623521 blazar-9.0.0.0rc1/blazar/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1914 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.623521 blazar-9.0.0.0rc1/blazar/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1150 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6317 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.623521 blazar-9.0.0.0rc1/blazar/manager/floatingips/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/floatingips/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/floatingips/rpcapi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.623521 blazar-9.0.0.0rc1/blazar/manager/leases/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/leases/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/leases/rpcapi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.623521 blazar-9.0.0.0rc1/blazar/manager/oshosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/oshosts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2937 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/oshosts/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37171 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/manager/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.627521 blazar-9.0.0.0rc1/blazar/monitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/monitor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/monitor/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5271 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/monitor/notification_monitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2095 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/monitor/polling_monitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.627521 blazar-9.0.0.0rc1/blazar/notification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/notification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/notification/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2065 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/notification/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2078 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.627521 blazar-9.0.0.0rc1/blazar/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6634 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/dummy_vm_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.627521 blazar-9.0.0.0rc1/blazar/plugins/floatingips/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/floatingips/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18100 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/floatingips/floatingip_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.627521 blazar-9.0.0.0rc1/blazar/plugins/instances/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/instances/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35478 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/instances/instance_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.627521 blazar-9.0.0.0rc1/blazar/plugins/oshosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/oshosts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39310 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/plugins/oshosts/host_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.627521 blazar-9.0.0.0rc1/blazar/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/policies/floatingips.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/policies/leases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3378 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/policies/oshosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3920 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12588 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.631521 blazar-9.0.0.0rc1/blazar/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2729 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.631521 blazar-9.0.0.0rc1/blazar/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10318 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/test_acl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4025 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1903 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/test_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6121 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/test_version_selector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.631521 blazar-9.0.0.0rc1/blazar/tests/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.631521 blazar-9.0.0.0rc1/blazar/tests/api/v1/leases/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/leases/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/leases/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8446 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/leases/test_v1_0.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.635522 blazar-9.0.0.0rc1/blazar/tests/api/v1/oshosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/oshosts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1582 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/oshosts/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11645 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/oshosts/test_v1_0.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4750 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/test_api_version_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3458 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/test_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5597 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v1/test_validation.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.635522 blazar-9.0.0.0rc1/blazar/tests/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15672 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v2/test_hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14101 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/api/v2/test_leases.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.635522 blazar-9.0.0.0rc1/blazar/tests/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.635522 blazar-9.0.0.0rc1/blazar/tests/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.635522 blazar-9.0.0.0rc1/blazar/tests/db/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24615 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/migration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/migration/test_migrations.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7059 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/migration/test_migrations.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.635522 blazar-9.0.0.0rc1/blazar/tests/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43757 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/sqlalchemy/test_sqlalchemy_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16946 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/sqlalchemy/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/db/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.635522 blazar-9.0.0.0rc1/blazar/tests/enforcement/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/enforcement/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.635522 blazar-9.0.0.0rc1/blazar/tests/enforcement/filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/enforcement/filters/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9732 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/enforcement/filters/test_max_lease_duration_filter.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10772 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/enforcement/test_enforcement.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/fake_lease.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1618 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/fake_requests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/local_hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/local_hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1427 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/local_hacking/test_hacking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1924 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/manager/test_rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    73427 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/manager/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/monitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/monitor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4256 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/monitor/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3500 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/monitor/test_notification_monitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/monitor/test_polling_monitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/notification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/notification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/notification/test_notifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/plugins/floatingips/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/plugins/floatingips/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39555 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/plugins/floatingips/test_floatingip_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/plugins/instances/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/plugins/instances/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71658 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/plugins/instances/test_instance_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/plugins/oshosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/plugins/oshosts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   111539 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/plugins/oshosts/test_physical_host_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4242 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2314 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2396 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16300 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.639522 blazar-9.0.0.0rc1/blazar/tests/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.643522 blazar-9.0.0.0rc1/blazar/tests/utils/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4383 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5049 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6174 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24815 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25831 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_placement.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3808 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/test_plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3862 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/tests/utils/test_trusts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.643522 blazar-9.0.0.0rc1/blazar/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1094 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.643522 blazar-9.0.0.0rc1/blazar/utils/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2763 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/openstack/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2335 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/openstack/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6525 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/openstack/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6437 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/openstack/neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22173 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/openstack/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17908 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/openstack/placement.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3662 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3179 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/utils/trusts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/blazar/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.607520 blazar-9.0.0.0rc1/blazar.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/blazar.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14782 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/blazar.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/blazar.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/blazar.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/blazar.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/blazar.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/blazar.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-03-08 12:17:58.000000 blazar-9.0.0.0rc1/blazar.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.647522 blazar-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8343 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.647522 blazar-9.0.0.0rc1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.599520 blazar-9.0.0.0rc1/doc/api_samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.647522 blazar-9.0.0.0rc1/doc/api_samples/floatingips/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/floatingips/floatingip-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/floatingips/floatingip-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/floatingips/floatingip-details-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/floatingips/floatingip-list-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.647522 blazar-9.0.0.0rc1/doc/api_samples/hosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      645 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/allocation-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/allocation-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-details-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-property-list-detail.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-property-list.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-property-update-res.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-property-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/hosts/host-update-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.651522 blazar-9.0.0.0rc1/doc/api_samples/leases/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/leases/lease-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/leases/lease-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/leases/lease-details-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3631 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/leases/lease-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/leases/lease-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/api_samples/leases/lease-update-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.651522 blazar-9.0.0.0rc1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.651522 blazar-9.0.0.0rc1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/admin/blazar-status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1507 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/admin/usage-enforcement.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.651522 blazar-9.0.0.0rc1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15744 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/cli/floatingip-reservation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13259 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/cli/host-reservation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9696 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/cli/instance-reservation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8242 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.655522 blazar-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/configuration/blazar-conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/configuration/blazar-policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      502 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/configuration/nova-conf.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.655522 blazar-9.0.0.0rc1/doc/source/configuration/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/configuration/samples/blazar-conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/configuration/samples/blazar-policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.655522 blazar-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/contributor/contribution.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/contributor/development.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/contributor/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.659522 blazar-9.0.0.0rc1/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18674 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/blazar-architecture-old.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18114 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/blazar-architecture.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17477 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/event_statuses.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/healing_flow.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55752 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/lease_statuses.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24998 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/reservation_statuses.png
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.659522 blazar-9.0.0.0rc1/doc/source/images/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/source/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/source/event_statuses.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/source/healing_flow.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/source/lease_statuses.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/images/source/reservation_statuses.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.659522 blazar-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/install/install-dashboard.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/install/install-using-devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3918 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/install/install-without-devstack.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.659522 blazar-9.0.0.0rc1/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/reference/api-microversion-history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.659522 blazar-9.0.0.0rc1/doc/source/restapi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/restapi/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.663523 blazar-9.0.0.0rc1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3300 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/user/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/user/compute-host-monitor.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5812 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/user/introduction.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4012 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/user/resource-monitoring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4138 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/doc/source/user/state-machines.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.599520 blazar-9.0.0.0rc1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.663523 blazar-9.0.0.0rc1/etc/blazar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/etc/blazar/README-blazar.conf.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/etc/blazar/blazar-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/etc/blazar/blazar-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2062 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/lower-constraints.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7473 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/pylintrc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.599520 blazar-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.671523 blazar-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/add-newly-allocated-hosts-to-aggregate-95bb75410afc6b8d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/alembic-fix-alter-column-42a87657992d1e78.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/api-microversioning-141e473bff34aad2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/before-end-actions-7e53e740e006195a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/blazar-status-upgrade-check-framework-895079486d8085f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/bug-1779660-b623de868955e7d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/bug-1786031-800a33c681fafdc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/bug-1786031-836c6d6acae08403.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/bug-1847821-2f9d6e61f438dc4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/bug-1880646-f1af8c48f895f00e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/bug-1881162-ebe012fcc7176594.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/bug-1957761-8b126a392c0c79ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/bug-1958307-63bf308ca6a97068.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/cleaning-time-825d148b704b0c56.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/create-extra-capabilities-in-update-host-c74ce75c88e88c67.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/delete-on-end-3a6d3ced93ffed25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/deprecate-climate-filter-f1ffca52a7a4e70c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/deprecate-json-formatted-policy-file-5ceba2a580b69101.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/devstack-dashboard-1b96128952e64c1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/drop-python2-support-148148077280122c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/floatingip-reservation-6c2f3c3ad8843948.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/floatingip-reservation-update-f53c0c6239ccf9ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/global_request_id-f30e900f20752c2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/host-allocation-dates-6da5ac1ec9befa8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/host-dashboard-570a9971be1a86ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/internal-endpoint-interface-748511b8b25455c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/issue-instance-reservation-7b3c0868caaabc85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/move-hosts-back-to-freepool-041fcda9fb3fc6c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/move-specs-cf3568febaaf3b1c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/multi-freepools-9d88b1f79c330a3c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/new-instance-reservation-1f3cbfe21146e251.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/no-affinity-instance-reservation-d356e33088772ea3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/periodic-healing-143ed251d990580b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/policy-in-code-3107271b0636fcea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/prevent-delete-during-events-c206a8f0a116798c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/python3-support-d9657c136cad2a41.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/region-in-placement-client-dfbd0bcd09f81aac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/remove-climate-fb62d72ca8fc5c7d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/remove-old-instance-reservation-60820d8afe00819e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/request_id-0ebc34f09c6d01f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/resource-allocation-api-f2fff51fc4556cd4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/resource-monitoring-622b6ebcb7472cf2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/resource-property-discovery-42df197a1a49bd76.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/response-code-fix-in-rocky-2197a9c1516a0ac4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/state-machine-37be751ed54c1c75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/update-reserved-capacity-9f079395959f4474.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/update-used-extra-capability-6d7bc7fa23c91295.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/upgrade-info-1a5b8bfbb323d525.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/notes/usage-enforcement-f997ce618f542104.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.675523 blazar-9.0.0.0rc1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.675523 blazar-9.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.675523 blazar-9.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8563 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1343 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2022-03-08 12:17:58.679523 blazar-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:17:58.675523 blazar-9.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2014 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3598 2022-03-08 12:17:26.000000 blazar-9.0.0.0rc1/tox.ini
```

### Comparing `blazar-9.0.0/.zuul.yaml` & `blazar-9.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/AUTHORS` & `blazar-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/CONTRIBUTING.rst` & `blazar-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/ChangeLog` & `blazar-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Preserve traceback on lease transition errors
 * Use configured endpoint type in url\_for
 * Add resource properties discovery API
 * Switch to using internal endpoints
 * Update Nova scheduler filter configuration
 * Delete preemptible instances on reservation start
```

### Comparing `blazar-9.0.0/LICENSE` & `blazar-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/PKG-INFO` & `blazar-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: blazar
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Reservation Service for OpenStack clouds
 Home-page: https://docs.openstack.org/blazar/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache Software License
 Description: Team and repository tags
         ========================
```

### Comparing `blazar-9.0.0/README.rst` & `blazar-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/api-ref/source/conf.py` & `blazar-9.0.0.0rc1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/api-ref/source/v1/floatingips.inc` & `blazar-9.0.0.0rc1/api-ref/source/v1/floatingips.inc`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/api-ref/source/v1/global-request-id.inc` & `blazar-9.0.0.0rc1/api-ref/source/v1/global-request-id.inc`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/api-ref/source/v1/hosts.inc` & `blazar-9.0.0.0rc1/api-ref/source/v1/hosts.inc`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/api-ref/source/v1/leases.inc` & `blazar-9.0.0.0rc1/api-ref/source/v1/leases.inc`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/api-ref/source/v1/parameters.yaml` & `blazar-9.0.0.0rc1/api-ref/source/v1/parameters.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/api-ref/source/v1/request-ids.inc` & `blazar-9.0.0.0rc1/api-ref/source/v1/request-ids.inc`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/app.py` & `blazar-9.0.0.0rc1/blazar/api/app.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/context.py` & `blazar-9.0.0.0rc1/blazar/api/context.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/root.py` & `blazar-9.0.0.0rc1/blazar/api/root.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/api_version_request.py` & `blazar-9.0.0.0rc1/blazar/api/v1/api_version_request.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/app.py` & `blazar-9.0.0.0rc1/blazar/api/v1/app.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/floatingips/service.py` & `blazar-9.0.0.0rc1/blazar/api/v1/floatingips/service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/floatingips/v1_0.py` & `blazar-9.0.0.0rc1/blazar/api/v1/floatingips/v1_0.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/leases/service.py` & `blazar-9.0.0.0rc1/blazar/api/v1/leases/service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/leases/v1_0.py` & `blazar-9.0.0.0rc1/blazar/api/v1/leases/v1_0.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/oshosts/service.py` & `blazar-9.0.0.0rc1/blazar/api/v1/oshosts/service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/oshosts/v1_0.py` & `blazar-9.0.0.0rc1/blazar/api/v1/oshosts/v1_0.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/request_id.py` & `blazar-9.0.0.0rc1/blazar/api/v1/request_id.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/request_log.py` & `blazar-9.0.0.0rc1/blazar/api/v1/request_log.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/rest_api_version_history.rst` & `blazar-9.0.0.0rc1/blazar/api/v1/rest_api_version_history.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/utils.py` & `blazar-9.0.0.0rc1/blazar/api/v1/utils.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v1/validation.py` & `blazar-9.0.0.0rc1/blazar/api/v1/validation.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/app.py` & `blazar-9.0.0.0rc1/blazar/api/v2/app.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/controllers/__init__.py` & `blazar-9.0.0.0rc1/blazar/api/v2/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/controllers/base.py` & `blazar-9.0.0.0rc1/blazar/api/v2/controllers/base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/controllers/extensions/__init__.py` & `blazar-9.0.0.0rc1/blazar/api/v2/controllers/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/controllers/extensions/host.py` & `blazar-9.0.0.0rc1/blazar/api/v2/controllers/extensions/host.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/controllers/extensions/lease.py` & `blazar-9.0.0.0rc1/blazar/api/v2/controllers/extensions/lease.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/controllers/types.py` & `blazar-9.0.0.0rc1/blazar/api/v2/controllers/types.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/hooks.py` & `blazar-9.0.0.0rc1/blazar/api/v2/hooks.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/v2/middleware/__init__.py` & `blazar-9.0.0.0rc1/blazar/api/v2/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/api/wsgi_app.py` & `blazar-9.0.0.0rc1/blazar/api/wsgi_app.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/cmd/api.py` & `blazar-9.0.0.0rc1/blazar/cmd/api.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/cmd/manager.py` & `blazar-9.0.0.0rc1/blazar/cmd/manager.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/cmd/status.py` & `blazar-9.0.0.0rc1/blazar/cmd/status.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/config.py` & `blazar-9.0.0.0rc1/blazar/config.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/context.py` & `blazar-9.0.0.0rc1/blazar/context.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/api.py` & `blazar-9.0.0.0rc1/blazar/db/api.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/base.py` & `blazar-9.0.0.0rc1/blazar/db/base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/exceptions.py` & `blazar-9.0.0.0rc1/blazar/db/exceptions.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/README` & `blazar-9.0.0.0rc1/blazar/db/migration/README`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic.ini` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/env.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/script.py.mako` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/02e2f2186d98_resource_property.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/02e2f2186d98_resource_property.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/0_1_initial.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/0_1_initial.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/10e34bba18e8_add_service_name_to_.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/10e34bba18e8_add_service_name_to_.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/1fd6c2eded89_add_trust_id_to_comp.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/1fd6c2eded89_add_trust_id_to_comp.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/23d6240b51b2_add_status_to_leases.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/23d6240b51b2_add_status_to_leases.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/2bcfe76b0474_change_tenant_to_project.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/2bcfe76b0474_change_tenant_to_project.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/35b314cd39ee_add_az_in_compute.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/35b314cd39ee_add_az_in_compute.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/6bfd1c23aa18_allow_duplicate_lease_names.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/6bfd1c23aa18_allow_duplicate_lease_names.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/75a74e4539cb_update_lease_status.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/75a74e4539cb_update_lease_status.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/7f1a7bbb2cd2_add_aggregate_id_field_into_the_.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/7f1a7bbb2cd2_add_aggregate_id_field_into_the_.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/8805be233864_instance_reservation_table.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/8805be233864_instance_reservation_table.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/9593f3656974_no_affinity_instance_reservation.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/9593f3656974_no_affinity_instance_reservation.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/97d2cad1504e_add_fields_for_resource_monitoring.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/97d2cad1504e_add_fields_for_resource_monitoring.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/ba75b766b64e_add_before_end_into_computehost.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/ba75b766b64e_add_before_end_into_computehost.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/c0ae6b08b0d7_resource_properties_in_instance_plugin.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/c0ae6b08b0d7_resource_properties_in_instance_plugin.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/e069c014356d_add_floatingip.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/e069c014356d_add_floatingip.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/e66f199a5414_delete_unused_status_related_fields.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/e66f199a5414_delete_unused_status_related_fields.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/alembic_migrations/versions/f4084140f608_add_floatingip_reservation.py` & `blazar-9.0.0.0rc1/blazar/db/migration/alembic_migrations/versions/f4084140f608_add_floatingip_reservation.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/migration/cli.py` & `blazar-9.0.0.0rc1/blazar/db/migration/cli.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/sqlalchemy/api.py` & `blazar-9.0.0.0rc1/blazar/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/sqlalchemy/facade_wrapper.py` & `blazar-9.0.0.0rc1/blazar/db/sqlalchemy/facade_wrapper.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/sqlalchemy/model_base.py` & `blazar-9.0.0.0rc1/blazar/db/sqlalchemy/model_base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/sqlalchemy/models.py` & `blazar-9.0.0.0rc1/blazar/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/sqlalchemy/types.py` & `blazar-9.0.0.0rc1/blazar/db/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/sqlalchemy/utils.py` & `blazar-9.0.0.0rc1/blazar/db/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/db/utils.py` & `blazar-9.0.0.0rc1/blazar/db/utils.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/enforcement/__init__.py` & `blazar-9.0.0.0rc1/blazar/enforcement/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/enforcement/enforcement.py` & `blazar-9.0.0.0rc1/blazar/enforcement/enforcement.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/enforcement/exceptions.py` & `blazar-9.0.0.0rc1/blazar/enforcement/exceptions.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/enforcement/filters/__init__.py` & `blazar-9.0.0.0rc1/blazar/enforcement/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/enforcement/filters/base_filter.py` & `blazar-9.0.0.0rc1/blazar/enforcement/filters/base_filter.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/enforcement/filters/max_lease_duration_filter.py` & `blazar-9.0.0.0rc1/blazar/enforcement/filters/max_lease_duration_filter.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/exceptions.py` & `blazar-9.0.0.0rc1/blazar/exceptions.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/hacking/checks.py` & `blazar-9.0.0.0rc1/blazar/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/i18n.py` & `blazar-9.0.0.0rc1/blazar/i18n.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/manager/__init__.py` & `blazar-9.0.0.0rc1/blazar/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/manager/exceptions.py` & `blazar-9.0.0.0rc1/blazar/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/manager/floatingips/rpcapi.py` & `blazar-9.0.0.0rc1/blazar/manager/floatingips/rpcapi.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/manager/leases/rpcapi.py` & `blazar-9.0.0.0rc1/blazar/manager/leases/rpcapi.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/manager/oshosts/rpcapi.py` & `blazar-9.0.0.0rc1/blazar/manager/oshosts/rpcapi.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/manager/service.py` & `blazar-9.0.0.0rc1/blazar/manager/service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/monitor/__init__.py` & `blazar-9.0.0.0rc1/blazar/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/monitor/base.py` & `blazar-9.0.0.0rc1/blazar/monitor/base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/monitor/notification_monitor.py` & `blazar-9.0.0.0rc1/blazar/monitor/notification_monitor.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/monitor/polling_monitor.py` & `blazar-9.0.0.0rc1/blazar/monitor/polling_monitor.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/notification/api.py` & `blazar-9.0.0.0rc1/blazar/notification/api.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/notification/notifier.py` & `blazar-9.0.0.0rc1/blazar/notification/notifier.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/opts.py` & `blazar-9.0.0.0rc1/blazar/opts.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/plugins/base.py` & `blazar-9.0.0.0rc1/blazar/plugins/base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/plugins/dummy_vm_plugin.py` & `blazar-9.0.0.0rc1/blazar/plugins/dummy_vm_plugin.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/plugins/floatingips/__init__.py` & `blazar-9.0.0.0rc1/blazar/plugins/floatingips/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/plugins/floatingips/floatingip_plugin.py` & `blazar-9.0.0.0rc1/blazar/plugins/floatingips/floatingip_plugin.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/plugins/instances/__init__.py` & `blazar-9.0.0.0rc1/blazar/plugins/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/plugins/instances/instance_plugin.py` & `blazar-9.0.0.0rc1/blazar/plugins/instances/instance_plugin.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/plugins/oshosts/__init__.py` & `blazar-9.0.0.0rc1/blazar/plugins/oshosts/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/plugins/oshosts/host_plugin.py` & `blazar-9.0.0.0rc1/blazar/plugins/oshosts/host_plugin.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/policies/__init__.py` & `blazar-9.0.0.0rc1/blazar/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/policies/base.py` & `blazar-9.0.0.0rc1/blazar/policies/base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/policies/floatingips.py` & `blazar-9.0.0.0rc1/blazar/policies/floatingips.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/policies/leases.py` & `blazar-9.0.0.0rc1/blazar/policies/leases.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/policies/oshosts.py` & `blazar-9.0.0.0rc1/blazar/policies/oshosts.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/policy.py` & `blazar-9.0.0.0rc1/blazar/policy.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/rpc.py` & `blazar-9.0.0.0rc1/blazar/rpc.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/status.py` & `blazar-9.0.0.0rc1/blazar/status.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/__init__.py` & `blazar-9.0.0.0rc1/blazar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/__init__.py` & `blazar-9.0.0.0rc1/blazar/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/test_acl.py` & `blazar-9.0.0.0rc1/blazar/tests/api/test_acl.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/test_context.py` & `blazar-9.0.0.0rc1/blazar/tests/api/test_context.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/test_root.py` & `blazar-9.0.0.0rc1/blazar/tests/api/test_root.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/test_version_selector.py` & `blazar-9.0.0.0rc1/blazar/tests/api/test_version_selector.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v1/leases/test_service.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v1/leases/test_service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v1/leases/test_v1_0.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v1/leases/test_v1_0.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v1/oshosts/test_service.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v1/oshosts/test_service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v1/oshosts/test_v1_0.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v1/oshosts/test_v1_0.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v1/test_api_version_request.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v1/test_api_version_request.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v1/test_app.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v1/test_app.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v1/test_utils.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v1/test_utils.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v1/test_validation.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v1/test_validation.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v2/test_hosts.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v2/test_hosts.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/api/v2/test_leases.py` & `blazar-9.0.0.0rc1/blazar/tests/api/v2/test_leases.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/cmd/test_status.py` & `blazar-9.0.0.0rc1/blazar/tests/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/db/migration/__init__.py` & `blazar-9.0.0.0rc1/blazar/tests/db/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/db/migration/test_migrations.conf` & `blazar-9.0.0.0rc1/blazar/tests/db/migration/test_migrations.conf`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/db/migration/test_migrations.py` & `blazar-9.0.0.0rc1/blazar/tests/db/migration/test_migrations.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/db/sqlalchemy/test_sqlalchemy_api.py` & `blazar-9.0.0.0rc1/blazar/tests/db/sqlalchemy/test_sqlalchemy_api.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/db/sqlalchemy/test_utils.py` & `blazar-9.0.0.0rc1/blazar/tests/db/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/db/test_api.py` & `blazar-9.0.0.0rc1/blazar/tests/db/test_api.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/db/test_utils.py` & `blazar-9.0.0.0rc1/blazar/tests/db/test_utils.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/enforcement/filters/test_max_lease_duration_filter.py` & `blazar-9.0.0.0rc1/blazar/tests/enforcement/filters/test_max_lease_duration_filter.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/enforcement/test_enforcement.py` & `blazar-9.0.0.0rc1/blazar/tests/enforcement/test_enforcement.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/fake_lease.py` & `blazar-9.0.0.0rc1/blazar/tests/fake_lease.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/fake_requests.py` & `blazar-9.0.0.0rc1/blazar/tests/fake_requests.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/local_hacking/test_hacking.py` & `blazar-9.0.0.0rc1/blazar/tests/local_hacking/test_hacking.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/manager/test_rpcapi.py` & `blazar-9.0.0.0rc1/blazar/tests/manager/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/manager/test_service.py` & `blazar-9.0.0.0rc1/blazar/tests/manager/test_service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/monitor/test_base.py` & `blazar-9.0.0.0rc1/blazar/tests/monitor/test_base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/monitor/test_notification_monitor.py` & `blazar-9.0.0.0rc1/blazar/tests/monitor/test_notification_monitor.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/monitor/test_polling_monitor.py` & `blazar-9.0.0.0rc1/blazar/tests/monitor/test_polling_monitor.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/notification/test_notifier.py` & `blazar-9.0.0.0rc1/blazar/tests/notification/test_notifier.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/plugins/floatingips/test_floatingip_plugin.py` & `blazar-9.0.0.0rc1/blazar/tests/plugins/floatingips/test_floatingip_plugin.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/plugins/instances/test_instance_plugin.py` & `blazar-9.0.0.0rc1/blazar/tests/plugins/instances/test_instance_plugin.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/plugins/oshosts/test_physical_host_plugin.py` & `blazar-9.0.0.0rc1/blazar/tests/plugins/oshosts/test_physical_host_plugin.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/test_context.py` & `blazar-9.0.0.0rc1/blazar/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/test_exceptions.py` & `blazar-9.0.0.0rc1/blazar/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/test_policy.py` & `blazar-9.0.0.0rc1/blazar/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/test_service.py` & `blazar-9.0.0.0rc1/blazar/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/test_status.py` & `blazar-9.0.0.0rc1/blazar/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/utils/openstack/test_base.py` & `blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/utils/openstack/test_keystone.py` & `blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_keystone.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/utils/openstack/test_neutron.py` & `blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_neutron.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/utils/openstack/test_nova.py` & `blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_nova.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/utils/openstack/test_placement.py` & `blazar-9.0.0.0rc1/blazar/tests/utils/openstack/test_placement.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/utils/test_plugins.py` & `blazar-9.0.0.0rc1/blazar/tests/utils/test_plugins.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/tests/utils/test_trusts.py` & `blazar-9.0.0.0rc1/blazar/tests/utils/test_trusts.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/__init__.py` & `blazar-9.0.0.0rc1/blazar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/openstack/base.py` & `blazar-9.0.0.0rc1/blazar/utils/openstack/base.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/openstack/exceptions.py` & `blazar-9.0.0.0rc1/blazar/utils/openstack/exceptions.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/openstack/keystone.py` & `blazar-9.0.0.0rc1/blazar/utils/openstack/keystone.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/openstack/neutron.py` & `blazar-9.0.0.0rc1/blazar/utils/openstack/neutron.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/openstack/nova.py` & `blazar-9.0.0.0rc1/blazar/utils/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/openstack/placement.py` & `blazar-9.0.0.0rc1/blazar/utils/openstack/placement.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/plugins.py` & `blazar-9.0.0.0rc1/blazar/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/service.py` & `blazar-9.0.0.0rc1/blazar/utils/service.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/utils/trusts.py` & `blazar-9.0.0.0rc1/blazar/utils/trusts.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar/version.py` & `blazar-9.0.0.0rc1/blazar/version.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar.egg-info/PKG-INFO` & `blazar-9.0.0.0rc1/blazar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: blazar
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Reservation Service for OpenStack clouds
 Home-page: https://docs.openstack.org/blazar/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache Software License
 Description: Team and repository tags
         ========================
```

### Comparing `blazar-9.0.0/blazar.egg-info/SOURCES.txt` & `blazar-9.0.0.0rc1/blazar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar.egg-info/entry_points.txt` & `blazar-9.0.0.0rc1/blazar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/blazar.egg-info/requires.txt` & `blazar-9.0.0.0rc1/blazar.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/devstack/plugin.sh` & `blazar-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/devstack/settings` & `blazar-9.0.0.0rc1/devstack/settings`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/floatingips/floatingip-list-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/floatingips/floatingip-list-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/hosts/allocation-get-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/hosts/allocation-get-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/hosts/allocation-list-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/hosts/allocation-list-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/hosts/host-create-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/hosts/host-create-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/hosts/host-details-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/hosts/host-details-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/hosts/host-list-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/hosts/host-list-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/hosts/host-update-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/hosts/host-update-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/leases/lease-create-req.json` & `blazar-9.0.0.0rc1/doc/api_samples/leases/lease-create-req.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/leases/lease-create-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/leases/lease-create-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/leases/lease-details-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/leases/lease-details-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/leases/lease-list-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/leases/lease-list-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/api_samples/leases/lease-update-resp.json` & `blazar-9.0.0.0rc1/doc/api_samples/leases/lease-update-resp.json`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/admin/blazar-status.rst` & `blazar-9.0.0.0rc1/doc/source/admin/blazar-status.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/admin/usage-enforcement.rst` & `blazar-9.0.0.0rc1/doc/source/admin/usage-enforcement.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/cli/floatingip-reservation.rst` & `blazar-9.0.0.0rc1/doc/source/cli/floatingip-reservation.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/cli/host-reservation.rst` & `blazar-9.0.0.0rc1/doc/source/cli/host-reservation.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/cli/instance-reservation.rst` & `blazar-9.0.0.0rc1/doc/source/cli/instance-reservation.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/conf.py` & `blazar-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/configuration/blazar-policy.rst` & `blazar-9.0.0.0rc1/doc/source/configuration/blazar-policy.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/configuration/index.rst` & `blazar-9.0.0.0rc1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/configuration/samples/blazar-policy.rst` & `blazar-9.0.0.0rc1/doc/source/configuration/samples/blazar-policy.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/contributor/contribution.rst` & `blazar-9.0.0.0rc1/doc/source/contributor/contribution.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/contributor/development.rst` & `blazar-9.0.0.0rc1/doc/source/contributor/development.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/blazar-architecture-old.png` & `blazar-9.0.0.0rc1/doc/source/images/blazar-architecture-old.png`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/blazar-architecture.png` & `blazar-9.0.0.0rc1/doc/source/images/blazar-architecture.png`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/event_statuses.png` & `blazar-9.0.0.0rc1/doc/source/images/event_statuses.png`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/healing_flow.png` & `blazar-9.0.0.0rc1/doc/source/images/healing_flow.png`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/lease_statuses.png` & `blazar-9.0.0.0rc1/doc/source/images/lease_statuses.png`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/reservation_statuses.png` & `blazar-9.0.0.0rc1/doc/source/images/reservation_statuses.png`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/source/event_statuses.xml` & `blazar-9.0.0.0rc1/doc/source/images/source/event_statuses.xml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/source/healing_flow.xml` & `blazar-9.0.0.0rc1/doc/source/images/source/healing_flow.xml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/source/lease_statuses.xml` & `blazar-9.0.0.0rc1/doc/source/images/source/lease_statuses.xml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/images/source/reservation_statuses.xml` & `blazar-9.0.0.0rc1/doc/source/images/source/reservation_statuses.xml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/index.rst` & `blazar-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/install/install-using-devstack.rst` & `blazar-9.0.0.0rc1/doc/source/install/install-using-devstack.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/install/install-without-devstack.rst` & `blazar-9.0.0.0rc1/doc/source/install/install-without-devstack.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/user/architecture.rst` & `blazar-9.0.0.0rc1/doc/source/user/architecture.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/user/compute-host-monitor.rst` & `blazar-9.0.0.0rc1/doc/source/user/compute-host-monitor.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/user/introduction.rst` & `blazar-9.0.0.0rc1/doc/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/user/resource-monitoring.rst` & `blazar-9.0.0.0rc1/doc/source/user/resource-monitoring.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/doc/source/user/state-machines.rst` & `blazar-9.0.0.0rc1/doc/source/user/state-machines.rst`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/lower-constraints.txt` & `blazar-9.0.0.0rc1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/pylintrc` & `blazar-9.0.0.0rc1/pylintrc`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/before-end-actions-7e53e740e006195a.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/before-end-actions-7e53e740e006195a.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/bug-1779660-b623de868955e7d9.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/bug-1779660-b623de868955e7d9.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/cleaning-time-825d148b704b0c56.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/cleaning-time-825d148b704b0c56.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/deprecate-json-formatted-policy-file-5ceba2a580b69101.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/deprecate-json-formatted-policy-file-5ceba2a580b69101.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/floatingip-reservation-6c2f3c3ad8843948.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/floatingip-reservation-6c2f3c3ad8843948.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/global_request_id-f30e900f20752c2b.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/global_request_id-f30e900f20752c2b.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/internal-endpoint-interface-748511b8b25455c6.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/internal-endpoint-interface-748511b8b25455c6.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/multi-freepools-9d88b1f79c330a3c.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/multi-freepools-9d88b1f79c330a3c.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/new-instance-reservation-1f3cbfe21146e251.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/new-instance-reservation-1f3cbfe21146e251.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/no-affinity-instance-reservation-d356e33088772ea3.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/no-affinity-instance-reservation-d356e33088772ea3.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/periodic-healing-143ed251d990580b.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/periodic-healing-143ed251d990580b.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/policy-in-code-3107271b0636fcea.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/policy-in-code-3107271b0636fcea.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/request_id-0ebc34f09c6d01f2.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/request_id-0ebc34f09c6d01f2.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/resource-allocation-api-f2fff51fc4556cd4.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/resource-allocation-api-f2fff51fc4556cd4.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/resource-monitoring-622b6ebcb7472cf2.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/resource-monitoring-622b6ebcb7472cf2.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/response-code-fix-in-rocky-2197a9c1516a0ac4.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/response-code-fix-in-rocky-2197a9c1516a0ac4.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/state-machine-37be751ed54c1c75.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/state-machine-37be751ed54c1c75.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/notes/upgrade-info-1a5b8bfbb323d525.yaml` & `blazar-9.0.0.0rc1/releasenotes/notes/upgrade-info-1a5b8bfbb323d525.yaml`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/releasenotes/source/conf.py` & `blazar-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/requirements.txt` & `blazar-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/setup.cfg` & `blazar-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/setup.py` & `blazar-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/tools/test-setup.sh` & `blazar-9.0.0.0rc1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `blazar-9.0.0/tox.ini` & `blazar-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

