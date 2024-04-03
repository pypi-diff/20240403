# Comparing `tmp/neutron-fwaas-20.0.0.tar.gz` & `tmp/neutron-fwaas-20.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-fwaas-20.0.0.tar", last modified: Wed Apr  3 11:51:54 2024, max compression
+gzip compressed data, was "neutron-fwaas-20.0.0.0rc1.tar", last modified: Thu Mar 14 06:25:29 2024, max compression
```

## Comparing `neutron-fwaas-20.0.0.tar` & `neutron-fwaas-20.0.0.0rc1.tar`

### file list

```diff
@@ -1,421 +1,421 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.341352 neutron-fwaas-20.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      590 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3491 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3668 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12564 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62360 2024-04-03 11:51:53.000000 neutron-fwaas-20.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2024-04-03 11:51:54.341352 neutron-fwaas-20.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/TESTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.285350 neutron-fwaas-20.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.285350 neutron-fwaas-20.0.0/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/devstack/lib/l2_agent
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/devstack/lib/l3_agent
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4329 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.285350 neutron-fwaas-20.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.285350 neutron-fwaas-20.0.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.285350 neutron-fwaas-20.0.0/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10109 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.285350 neutron-fwaas-20.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/configuration/fwaas_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/configuration/neutron_fwaas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/configuration/policy-sample.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/configuration/policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.285350 neutron-fwaas-20.0.0/doc/source/configuration/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/configuration/samples/fwaas_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/configuration/samples/neutron_fwaas.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.289350 neutron-fwaas-20.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1141 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/contributor/devstack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/contributor/fwaas_v2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/contributor/modules.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.289350 neutron-fwaas-20.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.289350 neutron-fwaas-20.0.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/etc/README.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.265349 neutron-fwaas-20.0.0/etc/neutron/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.289350 neutron-fwaas-20.0.0/etc/neutron/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/etc/neutron/rootwrap.d/fwaas-privsep.filters
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.289350 neutron-fwaas-20.0.0/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/etc/oslo-config-generator/fwaas_driver.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/etc/oslo-config-generator/neutron_fwaas.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.289350 neutron-fwaas-20.0.0/etc/oslo-policy-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/etc/oslo-policy-generator/policy.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.289350 neutron-fwaas-20.0.0/neutron_fwaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.293350 neutron-fwaas-20.0.0/neutron_fwaas/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/cmd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.293350 neutron-fwaas-20.0.0/neutron_fwaas/cmd/upgrade_checks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/cmd/upgrade_checks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1414 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/cmd/upgrade_checks/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5715 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/cmd/v1_to_v2_db_migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.293350 neutron-fwaas-20.0.0/neutron_fwaas/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1301 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/common/fwaas_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/common/resources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.293350 neutron-fwaas-20.0.0/neutron_fwaas/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.293350 neutron-fwaas-20.0.0/neutron_fwaas/db/firewall/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/firewall/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3627 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/firewall/firewall_db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.293350 neutron-fwaas-20.0.0/neutron_fwaas/db/firewall/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/firewall/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51848 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/firewall/v2/firewall_db_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.293350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.293350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.265349 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/2023.2/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/2023.2/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/2023.2/expand/6941ce70131e_add_standard_attr_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/4202e3047e47_add_index_tenant_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2074 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/540142f314f4_fwaas_router_insertion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/796c68dffbb_cisco_csr_fwaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/CONTRACT_HEAD
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/EXPAND_HEAD
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/kilo_release.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.265349 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/contract/67c8e8d61d5_initial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/4b47ea298795_add_reject_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/c40fbb377ad_initial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.265349 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/mitaka/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/mitaka/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/mitaka/contract/458aa42b14b_fw_table_alter.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.269349 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/newton/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/newton/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3429 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/newton/contract/f83a0b2964d0_rename_tenant_to_project.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/newton/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4517 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/newton/expand/d6a12e637e28_neutron_fwaas_v2_0.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.269349 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/pike/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/pike/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/pike/contract/fd38cd995cc0_shared_attribute_for_firewall_resources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.269349 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/queens/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2419 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/876782258a43_create_default_firewall_groups_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2401 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/f24e0d5e5bff_uniq_firewallgroupportassociation0port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/start_neutron_fwaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/db/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/db/models/head.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.297350 neutron-fwaas-20.0.0/neutron_fwaas/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8082 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/extensions/firewall_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/extensions/firewall_v2_stdattrs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1242 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.301350 neutron-fwaas-20.0.0/neutron_fwaas/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3020 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/policies/firewall_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3059 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/policies/firewall_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3585 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/policies/firewall_rule.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.301350 neutron-fwaas-20.0.0/neutron_fwaas/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.301350 neutron-fwaas-20.0.0/neutron_fwaas/privileged/netfilter_log/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/netfilter_log/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10585 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/netfilter_log/libnetfilter_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2737 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/netlink_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12940 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/netlink_lib.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.301350 neutron-fwaas-20.0.0/neutron_fwaas/privileged/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.301350 neutron-fwaas-20.0.0/neutron_fwaas/privileged/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1096 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/tests/functional/dummy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/tests/functional/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/privileged/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.301350 neutron-fwaas-20.0.0/neutron_fwaas/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.301350 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19090 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/fwaas_plugin_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.301350 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.305350 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16312 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/agents.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.305350 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1779 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/conntrack_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4311 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/fwaas_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/fwaas_base_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.305350 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23997 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/iptables_fwaas_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.305350 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1805 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/driver_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.305350 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/noop/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/noop/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1300 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/noop/noop_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.309351 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41153 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/firewall.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7603 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9610 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/legacy_conntrack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5628 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/netlink_conntrack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/firewall_agent_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/firewall_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.309351 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/l2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/l2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19276 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/l2/fwaas_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.309351 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/l3reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/l3reference/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23933 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/l3reference/firewall_l3_agent_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19934 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/driver_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.309351 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.309351 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.309351 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.309351 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/drivers/iptables/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/drivers/iptables/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2596 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/drivers/iptables/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20205 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/drivers/iptables/log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.309351 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/l3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/l3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/l3/fwg_log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.313351 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2438 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/common/fwg_callback.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7804 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/common/log_db_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/common/port_callback.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5063 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/fwg_validate.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.313351 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/rpc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/rpc/log_server.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.313351 neutron-fwaas-20.0.0/neutron_fwaas/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.313351 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/filters.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/functional-testing.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/gate_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1062 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/gate_hook_tempest.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.313351 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/hooks/api_extensions-base
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/hooks/api_extensions-legacy
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/hooks/api_extensions-v1
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/hooks/api_extensions-v2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/hooks/iptables_verify
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/post_test_hook.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2608 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9080 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10390 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14106 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/environment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6049 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/machine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8397 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7378 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/test_l3_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/db/test_migrations.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/privileged/test_dummy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7383 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/privileged/test_netlink_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/privileged/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/agents/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/agents/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.317351 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/agents/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/agents/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/agents/drivers/iptables/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/agents/drivers/iptables/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25021 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/agents/drivers/iptables/test_log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/cmd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/cmd/upgrade_checks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/cmd/upgrade_checks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/cmd/upgrade_checks/test_checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/db/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/db/firewall/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/db/firewall/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/db/firewall/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/db/firewall/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    93235 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/db/firewall/v2/test_firewall_db_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/netfilter_log/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/netfilter_log/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5509 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/netfilter_log/test_libnetfilter_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15708 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/test_netlink_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.321351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.325351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.325351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.325351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.325351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.325351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/noop/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/noop/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/noop/test_noop_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.325351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32824 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/test_firewall.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13075 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/test_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23606 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_iptables_fwaas_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6649 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_legacy_conntrack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10470 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_netlink_conntrack.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.325351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5286 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/fake_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30424 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/test_fwaas_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.325351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l3reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l3reference/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27940 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l3reference/test_firewall_l3_agent_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29131 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_agents.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3217 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_firewall_agent_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2474 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_firewall_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13178 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/test_driver_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34200 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/test_fwaas_plugin_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.329351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.329351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.329351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.329351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14785 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/test_log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.329351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/l3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/l3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2206 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/l3/test_fwg_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.329351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9741 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/common/test_fwg_callback.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14732 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/common/test_log_db_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8648 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/common/test_port_callback.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.329351 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/rpc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2365 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/rpc/test_log_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6821 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/test_fwg_validate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/neutron_fwaas/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.289350 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16247 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2024-04-03 11:51:54.000000 neutron-fwaas-20.0.0/neutron_fwaas.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.329351 neutron-fwaas-20.0.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/playbooks/configure_functional_job.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.277349 neutron-fwaas-20.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.337351 neutron-fwaas-20.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/adding-new-tables-for-future-consumption-ffd537c1f82e2e01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/auto-association-default-firewall-group-7e9faf1afca1df85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/bug-1702242-c917c832ac2fa4e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/bug-1746404-493a66faac333403.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/bug-1799358-360c6ab27a32e0ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/cisco-fwaas-driver-move-8f46325d13c93543.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/coexistence-between-sg-and-fwg-1f77a755539a9463.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/config-file-generation-265c5256668a26bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/deprecate-neutron-fwaas-as-stadium-project-934d6acb3e824249.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/drop-python-2-7-73d3113c69d724c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/drop-python-3-6-and-3-7-b1cf8738aaab988f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/enable-quotas-a3d0a21743bb1985.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/fwaas-config-9c780ccfb0e7887f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/fwaas-v2-logging-79cbaa43ff17f47f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/fwaas_v2-374471c215af0ca0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/mcafee-fwaas-driver-removal-8915271e5d4288cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/ovs-firewall-driver-c347ea0a560b7e38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/remove_fwaas_v1-15c6e19484f46d1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/validation_if_port_is_supported-639d0df705eb67f9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/varmour-fwaas-driver-removal-f7aa304a4544134a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/notes/vyatta-fwaas-driver-removal-e38e6ecde5105084.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.337351 neutron-fwaas-20.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.337351 neutron-fwaas-20.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.337351 neutron-fwaas-20.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9203 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.277349 neutron-fwaas-20.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.277349 neutron-fwaas-20.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.337351 neutron-fwaas-20.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17917 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.277349 neutron-fwaas-20.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.337351 neutron-fwaas-20.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.277349 neutron-fwaas-20.0.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.337351 neutron-fwaas-20.0.0/roles/configure_functional_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/roles/configure_functional_tests/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.341352 neutron-fwaas-20.0.0/roles/configure_functional_tests/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/roles/configure_functional_tests/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.341352 neutron-fwaas-20.0.0/roles/configure_functional_tests/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/roles/configure_functional_tests/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2024-04-03 11:51:54.341352 neutron-fwaas-20.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:54.341352 neutron-fwaas-20.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1613 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/tools/check_unit_test_structure.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      196 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/tools/clean.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8974 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/tools/configure_for_func_testing.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      850 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/tools/configure_for_fwaas_func_testing.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2180 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/tools/deploy_rootwrap.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      800 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/tools/generate_config_file_samples.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2024-04-03 11:51:27.000000 neutron-fwaas-20.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.024930 neutron-fwaas-20.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      590 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3491 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3668 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12564 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62370 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2124 2024-03-14 06:25:29.024930 neutron-fwaas-20.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/TESTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.984929 neutron-fwaas-20.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.984929 neutron-fwaas-20.0.0.0rc1/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/devstack/lib/l2_agent
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/devstack/lib/l3_agent
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4329 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.984929 neutron-fwaas-20.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.984929 neutron-fwaas-20.0.0.0rc1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.984929 neutron-fwaas-20.0.0.0rc1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10109 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/fwaas_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/neutron_fwaas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/policy-sample.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/samples/fwaas_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/configuration/samples/neutron_fwaas.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1141 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/contributor/devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/contributor/fwaas_v2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/contributor/modules.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/etc/README.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.976929 neutron-fwaas-20.0.0.0rc1/etc/neutron/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/etc/neutron/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/etc/neutron/rootwrap.d/fwaas-privsep.filters
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/etc/oslo-config-generator/fwaas_driver.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/etc/oslo-config-generator/neutron_fwaas.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/etc/oslo-policy-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/etc/oslo-policy-generator/policy.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.988929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/cmd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/cmd/upgrade_checks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/cmd/upgrade_checks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1414 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/cmd/upgrade_checks/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5715 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/cmd/v1_to_v2_db_migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1301 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/common/fwaas_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/common/resources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/firewall/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/firewall/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3627 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/firewall/firewall_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/firewall/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/firewall/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51848 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/firewall/v2/firewall_db_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.976929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/2023.2/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/2023.2/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/2023.2/expand/6941ce70131e_add_standard_attr_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/4202e3047e47_add_index_tenant_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2074 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/540142f314f4_fwaas_router_insertion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/796c68dffbb_cisco_csr_fwaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/CONTRACT_HEAD
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/EXPAND_HEAD
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/kilo_release.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.976929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/contract/67c8e8d61d5_initial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/4b47ea298795_add_reject_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/c40fbb377ad_initial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.976929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/mitaka/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/mitaka/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/mitaka/contract/458aa42b14b_fw_table_alter.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.976929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/newton/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/newton/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3429 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/newton/contract/f83a0b2964d0_rename_tenant_to_project.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/newton/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4517 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/newton/expand/d6a12e637e28_neutron_fwaas_v2_0.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.976929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/pike/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/pike/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/pike/contract/fd38cd995cc0_shared_attribute_for_firewall_resources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.976929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/queens/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.996930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2419 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/876782258a43_create_default_firewall_groups_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2401 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/f24e0d5e5bff_uniq_firewallgroupportassociation0port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/start_neutron_fwaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.996930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/models/head.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.996930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8082 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/extensions/firewall_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/extensions/firewall_v2_stdattrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1242 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.996930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3020 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/firewall_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3059 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/firewall_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3585 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/firewall_rule.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.996930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.996930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/netfilter_log/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/netfilter_log/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10585 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/netfilter_log/libnetfilter_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2737 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/netlink_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12940 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/netlink_lib.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.996930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.996930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1096 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/tests/functional/dummy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/tests/functional/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19090 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/fwaas_plugin_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16312 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/agents.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1779 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/conntrack_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4311 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/fwaas_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/fwaas_base_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23997 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/iptables_fwaas_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1805 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/driver_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/noop/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/noop/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1300 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/noop/noop_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41153 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/firewall.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7603 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9610 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/legacy_conntrack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5628 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/netlink_conntrack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/firewall_agent_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/firewall_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/l2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/l2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19276 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/l2/fwaas_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.000929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/l3reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/l3reference/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23933 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/l3reference/firewall_l3_agent_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19934 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/driver_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/drivers/iptables/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/drivers/iptables/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2596 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/drivers/iptables/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20205 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/drivers/iptables/log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/l3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/l3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/l3/fwg_log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2438 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/common/fwg_callback.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7804 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/common/log_db_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/common/port_callback.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5063 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/fwg_validate.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/rpc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/rpc/log_server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/filters.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/functional-testing.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/gate_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1062 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/gate_hook_tempest.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/hooks/api_extensions-base
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/hooks/api_extensions-legacy
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/hooks/api_extensions-v1
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/hooks/api_extensions-v2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/hooks/iptables_verify
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/post_test_hook.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.004929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2608 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9080 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10390 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14106 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/environment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6049 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/machine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8397 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7378 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/test_l3_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/db/test_migrations.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/privileged/test_dummy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7383 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/privileged/test_netlink_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/privileged/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/agents/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/agents/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/agents/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/agents/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/agents/drivers/iptables/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/agents/drivers/iptables/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25021 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/agents/drivers/iptables/test_log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/cmd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/cmd/upgrade_checks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/cmd/upgrade_checks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/cmd/upgrade_checks/test_checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/db/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/db/firewall/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/db/firewall/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/db/firewall/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/db/firewall/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    93235 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/db/firewall/v2/test_firewall_db_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/netfilter_log/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/netfilter_log/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5509 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/netfilter_log/test_libnetfilter_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15708 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/test_netlink_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.008930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/noop/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/noop/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/noop/test_noop_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32824 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/test_firewall.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13075 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/test_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23606 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_iptables_fwaas_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6649 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_legacy_conntrack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10470 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_netlink_conntrack.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5286 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/fake_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30424 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/test_fwaas_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l3reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l3reference/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27940 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l3reference/test_firewall_l3_agent_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29131 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_agents.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3217 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_firewall_agent_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2474 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_firewall_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13178 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/test_driver_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34200 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/test_fwaas_plugin_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.012930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.016930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14785 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/test_log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.016930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/l3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/l3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2206 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/l3/test_fwg_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.016930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9741 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/common/test_fwg_callback.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14732 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/common/test_log_db_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8648 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/common/test_port_callback.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.016930 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/rpc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2365 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/rpc/test_log_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6821 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/test_fwg_validate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.992929 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2124 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16247 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2024-03-14 06:25:28.000000 neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.016930 neutron-fwaas-20.0.0.0rc1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/playbooks/configure_functional_job.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.980929 neutron-fwaas-20.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/adding-new-tables-for-future-consumption-ffd537c1f82e2e01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/auto-association-default-firewall-group-7e9faf1afca1df85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/bug-1702242-c917c832ac2fa4e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/bug-1746404-493a66faac333403.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/bug-1799358-360c6ab27a32e0ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/cisco-fwaas-driver-move-8f46325d13c93543.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/coexistence-between-sg-and-fwg-1f77a755539a9463.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/config-file-generation-265c5256668a26bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/deprecate-neutron-fwaas-as-stadium-project-934d6acb3e824249.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/drop-python-2-7-73d3113c69d724c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-b1cf8738aaab988f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/enable-quotas-a3d0a21743bb1985.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/fwaas-config-9c780ccfb0e7887f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/fwaas-v2-logging-79cbaa43ff17f47f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/fwaas_v2-374471c215af0ca0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/mcafee-fwaas-driver-removal-8915271e5d4288cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/ovs-firewall-driver-c347ea0a560b7e38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/remove_fwaas_v1-15c6e19484f46d1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/validation_if_port_is_supported-639d0df705eb67f9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/varmour-fwaas-driver-removal-f7aa304a4544134a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/notes/vyatta-fwaas-driver-removal-e38e6ecde5105084.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9203 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.980929 neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.980929 neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17917 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.980929 neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:28.980929 neutron-fwaas-20.0.0.0rc1/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/roles/configure_functional_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/roles/configure_functional_tests/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/roles/configure_functional_tests/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/roles/configure_functional_tests/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.020930 neutron-fwaas-20.0.0.0rc1/roles/configure_functional_tests/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/roles/configure_functional_tests/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2024-03-14 06:25:29.024930 neutron-fwaas-20.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 06:25:29.024930 neutron-fwaas-20.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1613 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/tools/check_unit_test_structure.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      196 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/tools/clean.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8974 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/tools/configure_for_func_testing.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      850 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/tools/configure_for_fwaas_func_testing.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2180 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/tools/deploy_rootwrap.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      800 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/tools/generate_config_file_samples.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2024-03-14 06:24:57.000000 neutron-fwaas-20.0.0.0rc1/tox.ini
```

### Comparing `neutron-fwaas-20.0.0/.mailmap` & `neutron-fwaas-20.0.0.0rc1/.mailmap`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/.pylintrc` & `neutron-fwaas-20.0.0.0rc1/.pylintrc`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/.zuul.yaml` & `neutron-fwaas-20.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/AUTHORS` & `neutron-fwaas-20.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/ChangeLog` & `neutron-fwaas-20.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-20.0.0
-------
+20.0.0.0rc1
+-----------
 
 * Bump hacking
 * tox: Drop envdir
 * Update python classifier with py3.10 & py3.11 in setup.cfg
 * Remove usage of LBaaS constants
 * py311: Add py311 job and sqlalchemy-main job to weekly
 * [sqlalchemy-20] Replace the context writer/reader
