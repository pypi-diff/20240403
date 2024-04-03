# Comparing `tmp/barbican-9.0.0.0rc1.tar.gz` & `tmp/barbican-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbican-9.0.0.0rc1.tar", last modified: Fri Sep 27 20:16:50 2019, max compression
+gzip compressed data, was "dist/barbican-9.0.1.tar", last modified: Mon Jun 15 09:16:27 2020, max compression
```

## Comparing `barbican-9.0.0.0rc1.tar` & `barbican-9.0.1.tar`

### file list

```diff
@@ -1,573 +1,573 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2366 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4573 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1770 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/hooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8182 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/secretstores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12677 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18075 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7791 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5759 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8452 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/consumers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6105 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/transportkeys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15746 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/acls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5086 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7558 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/secretmeta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7722 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/controllers/orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3570 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/app.wsgi
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4929 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/middleware/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2978 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/api/middleware/simple.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35490 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/locale/zh_CN/LC_MESSAGES/barbican.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50638 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/locale/en_GB/LC_MESSAGES/barbican.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/plugin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/plugin/crypto/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9697 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/crypto/simple_crypto.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15161 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/crypto/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6147 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/crypto/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/crypto/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28804 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/crypto/pkcs11.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16047 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/crypto/p11_crypto.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5799 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/castellan_secret_store.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/plugin/interface/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25822 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/interface/secret_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/interface/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29540 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/interface/certificate_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11294 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/symantec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7022 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/simple_certificate_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/dogtag_config_opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/plugin/util/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/util/mime_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2033 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/util/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13163 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/util/multiple_backends.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/util/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7216 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/util/translations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53436 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/dogtag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3282 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/vault_secret_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12854 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/store_crypto.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25323 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/kmip_secret_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17164 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/snakeoil_ca.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16830 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/plugin/resources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5109 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tasks/keystone_consumer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3059 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tasks/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22543 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tasks/certificate_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15973 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tasks/resources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7690 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/accept.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6756 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/hrefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15526 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37425 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/validators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1981 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/resources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/common/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2986 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/secretstores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3656 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2984 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3129 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/consumers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/transportkeys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3782 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/acls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2240 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2649 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/secretmeta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/policies/orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7688 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13546 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/common/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/model/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53334 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15096 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/clean.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    95102 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/repositories.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/model/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2877 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/transport_keys_init_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/script.py.mako
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/order_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1974 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/kek_init_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/secrets_init_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/projects_init_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/encrypted_init_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3064 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/container_init_ops.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/254495565185_removing_redundant_fields_from_order.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/kilo_release.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/30dba269cc64_update_order_retry_tasks_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/4ecde3a3a72a_add_cas_column_to_project_quotas_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/aa2cf96a1d5_add_orderretrytask.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/256da65e0c5f_change_keystone_id_for_external_id_in_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/2843d6469f25_add_sub_status_info_for_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1175 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1bc885808c76_add_project_id_to_secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1287 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/3c3b04040bfe_add_owning_project_and_creator_to_cas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/cd4106a1a0_add_cert_to_container_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/443d6f4a69ac_added_secret_type_column_to_secrets_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5770 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1a7cf79559e3_new_secret_and_container_acl_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1063 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/3041b53b95d7_remove_size_limits_on_meta_table_values.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/156cd9933643_add_project_column_to_consumer_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3154 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/795737bb3c3_change_tenants_to_projects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3286 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/39cf2e645cba_model_for_multiple_backend_support.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/10220ccbe7fa_remove_transport_keys_column_from_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/d2780d5aa510_change_url_length.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/39a96e67e990_add_missing_constraints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/46b98cde536_add_project_quotas_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/juno_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/6a4457517a3_rename_acl_creator_only_to_project_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5115 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/2d21598e7e70_added_ca_related_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1912 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/13d127569afa_create_secret_store_metadata_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/47b69e523451_made_plugin_names_in_kek_datum_non_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1bece815014f_remove_projectsecret_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/3d36a26b88af_add_order_barbican_metadata_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2340 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/161f8aceb687_fill_project_id_to_secrets_where_missing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1a0c2cdafb38_initial_version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/dce488646127_add_secret_user_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1e86c18af2dd_add_new_columns_type_meta_containerid.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4615 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1c0f328bfce0_fixing_composite_primary_keys_and_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/4070806f6972_add_orders_plugin_metadata_table_and_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/2ab3f5371bde_dsa_in_container_type_modelbase_to.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/model/sync.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6272 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/secret_acl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/secret_acl_user.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2600 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/project_secret_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2013 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/kekdatum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4142 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/project_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/transport_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/container_secret.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7646 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/order_barbican_metadatum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1664 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/secret_stores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6875 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/container_acl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/secret_store_metadatum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3518 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3823 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/secret.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1797 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/secret_user_metadatum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1804 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/container_acl_user.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3916 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/order.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1303 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/order_plugin_metadatum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/order_retry_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5665 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/container_consumer_meta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1670 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/encrypted_datum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6013 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/objects/container.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/worker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7322 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/db_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/retry_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2558 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/keystone_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18097 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/barbican_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7129 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/pkcs11_kek_rewrap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/cmd/functionaltests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/functionaltests/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/functionaltests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11317 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/functionaltests/test_db_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5518 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/pkcs11_key_generation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5788 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/cmd/pkcs11_migrate_kek_signatures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/test_middleware_auth.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11734 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/test_transport_keys_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56223 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/test_resources_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3482 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/test_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44803 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/test_resources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13543 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_secretmeta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13020 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_secretstores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32161 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9999 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5830 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12733 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_consumers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45383 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_acls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28787 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_secrets.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/middleware/test_simple.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2176 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/api/middleware/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25715 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/certificate_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3989 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16752 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/test_crypto.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15215 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/test_p11_crypto.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16097 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/test_pkcs11.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18033 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/test_snakeoil_ca.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/interface/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12155 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/interface/test_secret_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11667 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/interface/test_certificate_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/interface/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3313 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/test_simple_certificate_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/util/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2111 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/util/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26288 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/util/test_multiple_backends.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/util/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9048 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/util/test_mime_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13546 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/util/test_translations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36132 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/test_dogtag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3432 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/test_symantec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29361 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/test_store_crypto.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36052 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/test_kmip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8713 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/test_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7804 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/plugin/test_castellan_secret_store.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/tasks/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42327 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/tasks/test_certificate_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19788 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/tasks/test_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13594 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/tasks/test_keystone_consumer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7601 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/common/test_hrefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70387 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/common/test_validators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12097 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/common/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10149 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/database_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/model/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33798 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/test_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10899 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3761 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1468 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_transport_keys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4449 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_secret_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_order_retry_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_projects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12652 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11453 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18390 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_certificate_authorities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18637 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_secret_stores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6845 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_consumers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23006 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_acls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3925 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9806 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/test_hacking.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/objects/test_ovo_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1130 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/objects/test_ovo_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10408 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/objects/test_ovo_project_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/objects/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10578 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/cmd/test_barbican_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/cmd/test-status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/cmd/test_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18821 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/cmd/test_db_cleanup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/cmd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/tests/queue/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14930 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/queue/test_keystone_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/queue/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/queue/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15770 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/queue/test_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7734 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/queue/test_retry_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21151 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/tests/keys.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9898 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican/queue/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9386 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/queue/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5906 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/queue/retry_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3289 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/queue/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3818 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/queue/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6829 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/queue/keystone_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/barbican/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4743 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2878 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1586 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/apiary.apib
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5828 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11367 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/LICENSE
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/api/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24294 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/acls.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22569 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/secrets.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17878 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/store_backends.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15979 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/containers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14310 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/orders.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11465 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/consumers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20424 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12312 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/secret_metadata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8656 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/reference/secret_types.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/api/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/sample_config.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1791 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/cli/barbican-status.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2231 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/common_prerequisites.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/common_configure.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1491 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4169 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/verify.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/get_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14364 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/barbican-backend.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/install/install-obs.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3731 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3523 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/devstack.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/contributor/plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4718 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/plugin/crypto.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6027 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/plugin/secret_store.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3002 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/plugin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3803 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/dataflow.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2891 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/getting_involved.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/dependencies.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3494 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/dev.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/structure.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5074 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13678 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/contributor/database_migrations.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3148 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/configuration/keystone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13254 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/configuration/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4144 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/configuration/plugin_backends.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1751 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/configuration/noauth.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/configuration/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5149 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/configuration/audit.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/configuration/config.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/_extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2194 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/_extra/.htaccess
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/admin/upgrade.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2957 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/admin/database_cleaning.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/admin/barbican_manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3261 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/admin/access_control.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25297 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/images/barbican-overall-architecture.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55633 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/images/barbican-components.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3163 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/doc/source/sample_policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-tempest-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-tempest-base/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-tempest-base/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/playbooks/legacy/grenade-devstack-barbican/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/grenade-devstack-barbican/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2262 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/grenade-devstack-barbican/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-functional-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-functional-base/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1089 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-functional-base/dogtag-post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-functional-base/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-base/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2321 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-base/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/devstack/barbican-vagrant/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/barbican-vagrant/Vagrantfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/barbican-vagrant/install_devstack.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/devstack/upgrade/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/upgrade/settings
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2614 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/upgrade/resources.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2462 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/upgrade/upgrade.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1377 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/upgrade/shutdown.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20039 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/lib/barbican
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      629 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/gate_hook.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3080 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/devstack/local.conf.example
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5267 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/.coveragerc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20741 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/barbican.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    88076 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/ChangeLog
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/etc/barbican/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/barbican/README.barbican.conf.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/barbican/barbican-api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/barbican/api_audit_map.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/etc/barbican/vassals/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/barbican/vassals/barbican-api.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2805 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/barbican/barbican-functional.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/etc/init/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/init/barbican.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/init/barbican-keystone-listener.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/init/barbican-worker.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/oslo-config-generator/barbican.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/oslo-config-generator/policy.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/etc/logrotate.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/etc/logrotate.d/barbican-api
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7311 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/bin/demo_requests.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3092 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/bin/barbican.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      374 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/bin/barbican-api
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2996 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/bin/versionbuild.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6342 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/bin/keystone_data.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/port-ruledefaults-to-documentedruledefaults-954fe88af9fe72ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/use_oslo_config_generator-f2a9be9e71d90b1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/remove_pkix-b045e7dde7e47356.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/http_proxy_to_wsgi-middleware-98dc4fe03eb362d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/oslopolicy-genscripts-1a7b364b8ffd7c3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/multiple-backends-75f5b85c63b930b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/barbican-status-upgrade-check-framework-9df56289b1d91ba4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/add-configurable-mechanism-options-2e5c57099b4c91b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/allow-aes-xts-512-bitlength-in-simple-crypto-95936a2d830035cc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/renamed-generate-iv-option-29770cfcff8e3b83.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1950 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/removing-cas-certificate-orders-96fc47a7acaea273.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/pkcs11-backend-performance-f3caacbe9e1ab535.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/fix-story-2004833-2b420688a82c3328.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/metadata-api-e95d4559e7bf9ca9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/remap-policy-to-match-controller-1673ec7c88235227.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/change_default_control_exchange-c47abc3e3f08aa31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/fix-story-2004734-977dbeda6b547f85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/fixed-invalid-route-response-code-15a681d07222a4f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/barbican-manage-d469b4d15454f981.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/notes/add-barbican-manage-check-subcommands-38835078f5cc0ce2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/rocky.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4400 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17505 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9096 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/releasenotes/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/api-guide/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/api-guide/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11391 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/acls.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5478 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/secrets.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10599 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/containers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6177 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/orders.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4893 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/consumers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7462 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4710 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/secret_metadata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2648 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/pkcs11keygeneration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6766 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/dogtag_setup.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9320 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/api-guide/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10422 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3931 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/functionaltests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/functionaltests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16773 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9187 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6783 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1909 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8919 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_consumers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8375 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_secrets.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3011 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/base_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/consumer_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/quota_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/acl_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1403 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/ca_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1664 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/secret_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/order_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/models/container_models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4218 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/acl_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/secretstores_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4859 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/consumer_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6223 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/container_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9891 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/secret_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5698 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/quota_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/base_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7178 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/order_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5053 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/secretmeta_behaviors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7753 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7819 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_secretmeta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13953 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_acls_rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_secretstores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9442 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_quotas_enforce.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20952 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29220 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15131 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_consumers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7206 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_quotas_rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21924 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_acls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25285 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_rsa.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64681 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8135 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_orders_rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12494 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_secrets_rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9901 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_containers_rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/.testr.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      977 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/post_test_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1356 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/run_tests.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:50.000000 barbican-9.0.0.0rc1/functionaltests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4967 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12279 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/common/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/common/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2019-09-27 20:16:10.000000 barbican-9.0.0.0rc1/functionaltests/run_tests_parallel.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20741 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2020-06-15 09:15:15.000000 barbican-9.0.1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5239 2020-06-15 09:15:15.000000 barbican-9.0.1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2020-06-15 09:15:15.000000 barbican-9.0.1/bindep.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    88254 2020-06-15 09:16:27.000000 barbican-9.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2020-06-15 09:15:15.000000 barbican-9.0.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11367 2020-06-15 09:15:15.000000 barbican-9.0.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-06-15 09:15:15.000000 barbican-9.0.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2020-06-15 09:16:27.000000 barbican-9.0.1/PKG-INFO
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2996 2020-06-15 09:15:15.000000 barbican-9.0.1/bin/versionbuild.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6342 2020-06-15 09:15:15.000000 barbican-9.0.1/bin/keystone_data.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7311 2020-06-15 09:15:15.000000 barbican-9.0.1/bin/demo_requests.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3092 2020-06-15 09:15:15.000000 barbican-9.0.1/bin/barbican.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      374 2020-06-15 09:15:15.000000 barbican-9.0.1/bin/barbican-api
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2020-06-15 09:15:15.000000 barbican-9.0.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2020-06-15 09:15:15.000000 barbican-9.0.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2878 2020-06-15 09:15:15.000000 barbican-9.0.1/HACKING.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3494 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/dev.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/contributor/plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3002 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/plugin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6027 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/plugin/secret_store.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4718 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/plugin/crypto.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3731 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5074 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13678 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/database_migrations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/dependencies.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3803 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/dataflow.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/structure.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2891 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/getting_involved.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3523 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/contributor/devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/sample_policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/sample_config.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1491 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2231 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/common_prerequisites.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4169 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/verify.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/get_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14364 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/barbican-backend.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/common_configure.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/install-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/_extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2194 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/_extra/.htaccess
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13254 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/configuration/troubleshooting.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5149 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/configuration/audit.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/configuration/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1751 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/configuration/noauth.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/configuration/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4144 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/configuration/plugin_backends.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3148 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/configuration/keystone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3163 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25297 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/images/barbican-overall-architecture.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55633 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/images/barbican-components.gif
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/admin/barbican_manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3261 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/admin/access_control.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2957 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/admin/database_cleaning.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/admin/upgrade.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1791 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/cli/barbican-status.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/doc/source/api/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22569 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/secrets.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15979 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/containers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11465 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/consumers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20424 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24294 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/acls.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17878 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/store_backends.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8656 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/secret_types.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12312 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/secret_metadata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14310 2020-06-15 09:15:15.000000 barbican-9.0.1/doc/source/api/reference/orders.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/functionaltests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/run_tests_parallel.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1356 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/.testr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/functionaltests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/common/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12279 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/common/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4967 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/functionaltests/api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/functionaltests/api/v1/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/functionaltests/api/v1/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1664 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/secret_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/quota_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/order_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/consumer_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/container_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/acl_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3011 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/base_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1403 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/models/ca_models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/functionaltests/api/v1/smoke/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8919 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/smoke/test_consumers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9187 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/smoke/test_containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1909 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/smoke/test_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8375 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/smoke/test_secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/smoke/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6783 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/smoke/test_orders.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/functionaltests/api/v1/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21924 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_acls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_secretstores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7819 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_secretmeta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9442 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_quotas_enforce.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9901 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_containers_rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13953 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_acls_rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7206 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_quotas_rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15131 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_consumers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25285 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_rsa.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12494 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_secrets_rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20952 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8135 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_orders_rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64681 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7753 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29220 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/functional/test_orders.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/base_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7178 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/order_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/secretstores_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6223 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/container_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4218 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/acl_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4859 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/consumer_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5698 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/quota_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5053 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/secretmeta_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9891 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/behaviors/secret_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16773 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/api/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      977 2020-06-15 09:15:15.000000 barbican-9.0.1/functionaltests/post_test_hook.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3931 2020-06-15 09:16:27.000000 barbican-9.0.1/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/etc/logrotate.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/logrotate.d/barbican-api
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/etc/barbican/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/barbican/api_audit_map.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2805 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/barbican/barbican-functional.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/barbican/barbican-api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/barbican/README.barbican.conf.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/etc/barbican/vassals/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/barbican/vassals/barbican-api.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/etc/init/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/init/barbican.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/init/barbican-worker.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/init/barbican-keystone-listener.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/oslo-config-generator/barbican.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2020-06-15 09:15:15.000000 barbican-9.0.1/etc/oslo-config-generator/policy.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2020-06-15 09:15:15.000000 barbican-9.0.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10458 2020-06-15 09:16:27.000000 barbican-9.0.1/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/model/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/sync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    95102 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/repositories.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/model/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2877 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/commands.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3064 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/container_init_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/order_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1974 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/kek_init_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/README
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/2ab3f5371bde_dsa_in_container_type_modelbase_to.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3286 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/39cf2e645cba_model_for_multiple_backend_support.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/4070806f6972_add_orders_plugin_metadata_table_and_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1287 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/3c3b04040bfe_add_owning_project_and_creator_to_cas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4615 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1c0f328bfce0_fixing_composite_primary_keys_and_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1e86c18af2dd_add_new_columns_type_meta_containerid.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/39a96e67e990_add_missing_constraints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/256da65e0c5f_change_keystone_id_for_external_id_in_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1175 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1bc885808c76_add_project_id_to_secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/cd4106a1a0_add_cert_to_container_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/443d6f4a69ac_added_secret_type_column_to_secrets_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/6a4457517a3_rename_acl_creator_only_to_project_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1bece815014f_remove_projectsecret_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1063 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/3041b53b95d7_remove_size_limits_on_meta_table_values.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1912 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/13d127569afa_create_secret_store_metadata_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3154 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/795737bb3c3_change_tenants_to_projects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1a0c2cdafb38_initial_version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/3d36a26b88af_add_order_barbican_metadata_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2340 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/161f8aceb687_fill_project_id_to_secrets_where_missing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/4ecde3a3a72a_add_cas_column_to_project_quotas_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/10220ccbe7fa_remove_transport_keys_column_from_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/30dba269cc64_update_order_retry_tasks_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/kilo_release.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5770 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1a7cf79559e3_new_secret_and_container_acl_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/46b98cde536_add_project_quotas_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/156cd9933643_add_project_column_to_consumer_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/dce488646127_add_secret_user_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5115 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/2d21598e7e70_added_ca_related_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/aa2cf96a1d5_add_orderretrytask.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/254495565185_removing_redundant_fields_from_order.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/2843d6469f25_add_sub_status_info_for_orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/juno_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/d2780d5aa510_change_url_length.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/47b69e523451_made_plugin_names_in_kek_datum_non_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/encrypted_init_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/transport_keys_init_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/secrets_init_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/alembic_migrations/projects_init_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/migration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53334 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15096 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/clean.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/model/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9898 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/hacking/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/retry_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7129 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/pkcs11_kek_rewrap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7322 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/db_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/worker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5788 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/pkcs11_migrate_kek_signatures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/cmd/functionaltests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11317 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/functionaltests/test_db_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/functionaltests/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/functionaltests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2558 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/keystone_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18097 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/barbican_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5518 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/pkcs11_key_generation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/cmd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/dogtag_config_opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/plugin/crypto/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28804 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/crypto/pkcs11.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16047 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/crypto/p11_crypto.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9697 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/crypto/simple_crypto.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15161 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/crypto/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/crypto/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6147 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/crypto/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16830 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7022 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/simple_certificate_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3282 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/vault_secret_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17164 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/snakeoil_ca.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/plugin/interface/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29540 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/interface/certificate_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25822 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/interface/secret_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/interface/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25323 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/kmip_secret_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12854 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/store_crypto.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5799 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/castellan_secret_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53436 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/dogtag.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/plugin/util/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2033 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/util/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/util/mime_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7216 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/util/translations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13163 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/util/multiple_backends.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/util/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11294 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/plugin/symantec.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9806 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/test_hacking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/model/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33798 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/test_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/model/repositories/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_projects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18390 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_certificate_authorities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23006 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_acls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11453 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_order_retry_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1468 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_transport_keys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12652 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3925 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4449 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_secret_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10899 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18637 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_secret_stores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6845 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_consumers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3761 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/model/repositories/test_repositories_containers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18821 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/cmd/test_db_cleanup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/cmd/test-status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/cmd/test_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10578 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/cmd/test_barbican_manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/plugin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/plugin/crypto/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16752 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/crypto/test_crypto.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3989 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/crypto/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16097 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/crypto/test_pkcs11.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15215 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/crypto/test_p11_crypto.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/crypto/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8713 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/test_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36132 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/test_dogtag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18033 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/test_snakeoil_ca.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29361 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/test_store_crypto.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/plugin/interface/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12155 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/interface/test_secret_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/interface/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11667 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/interface/test_certificate_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3313 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/test_simple_certificate_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/plugin/util/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9048 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/util/test_mime_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13546 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/util/test_translations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26288 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/util/test_multiple_backends.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2111 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/util/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/util/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36052 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/test_kmip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7804 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/test_castellan_secret_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3432 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/plugin/test_symantec.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/test_middleware_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25715 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10149 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/database_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21151 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/keys.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/common/test_hrefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7601 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12097 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/common/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70387 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/common/test_validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/queue/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15770 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/queue/test_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14930 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/queue/test_keystone_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/queue/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/queue/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7734 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/queue/test_retry_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1130 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/objects/test_ovo_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/objects/test_ovo_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10408 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/objects/test_ovo_project_quotas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/tasks/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13594 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/tasks/test_keystone_consumer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42327 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/tasks/test_certificate_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/tasks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19788 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/tasks/test_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/certificate_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56223 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/test_resources_policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2176 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/middleware/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/middleware/test_simple.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11734 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/test_transport_keys_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3482 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/test_init.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tests/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45383 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_acls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13020 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_secretstores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13543 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_secretmeta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12733 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_consumers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32161 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5830 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28787 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9999 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/controllers/test_orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44803 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tests/api/test_resources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7688 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1981 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37425 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7690 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15526 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6756 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/hrefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13546 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/common/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2240 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2984 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2649 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/secretmeta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2986 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/secretstores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/transportkeys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3782 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/acls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3656 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3129 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/consumers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policies/containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/accept.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/queue/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5906 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/queue/retry_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3289 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/queue/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9386 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/queue/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6829 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/queue/keystone_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3818 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/queue/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35490 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/locale/zh_CN/LC_MESSAGES/barbican.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50638 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/locale/en_GB/LC_MESSAGES/barbican.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1670 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/encrypted_datum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/transport_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/container_secret.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3916 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/order.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4142 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/project_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6013 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1804 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/container_acl_user.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1664 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/secret_stores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6272 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/secret_acl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2013 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/kekdatum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3823 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/secret.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6875 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/container_acl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/order_barbican_metadatum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5665 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/container_consumer_meta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3518 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/order_retry_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2600 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/project_secret_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1797 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/secret_user_metadatum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/secret_store_metadatum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1303 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/order_plugin_metadatum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7646 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/objects/secret_acl_user.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5109 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tasks/keystone_consumer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15973 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tasks/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22543 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tasks/certificate_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3059 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tasks/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/tasks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4929 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/middleware/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/middleware/simple.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2978 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3570 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/app.wsgi
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1770 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/hooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/barbican/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5086 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18075 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7558 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/secretmeta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8182 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/secretstores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6105 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/transportkeys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15746 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/acls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5759 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7791 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7722 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8452 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/consumers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12677 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/controllers/containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4573 2020-06-15 09:15:15.000000 barbican-9.0.1/barbican/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/oslopolicy-genscripts-1a7b364b8ffd7c3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/http_proxy_to_wsgi-middleware-98dc4fe03eb362d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/barbican-manage-d469b4d15454f981.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/pkcs11-backend-performance-f3caacbe9e1ab535.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1950 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/removing-cas-certificate-orders-96fc47a7acaea273.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/barbican-status-upgrade-check-framework-9df56289b1d91ba4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/fixed-invalid-route-response-code-15a681d07222a4f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/add-configurable-mechanism-options-2e5c57099b4c91b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/remove_pkix-b045e7dde7e47356.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/add-barbican-manage-check-subcommands-38835078f5cc0ce2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/multiple-backends-75f5b85c63b930b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/fix-story-2004734-977dbeda6b547f85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/change_default_control_exchange-c47abc3e3f08aa31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/use_oslo_config_generator-f2a9be9e71d90b1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/metadata-api-e95d4559e7bf9ca9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/allow-aes-xts-512-bitlength-in-simple-crypto-95936a2d830035cc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/renamed-generate-iv-option-29770cfcff8e3b83.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/fix-story-2004833-2b420688a82c3328.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/port-ruledefaults-to-documentedruledefaults-954fe88af9fe72ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/notes/remap-policy-to-match-controller-1673ec7c88235227.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/ocata.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4400 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17505 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9096 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/liberty.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-06-15 09:15:15.000000 barbican-9.0.1/releasenotes/source/pike.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/settings
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3047 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/local.conf.example
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20088 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/lib/barbican
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      629 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/gate_hook.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/devstack/upgrade/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2614 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/upgrade/resources.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2462 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/upgrade/upgrade.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/upgrade/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1377 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/upgrade/shutdown.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/devstack/barbican-vagrant/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/barbican-vagrant/Vagrantfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2020-06-15 09:15:15.000000 barbican-9.0.1/devstack/barbican-vagrant/install_devstack.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/playbooks/legacy/grenade-devstack-barbican/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/grenade-devstack-barbican/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2262 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/grenade-devstack-barbican/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-base/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2321 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-base/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-tempest-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-tempest-base/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-tempest-base/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-functional-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-functional-base/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1089 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-functional-base/dogtag-post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2020-06-15 09:15:15.000000 barbican-9.0.1/playbooks/legacy/barbican-devstack-functional-base/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1586 2020-06-15 09:15:15.000000 barbican-9.0.1/apiary.apib
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2366 2020-06-15 09:15:15.000000 barbican-9.0.1/lower-constraints.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5698 2020-06-15 09:15:15.000000 barbican-9.0.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2020-06-15 09:15:15.000000 barbican-9.0.1/.mailmap
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/api-guide/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:16:27.000000 barbican-9.0.1/api-guide/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5478 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/secrets.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10599 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/containers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4893 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/consumers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7462 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6766 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/dogtag_setup.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11391 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/acls.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9320 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2648 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/pkcs11keygeneration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4710 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/secret_metadata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6177 2020-06-15 09:15:15.000000 barbican-9.0.1/api-guide/source/orders.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4743 2020-06-15 09:15:15.000000 barbican-9.0.1/README.rst
```

### Comparing `barbican-9.0.0.0rc1/PKG-INFO` & `barbican-9.0.1/barbican.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barbican
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: OpenStack Secure Key Management
 Home-page: https://docs.openstack.org/barbican/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Service for storing sensitive client information for OpenStack
 Platform: UNKNOWN
