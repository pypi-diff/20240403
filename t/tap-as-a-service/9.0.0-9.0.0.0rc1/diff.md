# Comparing `tmp/tap-as-a-service-9.0.0.tar.gz` & `tmp/tap-as-a-service-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-as-a-service-9.0.0.tar", last modified: Wed Mar 30 11:59:47 2022, max compression
+gzip compressed data, was "tap-as-a-service-9.0.0.0rc1.tar", last modified: Thu Mar 10 08:43:07 2022, max compression
```

## Comparing `tap-as-a-service-9.0.0.tar` & `tap-as-a-service-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.783439 tap-as-a-service-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9938 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/API_REFERENCE.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1828 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8383 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/INSTALL.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2022-03-30 11:59:47.783439 tap-as-a-service-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.755439 tap-as-a-service-9.0.0/bin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/bin/i40e_sysfs_command
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.739439 tap-as-a-service-9.0.0/deliverables/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.755439 tap-as-a-service-9.0.0/deliverables/queens/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/deliverables/queens/tap-as-a-service.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.755439 tap-as-a-service-9.0.0/deliverables/rocky/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/deliverables/rocky/tap-as-a-service.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.755439 tap-as-a-service-9.0.0/deliverables/stein/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/deliverables/stein/tap-as-a-service.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.755439 tap-as-a-service-9.0.0/deliverables/train/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/deliverables/train/tap-as-a-service.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.755439 tap-as-a-service-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/devstack/devstackgaterc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.755439 tap-as-a-service-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.759439 tap-as-a-service-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/doc/source/api_reference.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2877 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/doc/source/presentations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.759439 tap-as-a-service-9.0.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.743439 tap-as-a-service-9.0.0/etc/neutron/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.759439 tap-as-a-service-9.0.0/etc/neutron/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/etc/neutron/rootwrap.d/taas-i40e-sysfs.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/etc/policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/etc/taas.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/etc/taas_plugin.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.759439 tap-as-a-service-9.0.0/neutron_taas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.759439 tap-as-a-service-9.0.0/neutron_taas/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/common/topics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/common/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.759439 tap-as-a-service-9.0.0/neutron_taas/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/head.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.759439 tap-as-a-service-9.0.0/neutron_taas/db/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.763439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.763439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/CONTRACT_HEAD
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/EXPAND_HEAD
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.743439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.763439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/1817af933379_remove_network_id_from_tap_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/2ecce0368a62_add_foreign_key_constraint_on_tap_id_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2872 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/4086b3cffc01_rename_tenant_to_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/80c85b675b6e_initial_newton_no_op_contract_script.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.763439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/expand/04625466c6fa_initial_newton_no_op_expand_script.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/expand/fddbdec8711a_add_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.743439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/pike/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.763439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/pike/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/pike/contract/bac61f603e39_alter_tap_id_associations_to_support_tap_id_reuse.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/start_neutron_taas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.743439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/stein/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.763439 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/stein/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/stein/expand/ccbcc559d175_add_vlan_filter_to_tap_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/migration/taas_init_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11499 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/db/taas_db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.767439 tap-as-a-service-9.0.0/neutron_taas/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8044 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/extensions/taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/extensions/vlan_filter.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.767439 tap-as-a-service-9.0.0/neutron_taas/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1702 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/policies/tap_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/policies/tap_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.767439 tap-as-a-service-9.0.0/neutron_taas/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.767439 tap-as-a-service-9.0.0/neutron_taas/services/taas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.767439 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.767439 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10013 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/common/taas_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.767439 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2676 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/extensions/taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/taas_agent_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.767439 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.771439 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/ovs_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21313 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/ovs_taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2726 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/ovs_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/sriov_nic_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16812 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/sriov_nic_taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11246 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/sriov_nic_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.771439 tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2240 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/service_driver_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/taas_agent_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13929 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/taas_rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8869 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/services/taas/taas_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.771439 tap-as-a-service-9.0.0/neutron_taas/taas_client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/taas_client/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.771439 tap-as-a-service-9.0.0/neutron_taas/taas_client/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/taas_client/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8725 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/taas_client/osc/tap_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7593 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/taas_client/osc/tap_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4155 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/taas_client/tapflow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/taas_client/tapservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.775439 tap-as-a-service-9.0.0/neutron_taas/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.775439 tap-as-a-service-9.0.0/neutron_taas/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.775439 tap-as-a-service-9.0.0/neutron_taas/tests/unit/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2329 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/db/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10007 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/db/test_taas_db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.775439 tap-as-a-service-9.0.0/neutron_taas/tests/unit/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/extensions/test_taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3858 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/extensions/test_vlan_filter.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.775439 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.775439 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10757 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/drivers/test_linux_sriov_nic_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12507 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/drivers/test_linux_sriov_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.775439 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/taas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/taas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13249 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/taas/test_taas_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.779439 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.779439 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2921 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9088 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/osc/test_osc_tap_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8283 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/osc/test_osc_tap_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4828 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/test_cli20_tapflow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4997 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/test_cli20_tapservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/openstack-common.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.747439 tap-as-a-service-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.779439 tap-as-a-service-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/notes/bp-port-mirroring-sriov-vf-879bc2aa53c2c8d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/notes/clear-tap-resources-on-port-delete-9583cdd7cd6098ea.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.779439 tap-as-a-service-9.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.779439 tap-as-a-service-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10509 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2022-03-30 11:59:47.787439 tap-as-a-service-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.779439 tap-as-a-service-9.0.0/specs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/specs/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.783439 tap-as-a-service-9.0.0/specs/mitaka/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20945 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/specs/mitaka/tap-as-a-service.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.783439 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5971 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1503 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-03-30 11:59:47.000000 tap-as-a-service-9.0.0/tap_as_a_service.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:47.783439 tap-as-a-service-9.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1980 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3061 2022-03-30 11:59:06.000000 tap-as-a-service-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.562265 tap-as-a-service-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9938 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/API_REFERENCE.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1828 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8393 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/INSTALL.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2022-03-10 08:43:07.562265 tap-as-a-service-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.538265 tap-as-a-service-9.0.0.0rc1/bin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/bin/i40e_sysfs_command
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.530264 tap-as-a-service-9.0.0.0rc1/deliverables/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.538265 tap-as-a-service-9.0.0.0rc1/deliverables/queens/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/deliverables/queens/tap-as-a-service.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.538265 tap-as-a-service-9.0.0.0rc1/deliverables/rocky/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/deliverables/rocky/tap-as-a-service.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.538265 tap-as-a-service-9.0.0.0rc1/deliverables/stein/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/deliverables/stein/tap-as-a-service.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.538265 tap-as-a-service-9.0.0.0rc1/deliverables/train/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/deliverables/train/tap-as-a-service.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.538265 tap-as-a-service-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/devstack/devstackgaterc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.538265 tap-as-a-service-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.542265 tap-as-a-service-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/doc/source/api_reference.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2877 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/doc/source/presentations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.542265 tap-as-a-service-9.0.0.0rc1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.530264 tap-as-a-service-9.0.0.0rc1/etc/neutron/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.542265 tap-as-a-service-9.0.0.0rc1/etc/neutron/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/etc/neutron/rootwrap.d/taas-i40e-sysfs.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/etc/policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/etc/taas.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/etc/taas_plugin.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.542265 tap-as-a-service-9.0.0.0rc1/neutron_taas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.542265 tap-as-a-service-9.0.0.0rc1/neutron_taas/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/common/topics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.542265 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/head.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.546265 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.546265 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.546265 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/CONTRACT_HEAD
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/EXPAND_HEAD
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.530264 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.546265 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/1817af933379_remove_network_id_from_tap_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/2ecce0368a62_add_foreign_key_constraint_on_tap_id_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2872 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/4086b3cffc01_rename_tenant_to_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/80c85b675b6e_initial_newton_no_op_contract_script.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.546265 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/expand/04625466c6fa_initial_newton_no_op_expand_script.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/expand/fddbdec8711a_add_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.530264 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/pike/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.546265 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/pike/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/pike/contract/bac61f603e39_alter_tap_id_associations_to_support_tap_id_reuse.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/start_neutron_taas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.530264 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/stein/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.546265 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/stein/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/stein/expand/ccbcc559d175_add_vlan_filter_to_tap_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/taas_init_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11499 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/db/taas_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.546265 tap-as-a-service-9.0.0.0rc1/neutron_taas/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8044 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/extensions/taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/extensions/vlan_filter.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.550265 tap-as-a-service-9.0.0.0rc1/neutron_taas/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1702 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/policies/tap_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/policies/tap_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.550265 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.550265 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.550265 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.550265 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10013 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/common/taas_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.550265 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2676 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/extensions/taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/taas_agent_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.550265 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.550265 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/ovs_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21313 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/ovs_taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2726 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/ovs_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/sriov_nic_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16812 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/sriov_nic_taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11246 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/sriov_nic_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.554265 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2240 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/service_driver_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/taas_agent_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13929 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/taas_rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8869 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/taas_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.554265 tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.554265 tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8725 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/osc/tap_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7593 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/osc/tap_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4155 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/tapflow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/tapservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.554265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.554265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.554265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2329 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/db/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10007 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/db/test_taas_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.554265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/extensions/test_taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3858 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/extensions/test_vlan_filter.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.554265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.558265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10757 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/drivers/test_linux_sriov_nic_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12507 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/drivers/test_linux_sriov_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.558265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/taas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/taas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13249 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/taas/test_taas_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.558265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.558265 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2921 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9088 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/osc/test_osc_tap_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8283 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/osc/test_osc_tap_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4828 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/test_cli20_tapflow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4997 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/test_cli20_tapservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/openstack-common.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.534264 tap-as-a-service-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.558265 tap-as-a-service-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/notes/bp-port-mirroring-sriov-vf-879bc2aa53c2c8d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/notes/clear-tap-resources-on-port-delete-9583cdd7cd6098ea.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.558265 tap-as-a-service-9.0.0.0rc1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.562265 tap-as-a-service-9.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10509 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2022-03-10 08:43:07.566266 tap-as-a-service-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.562265 tap-as-a-service-9.0.0.0rc1/specs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/specs/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.562265 tap-as-a-service-9.0.0.0rc1/specs/mitaka/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20945 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/specs/mitaka/tap-as-a-service.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.562265 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5971 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1503 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-03-10 08:43:07.000000 tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:07.562265 tap-as-a-service-9.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1980 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3061 2022-03-10 08:42:27.000000 tap-as-a-service-9.0.0.0rc1/tox.ini
```

### Comparing `tap-as-a-service-9.0.0/.zuul.yaml` & `tap-as-a-service-9.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/API_REFERENCE.rst` & `tap-as-a-service-9.0.0.0rc1/API_REFERENCE.rst`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/AUTHORS` & `tap-as-a-service-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/CONTRIBUTING.rst` & `tap-as-a-service-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/ChangeLog` & `tap-as-a-service-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Use ovs TUNNEL\_ constants from new location
 * Execute neutron-db-manage only if q-svc is enabled
 * CLI: remove leftover logs from tap-flow create
 * Update leftover x namespace to openstack
 
 8.0.0
```