```

### Comparing `neutron-fwaas-20.0.0/LICENSE` & `neutron-fwaas-20.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/PKG-INFO` & `neutron-fwaas-20.0.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-fwaas
-Version: 20.0.0
+Version: 20.0.0.0rc1
 Summary: OpenStack Networking FWaaS
 Home-page: https://docs.openstack.org/neutron-fwaas/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `neutron-fwaas-20.0.0/README.rst` & `neutron-fwaas-20.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/devstack/README.rst` & `neutron-fwaas-20.0.0.0rc1/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/devstack/lib/l2_agent` & `neutron-fwaas-20.0.0.0rc1/devstack/lib/l2_agent`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/devstack/lib/l3_agent` & `neutron-fwaas-20.0.0.0rc1/devstack/lib/l3_agent`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/devstack/plugin.sh` & `neutron-fwaas-20.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/doc/source/conf.py` & `neutron-fwaas-20.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/doc/source/configuration/index.rst` & `neutron-fwaas-20.0.0.0rc1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/doc/source/configuration/policy-sample.rst` & `neutron-fwaas-20.0.0.0rc1/doc/source/configuration/policy-sample.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/doc/source/contributor/contributing.rst` & `neutron-fwaas-20.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/doc/source/index.rst` & `neutron-fwaas-20.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/doc/source/install/index.rst` & `neutron-fwaas-20.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/__init__.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/_i18n.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/_i18n.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/cmd/upgrade_checks/checks.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/cmd/upgrade_checks/checks.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/cmd/v1_to_v2_db_migration.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/cmd/v1_to_v2_db_migration.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/common/exceptions.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/common/fwaas_constants.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/common/fwaas_constants.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/common/resources.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/common/resources.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/firewall/firewall_db.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/firewall/firewall_db.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/firewall/v2/firewall_db_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/firewall/v2/firewall_db_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/env.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/script.py.mako` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/2023.2/expand/6941ce70131e_add_standard_attr_id.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/2023.2/expand/6941ce70131e_add_standard_attr_id.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/4202e3047e47_add_index_tenant_id.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/4202e3047e47_add_index_tenant_id.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/540142f314f4_fwaas_router_insertion.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/540142f314f4_fwaas_router_insertion.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/796c68dffbb_cisco_csr_fwaas.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/796c68dffbb_cisco_csr_fwaas.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/kilo_release.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/kilo_release.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/contract/67c8e8d61d5_initial.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/contract/67c8e8d61d5_initial.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/4b47ea298795_add_reject_rule.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/4b47ea298795_add_reject_rule.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/c40fbb377ad_initial.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/liberty/expand/c40fbb377ad_initial.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/mitaka/contract/458aa42b14b_fw_table_alter.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/mitaka/contract/458aa42b14b_fw_table_alter.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/newton/contract/f83a0b2964d0_rename_tenant_to_project.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/newton/contract/f83a0b2964d0_rename_tenant_to_project.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/newton/expand/d6a12e637e28_neutron_fwaas_v2_0.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/newton/expand/d6a12e637e28_neutron_fwaas_v2_0.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/pike/contract/fd38cd995cc0_shared_attribute_for_firewall_resources.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/pike/contract/fd38cd995cc0_shared_attribute_for_firewall_resources.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/876782258a43_create_default_firewall_groups_table.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/876782258a43_create_default_firewall_groups_table.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/f24e0d5e5bff_uniq_firewallgroupportassociation0port.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/queens/expand/f24e0d5e5bff_uniq_firewallgroupportassociation0port.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/migration/alembic_migrations/versions/start_neutron_fwaas.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/migration/alembic_migrations/versions/start_neutron_fwaas.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/db/models/head.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/db/models/head.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/extensions/firewall_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/extensions/firewall_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/extensions/firewall_v2_stdattrs.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/extensions/firewall_v2_stdattrs.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/opts.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/opts.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/policies/__init__.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/policies/firewall_group.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/firewall_group.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/policies/firewall_policy.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/firewall_policy.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/policies/firewall_rule.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/policies/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/privileged/__init__.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/privileged/netfilter_log/libnetfilter_log.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/netfilter_log/libnetfilter_log.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/privileged/netlink_constants.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/netlink_constants.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/privileged/netlink_lib.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/netlink_lib.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/privileged/tests/functional/dummy.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/tests/functional/dummy.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/privileged/tests/functional/utils.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/privileged/utils.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/privileged/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/fwaas_plugin_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/fwaas_plugin_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/agents.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/conntrack_base.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/conntrack_base.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/fwaas_base.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/fwaas_base.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/fwaas_base_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/fwaas_base_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/iptables_fwaas_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/iptables_fwaas_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/driver_base.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/driver_base.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/noop/noop_driver.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/noop/noop_driver.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/__init__.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/constants.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/exceptions.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/firewall.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/firewall.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/rules.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/rules.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/legacy_conntrack.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/legacy_conntrack.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/netlink_conntrack.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/drivers/linux/netlink_conntrack.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/firewall_agent_api.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/firewall_agent_api.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/firewall_service.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/firewall_service.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/l2/fwaas_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/l2/fwaas_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/agents/l3reference/firewall_l3_agent_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/agents/l3reference/firewall_l3_agent_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/firewall/service_drivers/driver_api.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/firewall/service_drivers/driver_api.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/drivers/iptables/driver.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/drivers/iptables/driver.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/drivers/iptables/log.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/drivers/iptables/log.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/agents/l3/fwg_log.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/agents/l3/fwg_log.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/common/fwg_callback.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/common/fwg_callback.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/common/log_db_api.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/common/log_db_api.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/common/port_callback.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/common/port_callback.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/constants.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/exceptions.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/fwg_validate.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/fwg_validate.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/services/logapi/rpc/log_server.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/services/logapi/rpc/log_server.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/base.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/base.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/filters.template` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/filters.template`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/gate_hook.sh` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/gate_hook.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/gate_hook_tempest.sh` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/gate_hook_tempest.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/contrib/post_test_hook.sh` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/contrib/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/__init__.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/base.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/base.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/client.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/client.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/config.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/config.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/environment.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/environment.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/machine.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/machine.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/resources/process.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/resources/process.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/test_l3_agent.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/test_l3_agent.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/fullstack/utils.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/fullstack/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/db/test_migrations.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/privileged/test_dummy.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/privileged/test_dummy.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/privileged/test_netlink_lib.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/privileged/test_netlink_lib.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/privileged/test_utils.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/privileged/test_utils.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/functional/services/logapi/agents/drivers/iptables/test_log.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/functional/services/logapi/agents/drivers/iptables/test_log.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/cmd/upgrade_checks/test_checks.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/cmd/upgrade_checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/db/firewall/v2/test_firewall_db_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/db/firewall/v2/test_firewall_db_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/netfilter_log/test_libnetfilter_log.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/netfilter_log/test_libnetfilter_log.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/test_netlink_lib.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/test_netlink_lib.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/privileged/test_utils.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/privileged/test_utils.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/noop/test_noop_driver.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/noop/test_noop_driver.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/test_firewall.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/test_firewall.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/test_rules.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/l2/openvswitch_firewall/test_rules.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_iptables_fwaas_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_iptables_fwaas_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_legacy_conntrack.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_legacy_conntrack.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_netlink_conntrack.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/drivers/linux/test_netlink_conntrack.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/fake_data.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/fake_data.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/test_fwaas_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l2/test_fwaas_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l3reference/test_firewall_l3_agent_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/l3reference/test_firewall_l3_agent_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_agents.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_agents.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_firewall_agent_api.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_firewall_agent_api.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_firewall_service.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/agents/test_firewall_service.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/service_drivers/test_driver_api.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/service_drivers/test_driver_api.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/firewall/test_fwaas_plugin_v2.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/firewall/test_fwaas_plugin_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/test_driver.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/test_driver.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/test_log.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/drivers/iptables/test_log.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/agents/l3/test_fwg_log.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/agents/l3/test_fwg_log.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/base.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/base.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/common/test_fwg_callback.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/common/test_fwg_callback.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/common/test_log_db_api.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/common/test_log_db_api.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/common/test_port_callback.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/common/test_port_callback.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/rpc/test_log_server.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/rpc/test_log_server.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/tests/unit/services/logapi/test_fwg_validate.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/tests/unit/services/logapi/test_fwg_validate.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas/version.py` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas/version.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas.egg-info/PKG-INFO` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-fwaas