```

### Comparing `barbican-9.0.0.0rc1/lower-constraints.txt` & `barbican-9.0.1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/test-requirements.txt` & `barbican-9.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/__init__.py` & `barbican-9.0.1/barbican/api/__init__.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/hooks.py` & `barbican-9.0.1/barbican/api/hooks.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/secretstores.py` & `barbican-9.0.1/barbican/api/controllers/secretstores.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/containers.py` & `barbican-9.0.1/barbican/api/controllers/containers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/secrets.py` & `barbican-9.0.1/barbican/api/controllers/secrets.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/__init__.py` & `barbican-9.0.1/barbican/api/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/versions.py` & `barbican-9.0.1/barbican/api/controllers/versions.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/consumers.py` & `barbican-9.0.1/barbican/api/controllers/consumers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/transportkeys.py` & `barbican-9.0.1/barbican/api/controllers/transportkeys.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/acls.py` & `barbican-9.0.1/barbican/api/controllers/acls.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/quotas.py` & `barbican-9.0.1/barbican/api/controllers/quotas.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/secretmeta.py` & `barbican-9.0.1/barbican/api/controllers/secretmeta.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/controllers/orders.py` & `barbican-9.0.1/barbican/api/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/app.py` & `barbican-9.0.1/barbican/api/app.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/app.wsgi` & `barbican-9.0.1/barbican/api/app.wsgi`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/middleware/context.py` & `barbican-9.0.1/barbican/api/middleware/context.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/middleware/__init__.py` & `barbican-9.0.1/barbican/api/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/api/middleware/simple.py` & `barbican-9.0.1/barbican/api/middleware/simple.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/version.py` & `barbican-9.0.1/barbican/version.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/locale/zh_CN/LC_MESSAGES/barbican.po` & `barbican-9.0.1/barbican/locale/zh_CN/LC_MESSAGES/barbican.po`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/locale/en_GB/LC_MESSAGES/barbican.po` & `barbican-9.0.1/barbican/locale/en_GB/LC_MESSAGES/barbican.po`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/crypto/simple_crypto.py` & `barbican-9.0.1/barbican/plugin/crypto/simple_crypto.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/crypto/base.py` & `barbican-9.0.1/barbican/plugin/crypto/base.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/crypto/manager.py` & `barbican-9.0.1/barbican/plugin/crypto/manager.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/crypto/pkcs11.py` & `barbican-9.0.1/barbican/plugin/crypto/pkcs11.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/crypto/p11_crypto.py` & `barbican-9.0.1/barbican/plugin/crypto/p11_crypto.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/castellan_secret_store.py` & `barbican-9.0.1/barbican/plugin/castellan_secret_store.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/interface/secret_store.py` & `barbican-9.0.1/barbican/plugin/interface/secret_store.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/interface/certificate_manager.py` & `barbican-9.0.1/barbican/plugin/interface/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/symantec.py` & `barbican-9.0.1/barbican/plugin/symantec.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/simple_certificate_manager.py` & `barbican-9.0.1/barbican/plugin/simple_certificate_manager.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/dogtag_config_opts.py` & `barbican-9.0.1/barbican/plugin/dogtag_config_opts.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/util/mime_types.py` & `barbican-9.0.1/barbican/plugin/util/mime_types.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/util/utils.py` & `barbican-9.0.1/barbican/plugin/util/utils.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/util/multiple_backends.py` & `barbican-9.0.1/barbican/plugin/util/multiple_backends.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/util/translations.py` & `barbican-9.0.1/barbican/plugin/util/translations.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/dogtag.py` & `barbican-9.0.1/barbican/plugin/dogtag.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/vault_secret_store.py` & `barbican-9.0.1/barbican/plugin/vault_secret_store.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/store_crypto.py` & `barbican-9.0.1/barbican/plugin/store_crypto.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/kmip_secret_store.py` & `barbican-9.0.1/barbican/plugin/kmip_secret_store.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/snakeoil_ca.py` & `barbican-9.0.1/barbican/plugin/snakeoil_ca.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/plugin/resources.py` & `barbican-9.0.1/barbican/plugin/resources.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tasks/keystone_consumer.py` & `barbican-9.0.1/barbican/tasks/keystone_consumer.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tasks/common.py` & `barbican-9.0.1/barbican/tasks/common.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tasks/certificate_resources.py` & `barbican-9.0.1/barbican/tasks/certificate_resources.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tasks/resources.py` & `barbican-9.0.1/barbican/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/utils.py` & `barbican-9.0.1/barbican/common/utils.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/accept.py` & `barbican-9.0.1/barbican/common/accept.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/hrefs.py` & `barbican-9.0.1/barbican/common/hrefs.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policy.py` & `barbican-9.0.1/barbican/common/policy.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/config.py` & `barbican-9.0.1/barbican/common/config.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/validators.py` & `barbican-9.0.1/barbican/common/validators.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/resources.py` & `barbican-9.0.1/barbican/common/resources.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/secretstores.py` & `barbican-9.0.1/barbican/common/policies/secretstores.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/base.py` & `barbican-9.0.1/barbican/common/policies/base.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/containers.py` & `barbican-9.0.1/barbican/common/policies/containers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/secrets.py` & `barbican-9.0.1/barbican/common/policies/secrets.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/__init__.py` & `barbican-9.0.1/barbican/common/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/consumers.py` & `barbican-9.0.1/barbican/common/policies/consumers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/transportkeys.py` & `barbican-9.0.1/barbican/common/policies/transportkeys.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/acls.py` & `barbican-9.0.1/barbican/common/policies/acls.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/quotas.py` & `barbican-9.0.1/barbican/common/policies/quotas.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/secretmeta.py` & `barbican-9.0.1/barbican/common/policies/secretmeta.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/policies/orders.py` & `barbican-9.0.1/barbican/common/policies/orders.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/quota.py` & `barbican-9.0.1/barbican/common/quota.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/common/exception.py` & `barbican-9.0.1/barbican/common/exception.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/context.py` & `barbican-9.0.1/barbican/context.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/models.py` & `barbican-9.0.1/barbican/model/models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/clean.py` & `barbican-9.0.1/barbican/model/clean.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/repositories.py` & `barbican-9.0.1/barbican/model/repositories.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic.ini` & `barbican-9.0.1/barbican/model/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/commands.py` & `barbican-9.0.1/barbican/model/migration/commands.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/transport_keys_init_ops.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/transport_keys_init_ops.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/env.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/script.py.mako` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/order_ops.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/order_ops.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/kek_init_ops.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/kek_init_ops.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/secrets_init_ops.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/secrets_init_ops.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/projects_init_ops.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/projects_init_ops.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/encrypted_init_ops.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/encrypted_init_ops.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/container_init_ops.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/container_init_ops.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/254495565185_removing_redundant_fields_from_order.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/254495565185_removing_redundant_fields_from_order.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/kilo_release.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/kilo_release.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/30dba269cc64_update_order_retry_tasks_table.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/30dba269cc64_update_order_retry_tasks_table.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/4ecde3a3a72a_add_cas_column_to_project_quotas_table.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/4ecde3a3a72a_add_cas_column_to_project_quotas_table.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/aa2cf96a1d5_add_orderretrytask.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/aa2cf96a1d5_add_orderretrytask.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/256da65e0c5f_change_keystone_id_for_external_id_in_.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/256da65e0c5f_change_keystone_id_for_external_id_in_.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/2843d6469f25_add_sub_status_info_for_orders.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/2843d6469f25_add_sub_status_info_for_orders.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1bc885808c76_add_project_id_to_secrets.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1bc885808c76_add_project_id_to_secrets.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/3c3b04040bfe_add_owning_project_and_creator_to_cas.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/3c3b04040bfe_add_owning_project_and_creator_to_cas.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/cd4106a1a0_add_cert_to_container_type.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/cd4106a1a0_add_cert_to_container_type.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/443d6f4a69ac_added_secret_type_column_to_secrets_.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/443d6f4a69ac_added_secret_type_column_to_secrets_.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1a7cf79559e3_new_secret_and_container_acl_tables.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1a7cf79559e3_new_secret_and_container_acl_tables.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/3041b53b95d7_remove_size_limits_on_meta_table_values.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/3041b53b95d7_remove_size_limits_on_meta_table_values.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/156cd9933643_add_project_column_to_consumer_table.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/156cd9933643_add_project_column_to_consumer_table.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/795737bb3c3_change_tenants_to_projects.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/795737bb3c3_change_tenants_to_projects.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/39cf2e645cba_model_for_multiple_backend_support.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/39cf2e645cba_model_for_multiple_backend_support.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/10220ccbe7fa_remove_transport_keys_column_from_.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/10220ccbe7fa_remove_transport_keys_column_from_.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/d2780d5aa510_change_url_length.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/d2780d5aa510_change_url_length.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/39a96e67e990_add_missing_constraints.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/39a96e67e990_add_missing_constraints.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/46b98cde536_add_project_quotas_table.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/46b98cde536_add_project_quotas_table.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/juno_initial.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/juno_initial.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/6a4457517a3_rename_acl_creator_only_to_project_.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/6a4457517a3_rename_acl_creator_only_to_project_.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/2d21598e7e70_added_ca_related_tables.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/2d21598e7e70_added_ca_related_tables.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/13d127569afa_create_secret_store_metadata_table.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/13d127569afa_create_secret_store_metadata_table.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/47b69e523451_made_plugin_names_in_kek_datum_non_.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/47b69e523451_made_plugin_names_in_kek_datum_non_.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1bece815014f_remove_projectsecret_table.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1bece815014f_remove_projectsecret_table.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/3d36a26b88af_add_order_barbican_metadata_table.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/3d36a26b88af_add_order_barbican_metadata_table.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/161f8aceb687_fill_project_id_to_secrets_where_missing.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/161f8aceb687_fill_project_id_to_secrets_where_missing.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1a0c2cdafb38_initial_version.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1a0c2cdafb38_initial_version.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/dce488646127_add_secret_user_metadata.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/dce488646127_add_secret_user_metadata.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1e86c18af2dd_add_new_columns_type_meta_containerid.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1e86c18af2dd_add_new_columns_type_meta_containerid.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/1c0f328bfce0_fixing_composite_primary_keys_and_.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/1c0f328bfce0_fixing_composite_primary_keys_and_.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/4070806f6972_add_orders_plugin_metadata_table_and_.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/4070806f6972_add_orders_plugin_metadata_table_and_.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/migration/alembic_migrations/versions/2ab3f5371bde_dsa_in_container_type_modelbase_to.py` & `barbican-9.0.1/barbican/model/migration/alembic_migrations/versions/2ab3f5371bde_dsa_in_container_type_modelbase_to.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/model/sync.py` & `barbican-9.0.1/barbican/model/sync.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/secret_acl.py` & `barbican-9.0.1/barbican/objects/secret_acl.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/secret_acl_user.py` & `barbican-9.0.1/barbican/objects/secret_acl_user.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/project_secret_store.py` & `barbican-9.0.1/barbican/objects/project_secret_store.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/kekdatum.py` & `barbican-9.0.1/barbican/objects/kekdatum.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/project_quotas.py` & `barbican-9.0.1/barbican/objects/project_quotas.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/transport_key.py` & `barbican-9.0.1/barbican/objects/transport_key.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/container_secret.py` & `barbican-9.0.1/barbican/objects/container_secret.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/base.py` & `barbican-9.0.1/barbican/objects/base.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/order_barbican_metadatum.py` & `barbican-9.0.1/barbican/objects/order_barbican_metadatum.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/project.py` & `barbican-9.0.1/barbican/objects/project.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/secret_stores.py` & `barbican-9.0.1/barbican/objects/secret_stores.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/container_acl.py` & `barbican-9.0.1/barbican/objects/container_acl.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/secret_store_metadatum.py` & `barbican-9.0.1/barbican/objects/secret_store_metadatum.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/__init__.py` & `barbican-9.0.1/barbican/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/fields.py` & `barbican-9.0.1/barbican/objects/fields.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/secret.py` & `barbican-9.0.1/barbican/objects/secret.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/secret_user_metadatum.py` & `barbican-9.0.1/barbican/objects/secret_user_metadatum.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/container_acl_user.py` & `barbican-9.0.1/barbican/objects/container_acl_user.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/order.py` & `barbican-9.0.1/barbican/objects/order.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/order_plugin_metadatum.py` & `barbican-9.0.1/barbican/objects/order_plugin_metadatum.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/order_retry_task.py` & `barbican-9.0.1/barbican/objects/order_retry_task.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/container_consumer_meta.py` & `barbican-9.0.1/barbican/objects/container_consumer_meta.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/encrypted_datum.py` & `barbican-9.0.1/barbican/objects/encrypted_datum.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/objects/container.py` & `barbican-9.0.1/barbican/objects/container.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/worker.py` & `barbican-9.0.1/barbican/cmd/worker.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/db_manage.py` & `barbican-9.0.1/barbican/cmd/db_manage.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/retry_scheduler.py` & `barbican-9.0.1/barbican/cmd/retry_scheduler.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/keystone_listener.py` & `barbican-9.0.1/barbican/cmd/keystone_listener.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/status.py` & `barbican-9.0.1/barbican/cmd/status.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/barbican_manage.py` & `barbican-9.0.1/barbican/cmd/barbican_manage.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/pkcs11_kek_rewrap.py` & `barbican-9.0.1/barbican/cmd/pkcs11_kek_rewrap.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/functionaltests/test_db_manage.py` & `barbican-9.0.1/barbican/cmd/functionaltests/test_db_manage.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/pkcs11_key_generation.py` & `barbican-9.0.1/barbican/cmd/pkcs11_key_generation.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/cmd/pkcs11_migrate_kek_signatures.py` & `barbican-9.0.1/barbican/cmd/pkcs11_migrate_kek_signatures.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/test_middleware_auth.py` & `barbican-9.0.1/barbican/tests/test_middleware_auth.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/test_transport_keys_resource.py` & `barbican-9.0.1/barbican/tests/api/test_transport_keys_resource.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/test_resources_policy.py` & `barbican-9.0.1/barbican/tests/api/test_resources_policy.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/test_init.py` & `barbican-9.0.1/barbican/tests/api/test_init.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/test_resources.py` & `barbican-9.0.1/barbican/tests/api/test_resources.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_quotas.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_quotas.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_secretmeta.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_secretmeta.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_secretstores.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_secretstores.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_containers.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_containers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_orders.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_orders.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_versions.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_versions.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_consumers.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_consumers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_acls.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_acls.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/controllers/test_secrets.py` & `barbican-9.0.1/barbican/tests/api/controllers/test_secrets.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/middleware/test_simple.py` & `barbican-9.0.1/barbican/tests/api/middleware/test_simple.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/api/middleware/test_context.py` & `barbican-9.0.1/barbican/tests/api/middleware/test_context.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/utils.py` & `barbican-9.0.1/barbican/tests/utils.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/certificate_utils.py` & `barbican-9.0.1/barbican/tests/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/test_manager.py` & `barbican-9.0.1/barbican/tests/plugin/crypto/test_manager.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/test_crypto.py` & `barbican-9.0.1/barbican/tests/plugin/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/test_p11_crypto.py` & `barbican-9.0.1/barbican/tests/plugin/crypto/test_p11_crypto.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/crypto/test_pkcs11.py` & `barbican-9.0.1/barbican/tests/plugin/crypto/test_pkcs11.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/test_snakeoil_ca.py` & `barbican-9.0.1/barbican/tests/plugin/test_snakeoil_ca.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/interface/test_secret_store.py` & `barbican-9.0.1/barbican/tests/plugin/interface/test_secret_store.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/interface/test_certificate_manager.py` & `barbican-9.0.1/barbican/tests/plugin/interface/test_certificate_manager.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/test_simple_certificate_manager.py` & `barbican-9.0.1/barbican/tests/plugin/test_simple_certificate_manager.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/util/test_utils.py` & `barbican-9.0.1/barbican/tests/plugin/util/test_utils.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/util/test_multiple_backends.py` & `barbican-9.0.1/barbican/tests/plugin/util/test_multiple_backends.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/util/test_mime_types.py` & `barbican-9.0.1/barbican/tests/plugin/util/test_mime_types.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/util/test_translations.py` & `barbican-9.0.1/barbican/tests/plugin/util/test_translations.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/test_dogtag.py` & `barbican-9.0.1/barbican/tests/plugin/test_dogtag.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/test_symantec.py` & `barbican-9.0.1/barbican/tests/plugin/test_symantec.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/test_store_crypto.py` & `barbican-9.0.1/barbican/tests/plugin/test_store_crypto.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/test_kmip.py` & `barbican-9.0.1/barbican/tests/plugin/test_kmip.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/test_resource.py` & `barbican-9.0.1/barbican/tests/plugin/test_resource.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/plugin/test_castellan_secret_store.py` & `barbican-9.0.1/barbican/tests/plugin/test_castellan_secret_store.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/tasks/test_common.py` & `barbican-9.0.1/barbican/tests/tasks/test_common.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/tasks/test_certificate_resources.py` & `barbican-9.0.1/barbican/tests/tasks/test_certificate_resources.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/tasks/test_resources.py` & `barbican-9.0.1/barbican/tests/tasks/test_resources.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/tasks/test_keystone_consumer.py` & `barbican-9.0.1/barbican/tests/tasks/test_keystone_consumer.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/common/test_utils.py` & `barbican-9.0.1/barbican/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/common/test_hrefs.py` & `barbican-9.0.1/barbican/tests/common/test_hrefs.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/common/test_validators.py` & `barbican-9.0.1/barbican/tests/common/test_validators.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/common/test_quota.py` & `barbican-9.0.1/barbican/tests/common/test_quota.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/database_utils.py` & `barbican-9.0.1/barbican/tests/database_utils.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/fixture.py` & `barbican-9.0.1/barbican/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/test_models.py` & `barbican-9.0.1/barbican/tests/model/test_models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_quotas.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_quotas.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_containers.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_containers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_transport_keys.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_transport_keys.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_secret_metadata.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_secret_metadata.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_order_retry_tasks.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_order_retry_tasks.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_projects.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_projects.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_secrets.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_secrets.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_certificate_authorities.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_certificate_authorities.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_secret_stores.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_secret_stores.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_consumers.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_consumers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_acls.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_acls.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/model/repositories/test_repositories_orders.py` & `barbican-9.0.1/barbican/tests/model/repositories/test_repositories_orders.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/test_hacking.py` & `barbican-9.0.1/barbican/tests/test_hacking.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/objects/test_ovo_project.py` & `barbican-9.0.1/barbican/tests/objects/test_ovo_project.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/objects/test_ovo_base.py` & `barbican-9.0.1/barbican/tests/objects/test_ovo_base.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/objects/test_ovo_project_quotas.py` & `barbican-9.0.1/barbican/tests/objects/test_ovo_project_quotas.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/cmd/test_barbican_manage.py` & `barbican-9.0.1/barbican/tests/cmd/test_barbican_manage.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/cmd/test-status.py` & `barbican-9.0.1/barbican/tests/cmd/test-status.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/cmd/test_cmd.py` & `barbican-9.0.1/barbican/tests/cmd/test_cmd.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/cmd/test_db_cleanup.py` & `barbican-9.0.1/barbican/tests/cmd/test_db_cleanup.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/queue/test_keystone_listener.py` & `barbican-9.0.1/barbican/tests/queue/test_keystone_listener.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/queue/test_client.py` & `barbican-9.0.1/barbican/tests/queue/test_client.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/queue/test_server.py` & `barbican-9.0.1/barbican/tests/queue/test_server.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/queue/test_retry_scheduler.py` & `barbican-9.0.1/barbican/tests/queue/test_retry_scheduler.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/tests/keys.py` & `barbican-9.0.1/barbican/tests/keys.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/hacking/checks.py` & `barbican-9.0.1/barbican/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/queue/server.py` & `barbican-9.0.1/barbican/queue/server.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/queue/retry_scheduler.py` & `barbican-9.0.1/barbican/queue/retry_scheduler.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/queue/client.py` & `barbican-9.0.1/barbican/queue/client.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/queue/__init__.py` & `barbican-9.0.1/barbican/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/queue/keystone_listener.py` & `barbican-9.0.1/barbican/queue/keystone_listener.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican/i18n.py` & `barbican-9.0.1/barbican/i18n.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/README.rst` & `barbican-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/HACKING.rst` & `barbican-9.0.1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/apiary.apib` & `barbican-9.0.1/apiary.apib`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/.zuul.yaml` & `barbican-9.0.1/.zuul.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 - job:
     name: barbican-devstack-functional-base
-    # start running with Pike
-    branches: ^(?!stable/ocata).*$
     parent: legacy-dsvm-base
     vars:
       database: sql
       python_version: py36
       services: tempest,rabbit,mysql,key
     required-projects:
       - openstack/devstack-gate
@@ -130,16 +128,14 @@
     parent: barbican-devstack-tempest-base
     vars:
       cursive: 1
 
 - job:
     name: barbican-grenade-devstack
     parent: legacy-dsvm-base
-    # Start testing with pike
-    branches: ^(?!stable/ocata).*$
     irrelevant-files:
       - ^(test-|)requirements.txt$
       - ^setup.cfg$
     run: playbooks/legacy/grenade-devstack-barbican/run.yaml
     post-run: playbooks/legacy/grenade-devstack-barbican/post.yaml
     required-projects:
       - openstack/grenade
```