### Comparing `tap-as-a-service-9.0.0/INSTALL.rst` & `tap-as-a-service-9.0.0.0rc1/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/LICENSE` & `tap-as-a-service-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/PKG-INFO` & `tap-as-a-service-9.0.0.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tap-as-a-service
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Tap-as-a-Service (TaaS) is an extension to the OpenStack network service (Neutron), it provides remote port mirroring capability for tenant virtual networks.
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ================
         Tap as a Service
```

### Comparing `tap-as-a-service-9.0.0/README.rst` & `tap-as-a-service-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/bin/i40e_sysfs_command` & `tap-as-a-service-9.0.0.0rc1/bin/i40e_sysfs_command`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/devstack/devstackgaterc` & `tap-as-a-service-9.0.0.0rc1/devstack/devstackgaterc`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/devstack/plugin.sh` & `tap-as-a-service-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/doc/source/conf.py` & `tap-as-a-service-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/doc/source/index.rst` & `tap-as-a-service-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/doc/source/presentations.rst` & `tap-as-a-service-9.0.0.0rc1/doc/source/presentations.rst`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/_i18n.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/_i18n.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/common/constants.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/common/constants.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/common/topics.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/common/topics.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/common/utils.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/common/utils.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/head.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/head.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/env.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/env.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/1817af933379_remove_network_id_from_tap_service.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/1817af933379_remove_network_id_from_tap_service.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/2ecce0368a62_add_foreign_key_constraint_on_tap_id_association.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/2ecce0368a62_add_foreign_key_constraint_on_tap_id_association.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/4086b3cffc01_rename_tenant_to_project.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/4086b3cffc01_rename_tenant_to_project.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/contract/80c85b675b6e_initial_newton_no_op_contract_script.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/contract/80c85b675b6e_initial_newton_no_op_contract_script.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/expand/04625466c6fa_initial_newton_no_op_expand_script.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/expand/04625466c6fa_initial_newton_no_op_expand_script.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/newton/expand/fddbdec8711a_add_status.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/newton/expand/fddbdec8711a_add_status.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/pike/contract/bac61f603e39_alter_tap_id_associations_to_support_tap_id_reuse.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/pike/contract/bac61f603e39_alter_tap_id_associations_to_support_tap_id_reuse.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/start_neutron_taas.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/start_neutron_taas.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/alembic_migration/versions/stein/expand/ccbcc559d175_add_vlan_filter_to_tap_flow.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/alembic_migration/versions/stein/expand/ccbcc559d175_add_vlan_filter_to_tap_flow.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/migration/taas_init_ops.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/migration/taas_init_ops.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/db/taas_db.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/db/taas_db.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/extensions/taas.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/extensions/taas.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/extensions/vlan_filter.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/extensions/vlan_filter.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/policies/__init__.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/policies/tap_flow.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/policies/tap_flow.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/policies/tap_service.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/policies/tap_service.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/common/taas_agent.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/common/taas_agent.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/extensions/taas.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/extensions/taas.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/agents/taas_agent_api.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/agents/taas_agent_api.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/ovs_constants.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/ovs_constants.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/ovs_taas.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/ovs_taas.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/ovs_utils.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/ovs_utils.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/sriov_nic_exceptions.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/sriov_nic_exceptions.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/sriov_nic_taas.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/sriov_nic_taas.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/drivers/linux/sriov_nic_utils.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/drivers/linux/sriov_nic_utils.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/__init__.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/service_driver_context.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/service_driver_context.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/taas_agent_api.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/taas_agent_api.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/service_drivers/taas_rpc.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/service_drivers/taas_rpc.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/services/taas/taas_plugin.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/services/taas/taas_plugin.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/taas_client/osc/tap_flow.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/osc/tap_flow.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/taas_client/osc/tap_service.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/osc/tap_service.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/taas_client/tapflow.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/tapflow.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/taas_client/tapservice.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/taas_client/tapservice.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/base.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/base.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/db/test_migrations.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/db/test_taas_db.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/db/test_taas_db.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/extensions/test_taas.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/extensions/test_taas.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/extensions/test_vlan_filter.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/extensions/test_vlan_filter.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/drivers/test_linux_sriov_nic_driver.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/drivers/test_linux_sriov_nic_driver.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/drivers/test_linux_sriov_utils.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/drivers/test_linux_sriov_utils.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/services/taas/test_taas_plugin.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/services/taas/test_taas_plugin.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/osc/fakes.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/osc/test_osc_tap_flow.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/osc/test_osc_tap_flow.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/osc/test_osc_tap_service.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/osc/test_osc_tap_service.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/test_cli20_tapflow.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/test_cli20_tapflow.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/neutron_taas/tests/unit/taas_client/test_cli20_tapservice.py` & `tap-as-a-service-9.0.0.0rc1/neutron_taas/tests/unit/taas_client/test_cli20_tapservice.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/releasenotes/notes/bp-port-mirroring-sriov-vf-879bc2aa53c2c8d4.yaml` & `tap-as-a-service-9.0.0.0rc1/releasenotes/notes/bp-port-mirroring-sriov-vf-879bc2aa53c2c8d4.yaml`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/releasenotes/source/conf.py` & `tap-as-a-service-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/setup.cfg` & `tap-as-a-service-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/setup.py` & `tap-as-a-service-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/specs/mitaka/tap-as-a-service.rst` & `tap-as-a-service-9.0.0.0rc1/specs/mitaka/tap-as-a-service.rst`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/tap_as_a_service.egg-info/PKG-INFO` & `tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tap-as-a-service
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Tap-as-a-Service (TaaS) is an extension to the OpenStack network service (Neutron), it provides remote port mirroring capability for tenant virtual networks.
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ================
         Tap as a Service
```

### Comparing `tap-as-a-service-9.0.0/tap_as_a_service.egg-info/SOURCES.txt` & `tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/tap_as_a_service.egg-info/entry_points.txt` & `tap-as-a-service-9.0.0.0rc1/tap_as_a_service.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/test-requirements.txt` & `tap-as-a-service-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/tools/test-setup.sh` & `tap-as-a-service-9.0.0.0rc1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `tap-as-a-service-9.0.0/tox.ini` & `tap-as-a-service-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