-Version: 20.0.0
+Version: 20.0.0.0rc1
 Summary: OpenStack Networking FWaaS
 Home-page: https://docs.openstack.org/neutron-fwaas/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas.egg-info/SOURCES.txt` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/neutron_fwaas.egg-info/entry_points.txt` & `neutron-fwaas-20.0.0.0rc1/neutron_fwaas.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/notes/coexistence-between-sg-and-fwg-1f77a755539a9463.yaml` & `neutron-fwaas-20.0.0.0rc1/releasenotes/notes/coexistence-between-sg-and-fwg-1f77a755539a9463.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/notes/deprecate-neutron-fwaas-as-stadium-project-934d6acb3e824249.yaml` & `neutron-fwaas-20.0.0.0rc1/releasenotes/notes/deprecate-neutron-fwaas-as-stadium-project-934d6acb3e824249.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/notes/enable-quotas-a3d0a21743bb1985.yaml` & `neutron-fwaas-20.0.0.0rc1/releasenotes/notes/enable-quotas-a3d0a21743bb1985.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/notes/fwaas-v2-logging-79cbaa43ff17f47f.yaml` & `neutron-fwaas-20.0.0.0rc1/releasenotes/notes/fwaas-v2-logging-79cbaa43ff17f47f.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/notes/fwaas_v2-374471c215af0ca0.yaml` & `neutron-fwaas-20.0.0.0rc1/releasenotes/notes/fwaas_v2-374471c215af0ca0.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/notes/ovs-firewall-driver-c347ea0a560b7e38.yaml` & `neutron-fwaas-20.0.0.0rc1/releasenotes/notes/ovs-firewall-driver-c347ea0a560b7e38.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/source/conf.py` & `neutron-fwaas-20.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-20.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/requirements.txt` & `neutron-fwaas-20.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/roles/configure_functional_tests/README.rst` & `neutron-fwaas-20.0.0.0rc1/roles/configure_functional_tests/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/roles/configure_functional_tests/tasks/main.yaml` & `neutron-fwaas-20.0.0.0rc1/roles/configure_functional_tests/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/setup.cfg` & `neutron-fwaas-20.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/setup.py` & `neutron-fwaas-20.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/test-requirements.txt` & `neutron-fwaas-20.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/tools/check_unit_test_structure.sh` & `neutron-fwaas-20.0.0.0rc1/tools/check_unit_test_structure.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/tools/configure_for_func_testing.sh` & `neutron-fwaas-20.0.0.0rc1/tools/configure_for_func_testing.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/tools/configure_for_fwaas_func_testing.sh` & `neutron-fwaas-20.0.0.0rc1/tools/configure_for_fwaas_func_testing.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/tools/deploy_rootwrap.sh` & `neutron-fwaas-20.0.0.0rc1/tools/deploy_rootwrap.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/tools/generate_config_file_samples.sh` & `neutron-fwaas-20.0.0.0rc1/tools/generate_config_file_samples.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-20.0.0/tox.ini` & `neutron-fwaas-20.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