### Comparing `barbican-9.0.0.0rc1/requirements.txt` & `barbican-9.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/LICENSE` & `barbican-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/acls.rst` & `barbican-9.0.1/doc/source/api/reference/acls.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/secrets.rst` & `barbican-9.0.1/doc/source/api/reference/secrets.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/store_backends.rst` & `barbican-9.0.1/doc/source/api/reference/store_backends.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/containers.rst` & `barbican-9.0.1/doc/source/api/reference/containers.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/orders.rst` & `barbican-9.0.1/doc/source/api/reference/orders.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/consumers.rst` & `barbican-9.0.1/doc/source/api/reference/consumers.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/quotas.rst` & `barbican-9.0.1/doc/source/api/reference/quotas.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/secret_metadata.rst` & `barbican-9.0.1/doc/source/api/reference/secret_metadata.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/reference/secret_types.rst` & `barbican-9.0.1/doc/source/api/reference/secret_types.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/api/index.rst` & `barbican-9.0.1/doc/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/cli/barbican-status.rst` & `barbican-9.0.1/doc/source/cli/barbican-status.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/index.rst` & `barbican-9.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/install-ubuntu.rst` & `barbican-9.0.1/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/common_prerequisites.rst` & `barbican-9.0.1/doc/source/install/common_prerequisites.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/common_configure.rst` & `barbican-9.0.1/doc/source/install/common_configure.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/install-rdo.rst` & `barbican-9.0.1/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/verify.rst` & `barbican-9.0.1/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/install.rst` & `barbican-9.0.1/doc/source/install/install.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/get_started.rst` & `barbican-9.0.1/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/barbican-backend.rst` & `barbican-9.0.1/doc/source/install/barbican-backend.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/index.rst` & `barbican-9.0.1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/install/install-obs.rst` & `barbican-9.0.1/doc/source/install/install-obs.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/architecture.rst` & `barbican-9.0.1/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/devstack.rst` & `barbican-9.0.1/doc/source/contributor/devstack.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/plugin/crypto.rst` & `barbican-9.0.1/doc/source/contributor/plugin/crypto.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/plugin/secret_store.rst` & `barbican-9.0.1/doc/source/contributor/plugin/secret_store.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/plugin/index.rst` & `barbican-9.0.1/doc/source/contributor/plugin/index.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/dataflow.rst` & `barbican-9.0.1/doc/source/contributor/dataflow.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/getting_involved.rst` & `barbican-9.0.1/doc/source/contributor/getting_involved.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/dependencies.rst` & `barbican-9.0.1/doc/source/contributor/dependencies.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/index.rst` & `barbican-9.0.1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/dev.rst` & `barbican-9.0.1/doc/source/contributor/dev.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/structure.rst` & `barbican-9.0.1/doc/source/contributor/structure.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/testing.rst` & `barbican-9.0.1/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/contributor/database_migrations.rst` & `barbican-9.0.1/doc/source/contributor/database_migrations.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/configuration/keystone.rst` & `barbican-9.0.1/doc/source/configuration/keystone.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/configuration/troubleshooting.rst` & `barbican-9.0.1/doc/source/configuration/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/configuration/plugin_backends.rst` & `barbican-9.0.1/doc/source/configuration/plugin_backends.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/configuration/noauth.rst` & `barbican-9.0.1/doc/source/configuration/noauth.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/configuration/audit.rst` & `barbican-9.0.1/doc/source/configuration/audit.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/_extra/.htaccess` & `barbican-9.0.1/doc/source/_extra/.htaccess`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/admin/upgrade.rst` & `barbican-9.0.1/doc/source/admin/upgrade.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/admin/database_cleaning.rst` & `barbican-9.0.1/doc/source/admin/database_cleaning.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/admin/barbican_manage.rst` & `barbican-9.0.1/doc/source/admin/barbican_manage.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/admin/access_control.rst` & `barbican-9.0.1/doc/source/admin/access_control.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/images/barbican-overall-architecture.gif` & `barbican-9.0.1/doc/source/images/barbican-overall-architecture.gif`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/images/barbican-components.gif` & `barbican-9.0.1/doc/source/images/barbican-components.gif`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/conf.py` & `barbican-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/doc/source/sample_policy.rst` & `barbican-9.0.1/doc/source/sample_policy.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-tempest-base/run.yaml` & `barbican-9.0.1/playbooks/legacy/barbican-devstack-tempest-base/run.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/playbooks/legacy/grenade-devstack-barbican/run.yaml` & `barbican-9.0.1/playbooks/legacy/grenade-devstack-barbican/run.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-functional-base/dogtag-post.yaml` & `barbican-9.0.1/playbooks/legacy/barbican-devstack-functional-base/dogtag-post.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-functional-base/run.yaml` & `barbican-9.0.1/playbooks/legacy/barbican-devstack-functional-base/run.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/playbooks/legacy/barbican-devstack-base/run.yaml` & `barbican-9.0.1/playbooks/legacy/barbican-devstack-base/run.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/devstack/settings` & `barbican-9.0.1/devstack/settings`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Defaults
 # --------
 
 # Set up default directories
 BARBICAN_DIR=$DEST/barbican
-BARBICANCLIENT_DIR=$DEST/python-barbicanclient
 BARBICAN_CONF_DIR=${BARBICAN_CONF_DIR:-/etc/barbican}
 BARBICAN_CONF=$BARBICAN_CONF_DIR/barbican.conf
 BARBICAN_PASTE_CONF=$BARBICAN_CONF_DIR/barbican-api-paste.ini
 BARBICAN_API_LOG_DIR=$DEST/logs
 BARBICAN_AUTH_CACHE_DIR=${BARBICAN_AUTH_CACHE_DIR:-/var/cache/barbican}
 
 PYKMIP_CONF_DIR=${PYKMIP_CONF_DIR:-/etc/pykmip}
@@ -25,17 +24,18 @@
 BARBICAN_WSGI=$BARBICAN_BIN_DIR/barbican-wsgi-api
 BARBICAN_UWSGI_CONF=$BARBICAN_CONF_DIR/barbican-uwsgi.ini
 
 # Set Barbican repository
 BARBICAN_REPO=${BARBICAN_REPO:-${GIT_BASE}/openstack/barbican.git}
 BARBICAN_BRANCH=${BARBICAN_BRANCH:-master}
 
-# Set client library repository
-BARBICANCLIENT_REPO=${BARBICANCLIENT_REPO:-${GIT_BASE}/openstack/python-barbicanclient.git}
-BARBICANCLIENT_BRANCH=${BARBICANCLIENT_BRANCH:-master}
+# python barbican client library
+GITREPO["python-barbicanclient"]=${BARBICANCLIENT_REPO:-${GIT_BASE}/openstack/python-barbicanclient.git}
+GITBRANCH["python-barbicanclient"]=${BARBICANCLIENT_BRANCH:-$TARGET_BRANCH}
+GITDIR["python-barbicanclient"]=$DEST/python-barbicanclient
 
 # Set host href
 BARBICAN_HOST_HREF=${BARBICAN_HOST_HREF:-http://${SERVICE_HOST}/key-manager}
 
 GITREPO["barbican-tempest-plugin"]=${BARBICANTEMPEST_REPO:-${GIT_BASE}/openstack/barbican-tempest-plugin.git}
 GITBRANCH["barbican-tempest-plugin"]=${BARBICANTEMPEST_BRANCH:-master}
 GITDIR["barbican-tempest-plugin"]=$DEST/barbican-tempest-plugin
```

### Comparing `barbican-9.0.0.0rc1/devstack/barbican-vagrant/Vagrantfile` & `barbican-9.0.1/devstack/barbican-vagrant/Vagrantfile`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/devstack/upgrade/settings` & `barbican-9.0.1/devstack/upgrade/settings`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/devstack/upgrade/resources.sh` & `barbican-9.0.1/devstack/upgrade/resources.sh`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/devstack/upgrade/upgrade.sh` & `barbican-9.0.1/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/devstack/upgrade/shutdown.sh` & `barbican-9.0.1/devstack/upgrade/shutdown.sh`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/devstack/README.md` & `barbican-9.0.1/devstack/README.md`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/devstack/lib/barbican` & `barbican-9.0.1/devstack/lib/barbican`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 # runs that a clean run would need to clean up
 function cleanup_barbican {
     :
 }
 
 # configure_barbicanclient - Set config files, create data dirs, etc
 function configure_barbicanclient {
-    setup_develop $BARBICANCLIENT_DIR
+    setup_dev_lib "python-barbicanclient"
 }
 
 # configure_dogtag_plugin - Change config to use dogtag plugin
 function configure_dogtag_plugin {
     sudo openssl pkcs12 -in /root/.dogtag/pki-tomcat/ca_admin_cert.p12 -passin pass:PASSWORD -out $BARBICAN_CONF_DIR/kra_admin_cert.pem -nodes
     sudo chown $USER $BARBICAN_CONF_DIR/kra_admin_cert.pem
     iniset $BARBICAN_CONF dogtag_plugin dogtag_port 8373
@@ -180,16 +180,18 @@
     # TODO(ravips): We need this until barbican gets into devstack
     setup_develop $BARBICAN_DIR
     pip_install 'uwsgi'
 }
 
 # install_barbicanclient - Collect source and prepare
 function install_barbicanclient {
-    git_clone $BARBICANCLIENT_REPO $BARBICANCLIENT_DIR $BARBICANCLIENT_BRANCH
-    setup_develop $BARBICANCLIENT_DIR
+    if use_library_from_git "python-barbicanclient"; then
+        git_clone_by_name "python-barbicanclient"
+        setup_dev_lib "python-barbicanclient"
+    fi
 }
 
 # start_barbican - Start running processes, including screen
 function start_barbican {
     # Start the Barbican service up.
     run_process barbican-svc "$BARBICAN_BIN_DIR/uwsgi --ini $BARBICAN_UWSGI_CONF"
```

### Comparing `barbican-9.0.0.0rc1/devstack/gate_hook.sh` & `barbican-9.0.1/devstack/gate_hook.sh`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/devstack/plugin.sh` & `barbican-9.0.1/devstack/plugin.sh`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
             echo_summary "Configuring Dogtag plugin"
             configure_dogtag_plugin
         fi
         if is_service_enabled barbican-vault; then
             echo_summary "Configuring Vault plugin"
             configure_vault_plugin
         fi
-        configure_barbicanclient
 
         # Configure Cinder, Nova and Glance to use Barbican
         configure_core_services
 
         if is_service_enabled key; then
             create_barbican_accounts
         fi
```

### Comparing `barbican-9.0.0.0rc1/tox.ini` & `barbican-9.0.1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 envlist = py27,py36,py37,pep8,docs
 skipsdist = True
 
 [testenv]
 setenv =
     PYTHON=coverage run --source barbican --parallel-mode
 usedevelop = True
-install_command = pip install -c{env:UPPER_CONSTRAINTS_FILE:https://opendev.org/openstack/requirements/raw/branch/master/upper-constraints.txt} -U {opts} {packages}
+install_command = pip install -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train} -U {opts} {packages}
 deps = -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 
 commands =
     oslo-config-generator --config-file etc/oslo-config-generator/barbican.conf --output-file etc/barbican/barbican.conf
     /usr/bin/find . -type f -name "*.py[c|o]" -delete
     rm -f .testrepository/times.dbm
```

### Comparing `barbican-9.0.0.0rc1/barbican.egg-info/PKG-INFO` & `barbican-9.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barbican
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: OpenStack Secure Key Management
 Home-page: https://docs.openstack.org/barbican/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Service for storing sensitive client information for OpenStack
 Platform: UNKNOWN
```

### Comparing `barbican-9.0.0.0rc1/barbican.egg-info/SOURCES.txt` & `barbican-9.0.1/barbican.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican.egg-info/requires.txt` & `barbican-9.0.1/barbican.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/barbican.egg-info/entry_points.txt` & `barbican-9.0.1/barbican.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/ChangeLog` & `barbican-9.0.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 CHANGES
 =======
 
-9.0.0.0rc1
-----------
+9.0.1
+-----
+
+* Fix the barbicanclient installation not from source
+* Don't use branch matching
+* Update TOX/UPPER\_CONSTRAINTS\_FILE for stable/train
+* Update .gitreview for stable/train
+
+9.0.0
+-----
 
 * Start using the f29 nodeset
 * Ensure doc/source/\_static to fix docs gate
 * Fix py3 compatibility issue in PKCS#11 plugin
 * Imported Translations from Zanata
 * Update Castellan minimum version
 * Make broken job barbican-kmip-devstack-functional experimental
```

### Comparing `barbican-9.0.0.0rc1/etc/barbican/barbican-api-paste.ini` & `barbican-9.0.1/etc/barbican/barbican-api-paste.ini`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/etc/barbican/api_audit_map.conf` & `barbican-9.0.1/etc/barbican/api_audit_map.conf`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/etc/barbican/barbican-functional.conf` & `barbican-9.0.1/etc/barbican/barbican-functional.conf`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/etc/oslo-config-generator/barbican.conf` & `barbican-9.0.1/etc/oslo-config-generator/barbican.conf`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/bin/demo_requests.py` & `barbican-9.0.1/bin/demo_requests.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/bin/barbican.sh` & `barbican-9.0.1/bin/barbican.sh`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/bin/versionbuild.py` & `barbican-9.0.1/bin/versionbuild.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/bin/keystone_data.sh` & `barbican-9.0.1/bin/keystone_data.sh`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/releasenotes/notes/http_proxy_to_wsgi-middleware-98dc4fe03eb362d3.yaml` & `barbican-9.0.1/releasenotes/notes/http_proxy_to_wsgi-middleware-98dc4fe03eb362d3.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/releasenotes/notes/multiple-backends-75f5b85c63b930b7.yaml` & `barbican-9.0.1/releasenotes/notes/multiple-backends-75f5b85c63b930b7.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/releasenotes/notes/removing-cas-certificate-orders-96fc47a7acaea273.yaml` & `barbican-9.0.1/releasenotes/notes/removing-cas-certificate-orders-96fc47a7acaea273.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/releasenotes/notes/pkcs11-backend-performance-f3caacbe9e1ab535.yaml` & `barbican-9.0.1/releasenotes/notes/pkcs11-backend-performance-f3caacbe9e1ab535.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/releasenotes/notes/barbican-manage-d469b4d15454f981.yaml` & `barbican-9.0.1/releasenotes/notes/barbican-manage-d469b4d15454f981.yaml`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `barbican-9.0.1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `barbican-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/releasenotes/source/conf.py` & `barbican-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/acls.rst` & `barbican-9.0.1/api-guide/source/acls.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/secrets.rst` & `barbican-9.0.1/api-guide/source/secrets.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/containers.rst` & `barbican-9.0.1/api-guide/source/containers.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/orders.rst` & `barbican-9.0.1/api-guide/source/orders.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/consumers.rst` & `barbican-9.0.1/api-guide/source/consumers.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/quotas.rst` & `barbican-9.0.1/api-guide/source/quotas.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/secret_metadata.rst` & `barbican-9.0.1/api-guide/source/secret_metadata.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/pkcs11keygeneration.rst` & `barbican-9.0.1/api-guide/source/pkcs11keygeneration.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/dogtag_setup.rst` & `barbican-9.0.1/api-guide/source/dogtag_setup.rst`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/api-guide/source/conf.py` & `barbican-9.0.1/api-guide/source/conf.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/AUTHORS` & `barbican-9.0.1/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
 Kiran_totad <kiran.totad@nectechnologies.in>
 Le Hou <houl7@chinaunicom.cn>
 Lingxian Kong <anlin.kong@gmail.com>
 Lisa Clark <lisa.clark@rackspace.com>
 Longgeek <longgeek@thstack.com>
 Louis Taylor <kragniz@gmail.com>
 Lucky samadhiya <lucky.samadhiya@nectechnologies.in>
+Luigi Toscano <ltoscano@redhat.com>
 Luong Anh Tuan <tuanla@vn.fujitsu.com>
 Luz <luz.cazares@intel.com>
 M V P Nitesh <m.nitesh@nectechnologies.in>
 Malini K. Bhandaru <malini.k.bhandaru@intel.com>
 Marc Koderer <marc@koderer.com>
 Marc Methot <mmethot@redhat.com>
 Martin Kletzander <mkletzan@redhat.com>
```

### Comparing `barbican-9.0.0.0rc1/setup.cfg` & `barbican-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/setup.py` & `barbican-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/base.py` & `barbican-9.0.1/functionaltests/api/base.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_containers.py` & `barbican-9.0.1/functionaltests/api/v1/smoke/test_containers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_orders.py` & `barbican-9.0.1/functionaltests/api/v1/smoke/test_orders.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_versions.py` & `barbican-9.0.1/functionaltests/api/v1/smoke/test_versions.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_consumers.py` & `barbican-9.0.1/functionaltests/api/v1/smoke/test_consumers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/smoke/test_secrets.py` & `barbican-9.0.1/functionaltests/api/v1/smoke/test_secrets.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/models/base_models.py` & `barbican-9.0.1/functionaltests/api/v1/models/base_models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/models/consumer_model.py` & `barbican-9.0.1/functionaltests/api/v1/models/consumer_model.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/models/quota_models.py` & `barbican-9.0.1/functionaltests/api/v1/models/quota_models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/models/acl_models.py` & `barbican-9.0.1/functionaltests/api/v1/models/acl_models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/models/ca_models.py` & `barbican-9.0.1/functionaltests/api/v1/models/ca_models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/models/secret_models.py` & `barbican-9.0.1/functionaltests/api/v1/models/secret_models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/models/order_models.py` & `barbican-9.0.1/functionaltests/api/v1/models/order_models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/models/container_models.py` & `barbican-9.0.1/functionaltests/api/v1/models/container_models.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/acl_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/acl_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/secretstores_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/secretstores_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/consumer_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/consumer_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/container_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/container_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/secret_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/secret_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/quota_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/quota_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/base_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/base_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/order_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/order_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/behaviors/secretmeta_behaviors.py` & `barbican-9.0.1/functionaltests/api/v1/behaviors/secretmeta_behaviors.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_quotas.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_quotas.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_secretmeta.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_secretmeta.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_acls_rbac.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_acls_rbac.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_secretstores.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_secretstores.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_quotas_enforce.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_quotas_enforce.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_containers.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_containers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_orders.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_orders.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_consumers.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_consumers.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_quotas_rbac.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_quotas_rbac.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_acls.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_acls.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_rsa.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_rsa.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_secrets.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_secrets.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_orders_rbac.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_orders_rbac.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_secrets_rbac.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_secrets_rbac.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/api/v1/functional/test_containers_rbac.py` & `barbican-9.0.1/functionaltests/api/v1/functional/test_containers_rbac.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/post_test_hook.sh` & `barbican-9.0.1/functionaltests/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/run_tests.sh` & `barbican-9.0.1/functionaltests/run_tests.sh`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/common/config.py` & `barbican-9.0.1/functionaltests/common/config.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/common/client.py` & `barbican-9.0.1/functionaltests/common/client.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/common/auth.py` & `barbican-9.0.1/functionaltests/common/auth.py`

 * *Files identical despite different names*

### Comparing `barbican-9.0.0.0rc1/functionaltests/run_tests_parallel.sh` & `barbican-9.0.1/functionaltests/run_tests_parallel.sh`

 * *Files identical despite different names*

